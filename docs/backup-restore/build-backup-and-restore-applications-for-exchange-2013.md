---
title: Créer des applications de sauvegarde et de restauration pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Trouvez des informations sur les composants et l’architecture des applications de sauvegarde et de restauration pour Exchange 2013, ainsi que la configuration système requise pour la création d’une application de sauvegarde et de restauration.
ms.openlocfilehash: f8a332d0816792f8888c97a8394886b026f5204b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455270"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Créer des applications de sauvegarde et de restauration pour Exchange 2013

Trouvez des informations sur les composants et l’architecture des applications de sauvegarde et de restauration pour Exchange 2013, ainsi que la configuration système requise pour la création d’une application de sauvegarde et de restauration.
  
**S’applique à :** Exchange Server 2013 
  
Vous pouvez utiliser le [service VSS (Volume Shadow Copy Service)](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) dans les versions de Windows Server commençant par windows Server 2008 pour créer des applications qui sauvegardent et restaurent les données Exchange Server 2013. VSS fournit une infrastructure qui vous permet de créer et de gérer des clichés instantanés entre des systèmes de gestion de stockage tiers, des applications métiers et du matériel. Vous pouvez créer des solutions basées sur l’infrastructure VSS qui utilise des clichés instantanés pour sauvegarder et restaurer une ou plusieurs bases de données Exchange 2013. 
  
## <a name="backup-and-restore-application-prerequisites"></a>Configuration requise pour la sauvegarde et la restauration
<a name="bk_systemrequirements"> </a>

Pour que votre application de sauvegarde et de restauration personnalisée et VSS puisse sauvegarder et restaurer les bases de données Exchange 2013, votre environnement doit inclure les éléments suivants :
  
- Une version de Windows Server à partir de Windows Server 2008 
    
- Exchange 2013
    
En outre, si vous créez une application de sauvegarde et de restauration, vous devez prendre en compte les restrictions suivantes sur l’environnement de développement :
  
- VSS est une API COM non managée accessible à partir du code managé .NET Framework via un assembly d’interopérabilité COM.
    
- L’environnement de commande Exchange Management Shell est une application gérée accessible via le code managé .NET Framework.
    
- L’API CHKSGFILES fournie avec Exchange 2013 est une DLL 64 bits native. L’utilisation de la DLL CHKSGFILES Exchange 2007 32 bits avec les bases de données Exchange 2013 n’est pas prise en charge.
    
## <a name="backup-and-restore-application-overview"></a>Vue d’ensemble de l’application de sauvegarde et de restauration
<a name="bk_components"> </a>

VSS coordonne la communication entre les composants suivants : 
  
- Le demandeur VSS, qui est votre application de sauvegarde
    
- Enregistreur VSS
    
- Le fournisseur VSS, qui est le système, le logiciel ou les composants matériels qui créent les clichés instantanés
    
Pour utiliser VSS afin de sauvegarder les données Exchange 2013, votre application de sauvegarde doit être un demandeur VSS Exchange 2013. Exchange 2013 inclut un enregistreur VSS, appelé le rédacteur Microsoft Exchange, pour le programme de sauvegarde de Windows Server ; Toutefois, l’enregistreur Exchange sauvegarde uniquement les volumes entiers. Il ne sauvegarde pas les bases de données Exchange 2013 individuelles. Si vous avez besoin d’une plus grande flexibilité, vous pouvez utiliser une application de sauvegarde tierce qui dispose d’un enregistreur VSS compatible avec Exchange, qui peut fonctionner avec des bases de données Exchange individuelles, ou vous pouvez créer un demandeur VSS personnalisé.
  
