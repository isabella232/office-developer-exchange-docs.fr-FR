---
title: Créer des applications de sauvegarde et de restauration pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Recherchez des informations sur les composants et l’architecture des applications de sauvegarde et de restauration pour Exchange 2013, ainsi que sur la requise pour la création d’une application de sauvegarde et de restauration.
ms.openlocfilehash: 590ac029e157196d370cbcbe54e5df75bc1a830b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513877"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Créer des applications de sauvegarde et de restauration pour Exchange 2013

Recherchez des informations sur les composants et l’architecture des applications de sauvegarde et de restauration pour Exchange 2013, ainsi que sur la requise pour la création d’une application de sauvegarde et de restauration.
  
**S’applique à :** Exchange Server 2013 
  
Vous pouvez utiliser le [service VSS (Volume Shadow Copy Service)](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) dans les versions de Windows Server à partir de Windows Server 2008 pour créer des applications qui back up and restore Exchange Server 2013 data. VSS fournit une infrastructure qui vous permet de créer et de gérer des shadow copies sur des systèmes de gestion de stockage tiers, des applications métiers et du matériel. Vous pouvez créer des solutions basées sur l’infrastructure VSS qui utilisent des copies de l’ombre pour la back up et la restauration d’Exchange bases de données 2013. 
  
## <a name="backup-and-restore-application-prerequisites"></a>Conditions préalables à la sauvegarde et à la restauration de l’application
<a name="bk_systemrequirements"> </a>

Pour que votre application de sauvegarde et de restauration personnalisée et VSS sauvegarde et restaure des bases de données Exchange 2013, votre environnement doit inclure les options suivantes :
  
- Une version de Windows Server commençant par Windows Server 2008 
    
- Exchange 2013
    
En outre, si vous créez une application de sauvegarde et de restauration, vous devez connaître les restrictions suivantes sur l’environnement de développement :
  
- VSS est une API COM non gérée accessible à partir .NET Framework code géré via un assembly COM Interop.
    
- L Exchange Management Shell est une application gérée accessible via .NET Framework code géré.
    
- L’API CHKSGFILES fournie avec Exchange 2013 est une DLL 64 bits de code natif. L’utilisation Exchange DLL CHKSGFILES 32 bits 2007 avec Exchange bases de données 2013 n’est pas prise en charge.
    
## <a name="backup-and-restore-application-overview"></a>Vue d’ensemble de l’application de sauvegarde et de restauration
<a name="bk_components"> </a>

VSS coordonne la communication entre les composants suivants : 
  
- Demandeur VSS, qui est votre application de sauvegarde
    
- Rédacteur VSS
    
- Le fournisseur VSS, qui est le système, les logiciels ou les composants matériels qui créent les copies de l’ombre
    
Pour utiliser VSS afin de sauvegarder Exchange 2013, votre application de sauvegarde doit être un demandeur VSS Exchange 2013. Exchange 2013 inclut un rédacteur VSS, appelé Microsoft Exchange Writer, pour le programme de sauvegarde Windows Server ; toutefois, le rédacteur Exchange uniquement les volumes entiers. Il ne permet pas de Exchange bases de données 2013 individuelles. Si vous avez besoin de plus de flexibilité, vous pouvez utiliser une application de sauvegarde tierce qui dispose d’un rédacteur VSS Exchange qui peut fonctionner avec des bases de données Exchange individuelles, ou vous pouvez créer un demandeur VSS personnalisé.
  
