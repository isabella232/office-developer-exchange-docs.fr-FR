---
title: Créer la sauvegarde et de restaurer des applications pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Trouvez des informations sur les composants et l’architecture des applications de sauvegarde et de restauration pour Exchange 2013 et la configuration système requise pour la création d’une sauvegarde et restauration d’application.
ms.openlocfilehash: e85a5364c40c472c9e1ea9d1d3b4e89329b1676f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754754"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Créer la sauvegarde et de restaurer des applications pour Exchange 2013

Trouvez des informations sur les composants et l’architecture des applications de sauvegarde et de restauration pour Exchange 2013 et la configuration système requise pour la création d’une sauvegarde et restauration d’application.
  
**S’applique à :** Exchange Server 2013 
  
Vous pouvez utiliser le [Volume Shadow Copy Service (VSS)](http://msdn.microsoft.com/en-us/library/bb968832%28VS.85%29.aspx) dans les versions de Windows Server à partir de Windows Server 2008 pour créer des applications pour sauvegarder et restaurer des données Exchange Server 2013. VSS fournit une infrastructure qui permet de créer et gérer des clichés instantanés sur le matériel, applications d’entreprise et les systèmes de gestion de stockage tiers. Vous pouvez créer des solutions basées sur l’infrastructure VSS qui utilisent des clichés instantanés pour sauvegarder et restaurer une ou plusieurs bases de données Exchange 2013. 
  
## <a name="backup-and-restore-application-prerequisites"></a>Conditions préalables application sauvegarde et restauration
<a name="bk_systemrequirements"> </a>

Dans l’ordre pour votre sauvegarde personnalisée et application de restauration VSS pour sauvegarder et restaurer des bases de données Exchange 2013, votre environnement doit inclure les éléments suivants :
  
- Une version de Windows Server à partir de Windows Server 2008 
    
- Exchange 2013
    
En outre, si vous créez une sauvegarde et restaurez d’application, vous devez connaître les restrictions suivantes concernant l’environnement de développement :
  
- VSS est une API COM non managé qui est accessible à partir de code managé .NET Framework par le biais d’un Assembly d’interopérabilité COM.
    
- Exchange Management Shell est une application gérée qui est accessible via le code managé .NET Framework.
    
- L’API CHKSGFILES qui est fourni avec Exchange 2013 est une DLL de 64 bits de code natif. Utilisation de la DLL de CHKSGFILES Exchange 2007 32 bits avec des bases de données Exchange 2013 n’est pas prise en charge.
    
## <a name="backup-and-restore-application-overview"></a>Vue d’ensemble des applications de la sauvegarde et restauration
<a name="bk_components"> </a>

VSS coordonne la communication entre les composants suivants : 
  
- Le demandeur VSS, qui correspond à votre application de sauvegarde
    
- Le rédacteur VSS
    
- Le fournisseur VSS, c'est-à-dire les composants système, logiciel ou matériel qui créent les clichés instantanés
    
Pour utiliser VSS pour sauvegarder les données Exchange 2013, votre application de sauvegarde doit être un demandeur VSS Exchange 2013 prenant en charge. Exchange 2013 inclut un rédacteur VSS, appelé l’auteur du message Microsoft Exchange, pour le programme de sauvegarde Windows Server ; Toutefois, l’auteur du message change uniquement la sauvegarde des volumes entiers. Il ne sauvegarde pas individuels Exchange 2013 bases de données. Si vous avez besoin d’une plus grande flexibilité, vous pouvez utiliser une application de sauvegarde tierce ayant un rédacteur prenant en charge Exchange fonctionnant avec des bases de données Exchange, ou vous pouvez créer un demandeur VSS personnalisé.
  
Avant que votre application appelle VSS pour lancer une sauvegarde, il doit obtenir des informations sur la configuration du stockage pour le système de Exchange 2013 il sauvegarde. Ces informations sont stockées dans les Services de domaine Active Directory (AD DS). Votre application de sauvegarde peut obtenir des données de configuration du stockage Exchange à l’aide des commandes d’Exchange Management Shell. Pour plus d’informations, voir [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
Des applications de sauvegarde Exchange 2013 appellent l’API COM VSS pour créer complète, copie, les sauvegardes différentielles ou incrémentielles de bases de données Exchange ; ils n’ont pas d’interaction directement avec l’enregistreur VSS. La fonctionnalité de groupe de disponibilité de base de données (DAG) dans Exchange permet également à votre application créer une sauvegarde totalement cohérente, même si la sauvegarde complète initiale et version ultérieure des sauvegardes incrémentielles provenant de différents serveurs dans le DAG. Une fois que le service VSS crée la copie des données Exchange, votre application de sauvegarde stocke les données sur le support de destination.
  
Pour restaurer une base de données Exchange 2013, votre application de restauration extrait les fichiers journaux et de base de données à partir du support de sauvegarde et les stocke sur le stockage sur disque active d’un serveur Exchange. Des bases de données ne sont pas associés à un serveur Exchange spécifique. 
  
Applications de sauvegarde et de restauration doivent spécifier un nombre de paramètres spécifiques à Exchange 2013 de contrôler et de gérer les opérations exécutées par VSS sur les bases de données Exchange 2013 correctement. Par exemple, étant donné que Exchange 2013 prend en charge les bases de données actives simultanément jusqu'à 100, l’application de sauvegarde doit correctement spécifier et traiter le fichier de base de données, fichiers journaux de transactions et composants de base de données de fichier de point de contrôle.
  
Pour reconstruire une base de données dont les modifications apportées depuis la dernière sauvegarde complète, votre application de restauration nécessite des fichiers journaux et de base de données à partir de sauvegardes différents. Par exemple, il peut nécessiter une sauvegarde complète hebdomadaire et un ou plusieurs des sauvegardes incrémentielles quotidiennes. Dans Exchange 2013 systèmes qui utilisent des DAG, votre application de restauration permettre une reconstruction à l’aide de sauvegardes de copies de base de données différente sur différents serveurs dans le même DAG. Toutefois, la seule façon de restaurer une base de données DAG à partir de la sauvegarde est pour restaurer toutes les copies actives et passives de base de données à l’aide des mêmes données.
  
Une fois toutes les données en place, votre application de restauration signale Exchange pour vérifier l’intégrité des base de données et les fichiers journaux. Si les base de données et les fichiers journaux ont été restaurés correctement, le serveur Exchange peut puis relire les fichiers journaux de base de données pour mettre à jour la base de données et le monter. Si la base de données a été restaurée sur un serveur qui possède déjà une copie active de la base de données montée, la base de données est traitée comme une base de données de récupération. Si la base de données a été restaurée sur un autre serveur, la base de données peut être indépendamment montée ou que le réplica peut ensuite être ajouté dans le DAG.
  
## <a name="backup-and-restore-system-architecture"></a>Architecture du système de sauvegarde et de restauration
<a name="bk_ExchangeVSS"> </a>

Service VSS communique avec le système de fichiers Windows Server et le pilote de périphérique de stockage de masse via un fournisseur tiers (ou personnalisé). Le fournisseur de matériel détermine où le cliché instantané sera créé. VSS extrait le cliché instantané spécifiques au matériel afin que votre application de sauvegarde et de restauration peut accéder le cliché instantané sans informations sur les détails d’implémentation de matériel. La figure suivante illustre l’interaction de votre application de sauvegarde et de restauration avec Exchange 2013 et Windows Server.
  
**La figure 1. Architecture du système de sauvegarde et de restauration**

![Diagramme présentant les interactions entre une application de sauvegarde et de restauration. La communication à double sens existe entre Exchange, Windows Server et l’application cliente. Le serveur Windows interagit également avec un dispositif de stockage de masse ou un média de sauvegarde.](media/VSS_architecture_E2k7.gif)
  
L’application de sauvegarde et de restauration fonctionne comme le demandeur VSS. Le demandeur communique avec le service VSS visant à obtenir des informations sur Exchange 2013, pour initier la création de clichés instantanés et d’accéder aux données de sauvegarde. 
  
La banque d’informations Exchange est un composant d’Exchange 2013 et accède aux bases de données Exchange 2013 par le biais du système de fichiers Windows Server. Dans le système de fichiers, chaque serveur Exchange peut monter simultanément jusqu'à 100 bases de données avec un fichier de point de contrôle, fichiers journaux de transactions et leurs fichiers de base de données (.edb) correspondante.
  
Pour prendre en charge VSS, Exchange 2013 inclut un writer Exchange qui est intégré à la banque d’informations Exchange. Coordonnées de l’enregistreur Exchange avec la banque d’informations Exchange (en fonctionnement au nom du demandeur) Figer et démonter la base de données avant la sauvegarde, puis pour libérer et montez la base de données après la sauvegarde est terminée. Lors d’une restauration, votre application de sauvegarde et de restauration indique à l’auteur du message change pour coordonner avec la banque d’informations Exchange pour démonter la base de données, de remplacer les fichiers de base de données, montez la base de données et puis de relecture des journaux des transactions (si nécessaire).
  
Lors d’une restauration, le demandeur communique également avec le service VSS visant à préparer le système pour la restauration, puis pour mettre les données de sauvegarde sur le périphérique de stockage de masse. Votre application de sauvegarde et de restauration est également responsable de l’utilisation de Windows Server pour lire et écrire des données sur le support de stockage de sauvegarde, archiver ou non d’une bande, un réseau SAN ou autre support de sauvegarde.
  
La base de données restaurée peut être monté une base de données active régulière, soit comme la base de données de récupération Exchange 2013. Qu’une seule base de données montée peut être désigné comme une base de données de récupération sur chaque serveur Exchange.
  
Informations requises pour effectuer la sauvegarde et restauration entre Exchange 2013, VSS, et votre application de sauvegarde et de restauration est transférée dans le cadre des métadonnées enregistreur Exchange.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Types d’opérations de sauvegarde pour Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Restauration des bases de données Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Valider l’intégrité des sauvegardes en utilisant l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Valider l’intégrité des sauvegardes à l’aide l’outil Eseutil dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Sauvegarde et restauration pour Exchange](backup-and-restore-for-exchange-2013.md) 
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md) 
- [Service de cliché instantané de volume](http://msdn.microsoft.com/en-us/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