Avant que votre application appelle VSS pour lancer une sauvegarde, elle doit obtenir des informations sur la configuration de stockage du système Exchange 2013 qu’elle sauvegarde. Ces informations sont stockées dans les services de domaine Active Directory (AD DS). Votre application de sauvegarde peut obtenir des données de configuration du stockage Exchange à l’aide de commandes Exchange Management Shell. Pour plus d’informations, consultez la rubrique [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
Les applications de sauvegarde Exchange 2013 appellent les API VSS COM pour créer des sauvegardes complètes, copiées, différentielles et incrémentielles des bases de données Exchange ; elles n’interagissent pas directement avec l’enregistreur VSS. La fonctionnalité de groupe de disponibilité de base de données (DAG) dans Exchange permet également à votre application de créer une sauvegarde entièrement cohérente, même si la sauvegarde complète initiale et les sauvegardes incrémentielles ultérieures proviennent de différents serveurs dans le DAG. Une fois que VSS a créé la copie des données Exchange, votre application de sauvegarde stocke les données sur le support prévu.
  
Pour restaurer une base de données Exchange 2013, votre application de restauration récupère la base de données et les fichiers journaux à partir du support de sauvegarde et les stocke sur le stockage de disque actif d’un serveur Exchange. Les bases de données individuelles ne sont pas associées à un serveur Exchange particulier. 
  
Les applications de sauvegarde et de restauration doivent spécifier un certain nombre de paramètres Exchange 2013 spécifiques pour contrôler et gérer correctement les opérations exécutées par VSS sur les bases de données Exchange 2013. Par exemple, étant donné qu’Exchange 2013 prend en charge jusqu’à 100 bases de données simultanément actives, l’application de sauvegarde doit spécifier et traiter correctement les composants de base de données fichier de base de données, fichiers journaux de transactions et fichier de point de contrôle.
  
Pour reconstruire une base de données ayant subi des modifications depuis la dernière sauvegarde complète, votre application de restauration requiert des fichiers journaux et de base de données provenant de différentes sauvegardes. Par exemple, il peut s’avérer nécessaire de demander une sauvegarde complète hebdomadaire et une ou plusieurs sauvegardes incrémentielles quotidiennes. Dans les systèmes Exchange 2013 qui utilisent Dag, votre application de restauration peut reconstruire une base de données en utilisant des sauvegardes de différentes copies de bases de données sur des serveurs différents dans le même DAG. Toutefois, la seule façon de restaurer une base de données DAG à partir d’une sauvegarde est de restaurer toutes les copies actives et passives de la base de données à l’aide des mêmes données.
  
Une fois toutes les données en place, votre application de restauration signale à Exchange l’intégrité de la base de données et des fichiers journaux. Si la base de données et les fichiers journaux ont été restaurés correctement, le serveur Exchange peut ensuite relire les fichiers journaux de la base de données pour mettre à jour la base de données et la monter. Si la base de données a été récupérée sur un serveur qui possède déjà une copie active de la base de données montée, la base de données est traitée comme une base de données de récupération. Si la base de données a été récupérée sur un autre serveur, la base de données peut être montée de manière indépendante, ou ce réplica peut ensuite être ajouté au DAG.
  
## <a name="backup-and-restore-system-architecture"></a>Architecture du système de sauvegarde et de restauration
<a name="bk_ExchangeVSS"> </a>

VSS communique avec le système de fichiers Windows Server et avec le pilote de périphérique de stockage de masse via un fournisseur tiers (ou personnalisé). Le fournisseur de matériel détermine où le cliché instantané sera créé. VSS extrait le cliché instantané propre au matériel de sorte que votre application de sauvegarde et de restauration puisse accéder au cliché instantané sans informations sur les détails de l’implémentation matérielle. La figure suivante illustre l’interaction de votre application de sauvegarde et de restauration avec Exchange 2013 et Windows Server.
  
**Figure 1. Architecture du système de sauvegarde et de restauration**

![Diagramme présentant les interactions entre une application de sauvegarde et de restauration. La communication à double sens existe entre Exchange, Windows Server et l’application cliente. Le serveur Windows interagit également avec un dispositif de stockage de masse ou un média de sauvegarde.](media/VSS_architecture_E2k7.gif)
  
L’application de sauvegarde et de restauration fonctionne comme demandeur VSS. Le demandeur communique avec VSS pour obtenir des informations sur Exchange 2013, pour lancer la création de clichés instantanés et pour accéder aux données de sauvegarde. 
  
La Banque d’aide Exchange est un composant d’Exchange 2013 et accède aux bases de données Exchange 2013 via le système de fichiers Windows Server. Dans le système de fichiers, chaque serveur Exchange peut monter simultanément jusqu’à 100 bases de données avec les fichiers de base de données (. edb) associés, les fichiers journaux de transactions et un fichier de point de contrôle.
  
Pour prendre en charge VSS, Exchange 2013 inclut un enregistreur Exchange qui est intégré à la Banque d’aide Exchange. Le rédacteur Exchange coordonne avec la banque Exchange (fonctionnant pour le compte du demandeur) de geler et démonter la base de données avant de la sauvegarder, puis de libérer et de monter la base de données une fois la sauvegarde terminée. Pendant une restauration, votre application de sauvegarde et de restauration demande à l’enregistreur Exchange de se coordonner avec la Banque d’aide Exchange pour démonter la base de données, remplacer les fichiers de base de données, monter la base de données, puis relire les journaux de transactions (le cas échéant).
  
Pendant une restauration, le demandeur communique également avec VSS pour préparer le système pour la restauration, puis replace les données sur le périphérique de stockage de masse. Votre application de sauvegarde et de restauration est également chargée de travailler avec Windows Server pour lire et écrire des données sur le support de stockage de sauvegarde, qu’il s’agisse d’une archive sur bande, d’un réseau de zone de stockage ou d’un autre support de sauvegarde.
  
La base de données restaurée peut être montée en tant que base de données régulière, active ou en tant que base de données de récupération Exchange 2013. Une seule base de données montée peut être désignée comme base de données de récupération sur chaque serveur Exchange.
  
Les informations nécessaires pour effectuer correctement les opérations de sauvegarde et de restauration entre Exchange 2013, VSS et votre application de sauvegarde et de restauration sont transférées dans le cadre des métadonnées du rédacteur Exchange.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Restauration des bases de données Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Valider l’intégrité de la sauvegarde à l’aide de l’outil Eseutil dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Sauvegarde et restauration pour Exchange](backup-and-restore-for-exchange-2013.md) 
- [Référence de classe fonction cchksgfiles](cchksgfiles-class-reference.md) 
- [Service de cliché instantané de volume](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