Avant que votre application appelle VSS pour lancer une sauvegarde, elle doit obtenir des informations sur la configuration de stockage pour le système Exchange 2013 qu’elle sauvegarde. Ces informations sont stockées dans les services de domaine Active Directory (AD DS). Votre application de sauvegarde peut obtenir des Exchange de configuration de stockage à l’aide Exchange commandes de Management Shell. Pour plus d’informations, [voir Exchange Server PowerShell (Exchange Management Shell).](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
  
Exchange 2013 appellent les API COM VSS pour créer des sauvegardes complètes, de copie, différentielle et incrémentielles de bases de données Exchange données ; Ils n’interagissent pas directement avec le rédacteur VSS. La fonctionnalité de groupe de disponibilité de base de données (DAG) dans Exchange permet également à votre application de créer une sauvegarde entièrement cohérente, même si la sauvegarde complète initiale et les sauvegardes incrémentielles ultérieures proviennent de différents serveurs du DAG. Une fois que VSS a créé la copie des Exchange, votre application de sauvegarde stocke les données sur le support prévu.
  
Pour restaurer une base de données Exchange 2013, votre application de restauration récupère la base de données et les fichiers journaux du support de sauvegarde et les stocke sur le stockage de disque actif d’un serveur Exchange. Les bases de données individuelles ne sont pas associées à un serveur Exchange spécifique. 
  
Les applications de sauvegarde et de restauration doivent spécifier un certain nombre de paramètres spécifiques Exchange 2013 pour contrôler et gérer correctement les opérations exécutés par VSS sur les bases de données Exchange 2013. Par exemple, comme Exchange 2013 prend en charge jusqu’à 100 bases de données actives simultanément, l’application de sauvegarde doit spécifier et traiter correctement le fichier de base de données, les fichiers journaux des transactions et les composants de base de données de fichiers de point de contrôle.
  
Pour reconstruire une base de données qui avait des modifications depuis la dernière restauration complète, votre application de restauration nécessite des fichiers de base de données et des fichiers journaux de différentes sauvegardes. Par exemple, il peut nécessiter une sauvegarde complète hebdomadaire et une ou plusieurs sauvegardes incrémentielles quotidiennes. Dans Exchange 2013 qui utilisent des DAG, votre application de restauration peut reconstruire une base de données à l’aide de sauvegardes de différentes copies de base de données sur différents serveurs dans le même DAG. Toutefois, le seul moyen pris en charge pour restaurer une base de données DAG à partir d’une sauvegarde consiste à restaurer toutes les copies actives et passives de la base de données à l’aide des mêmes données.
  
Une fois toutes les données en place, votre application de restauration signale Exchange vérifier l’intégrité de la base de données et des fichiers journaux. Si la base de données et les fichiers journaux ont été restaurés correctement, le serveur Exchange peut ensuite relire les fichiers journaux de base de données pour mettre la base de données à jour et la monter. Si la base de données a été récupérée sur un serveur qui dispose déjà d’une copie active de la base de données montée, la base de données est traitée comme une base de données de récupération. Si la base de données a été récupérée sur un autre serveur, la base de données peut être montée indépendamment ou ce réplica peut être ajouté au DAG.
  
## <a name="backup-and-restore-system-architecture"></a>Architecture système de sauvegarde et de restauration
<a name="bk_ExchangeVSS"> </a>

VSS communique avec le système de fichiers Windows Server et avec le pilote de périphérique de stockage de masse via un fournisseur tiers (ou personnalisé). Le fournisseur de matériel détermine l’endroit où le shadow copy sera créé. VSS extrait le shadow copy spécifique au matériel afin que votre application de sauvegarde et de restauration puisse accéder au shadow copy sans informations sur les détails d’implémentation matérielle. La figure suivante montre comment votre application de sauvegarde et de restauration interagit avec Exchange 2013 et Windows Server.
  
**Figure 1. Architecture système de sauvegarde et de restauration**

![Diagramme présentant les interactions entre une application de sauvegarde et de restauration. La communication à double sens existe entre Exchange, Windows Server et l’application cliente. Le serveur Windows interagit également avec un dispositif de stockage de masse ou un média de sauvegarde.](media/VSS_architecture_E2k7.gif)
  
L’application de sauvegarde et de restauration fonctionne en tant que demandeur VSS. Le demandeur communique avec VSS pour obtenir des informations sur Exchange 2013, pour lancer la création de copies de secours et accéder aux données de sauvegarde. 
  
Le magasin Exchange est un composant de Exchange 2013 et accède aux bases de données Exchange 2013 via le système de fichiers Windows Server. Dans le système de fichiers, chaque serveur Exchange peut monter simultanément jusqu’à 100 bases de données avec les fichiers de base de données (.edb) qui l’accompagnent, les fichiers journaux des transactions et un fichier de point de contrôle.
  
Pour prendre en charge VSS, Exchange 2013 inclut un rédacteur Exchange intégré au Exchange store. Le rédacteur Exchange se coordonne avec le magasin Exchange (fonctionnant au nom du demandeur) pour figer et démonter la base de données avant de la sauvegarder, puis pour libérer et monter la base de données une fois la sauvegarde terminée. Lors d’une restauration, votre application de sauvegarde et de restauration demande à l’enregistreur Exchange de se coordonner avec le magasin Exchange pour démonter la base de données, remplacer les fichiers de base de données, monter la base de données, puis relire les journaux des transactions (si nécessaire).
  
Lors d’une restauration, le demandeur communique également avec VSS pour préparer le système à la restauration, puis pour remettre les données sur le périphérique de stockage de masse. Votre application de sauvegarde et de restauration est également responsable de l’utilisation de Windows Server pour lire et écrire des données sur le support de stockage de sauvegarde, qu’il s’agit d’une archive de bande, d’un réseau de stockage ou d’un autre support de sauvegarde.
  
La base de données restaurée peut être montée en tant que base de données normale et active ou en tant que base de données de récupération Exchange 2013. Une seule base de données montée peut être désignée comme base de données de récupération sur Exchange serveur.
  
Les informations requises pour effectuer correctement les opérations de sauvegarde et de restauration entre Exchange 2013, VSS et votre application de sauvegarde et restauration sont transférées dans le cadre des métadonnées du rédacteur Exchange.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Types d’opérations de sauvegarde Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Restauration de Exchange bases de données 2013](restoring-exchange-2013-databases.md)
    
- [Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validation de l’intégrité de la sauvegarde à l’aide de l’outil Eseutil Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Sauvegarde et restauration pour Exchange](backup-and-restore-for-exchange-2013.md) 
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md) 
- [Service de cliché instantané de volume](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

