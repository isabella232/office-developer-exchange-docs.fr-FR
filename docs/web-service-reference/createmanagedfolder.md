---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: L’élément CreateManagedFolder définit une demande d’ajout de dossiers personnalisés gérés à une boîte aux lettres.
ms.openlocfilehash: 01fe8b7341c38ad33089c56271434ad3f9a4e5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458361"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

L’élément **CreateManagedFolder** définit une demande d’ajout de dossiers personnalisés gérés à une boîte aux lettres. 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **CreateManagedFolderRequestType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |Contient un tableau de dossiers gérés nommés à ajouter à une boîte aux lettres.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> |Identifie un objet de service d'annuaire à extension messagerie Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le compte de la personne qui effectue la demande doit disposer d’autorisations FullAccess sur la boîte aux lettres dans laquelle les dossiers gérés sont créés. Vous pouvez utiliser le paramètre _-AccessRights _ avec la cmdlet **Add-MailboxPermission** de l’environnement de commande Exchange Management Shell pour attribuer l’autorisation FullAccess. 
  
Bien que vous puissiez utiliser les services Web Exchange pour ajouter des dossiers gérés à une boîte aux lettres, vous ne pouvez pas utiliser les services Web Exchange pour accéder à la liste des dossiers gérés disponibles. Pour obtenir la liste des dossiers gérés disponibles, utilisez la cmdlet **Get-ManagedFolder** Exchange Management Shell. La liste renvoyée par la **cmdlet Get-ManagedFolder** contiendra des dossiers personnalisés gérés et des dossiers par défaut gérés. Vous pouvez uniquement ajouter des dossiers de type **ManagedCustomFolder** à la boîte aux lettres à l’aide de l’opération CreateManagedFolder. 
  
> [!NOTE]
> Vous pouvez également obtenir la liste des dossiers gérés à l’aide de l’API DirectoryServices de Microsoft .NET Framework. 
  
Vous pouvez utiliser l' [opération FindFolder](findfolder-operation.md) pour rechercher des dossiers gérés dans une boîte aux lettres. Les dossiers gérés peuvent être distingués en définissant l’élément [BaseShape](baseshape.md) sur AllProperties dans la demande. La réponse contient un élément [ManagedFolderInformation](managedfolderinformation.md) pour faire la distinction entre les dossiers gérés et les dossiers de la Banque d’Exchange. Vous pouvez supprimer des dossiers gérés de la même manière que vous supprimez d’autres types de dossier. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateManagedFolder](createmanagedfolder-operation.md)
  
[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

