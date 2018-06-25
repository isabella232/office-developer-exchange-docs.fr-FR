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
description: L’élément CreateManagedFolder définit une requête pour ajouter des dossiers personnalisés gérés à une boîte aux lettres.
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755734"
---
# <a name="createmanagedfolder"></a>CreateManagedFolder

L’élément **CreateManagedFolder** définit une requête pour ajouter des dossiers personnalisés gérés à une boîte aux lettres. 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 **CreateManagedFolderRequestType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Noms de dossier](foldernames.md) <br/> |Contient un tableau des dossiers gérés nommées à ajouter à une boîte aux lettres.  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> |Identifie un objet de service d'annuaire à extension messagerie Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le compte de la personne qui effectue la demande doit posséder les autorisations de FullAccess sur la boîte aux lettres dans lequel les dossiers gérés sont créés. Vous pouvez utiliser le paramètre de _ _ - AccessRights avec l’applet de commande Exchange Management Shell **Add-MailboxPermission** pour attribuer l’autorisation FullAccess. 
  
Bien que vous pouvez utiliser les Services Web Exchange pour ajouter des dossiers gérés pour une boîte aux lettres, vous ne pouvez pas utiliser les Services Web Exchange pour accéder à la liste des dossiers gérés qui sont disponibles. Pour obtenir une liste des dossiers gérés disponibles, utilisez l’applet de commande **get-managedfolder** Exchange Management Shell. La liste qui est renvoyée par la **cmdlet get-managedfolder** contiendra des dossiers personnalisés gérés et dossiers gérés par défaut. Vous pouvez uniquement ajouter des dossiers de type **managedcustomfolder** la boîte aux lettres à l’aide de l’opération CreateManagedFolder. 
  
> [!NOTE]
> Vous pouvez également obtenir une liste des dossiers gérés à l’aide de l’API DirectoryServices de Microsoft .NET Framework. 
  
Vous pouvez utiliser l' [opération FindFolder](findfolder-operation.md) pour rechercher les dossiers gérés dans une boîte aux lettres. Dossiers gérés peuvent être distingués en définissant l’élément [BaseShape](baseshape.md) AllProperties dans la demande. La réponse contient un élément [ManagedFolderInformation](managedfolderinformation.md) pour distinguer les dossiers gérés dans les dossiers de la banque Exchange. Vous pouvez supprimer des dossiers gérés de la même manière que vous supprimez d’autres types de dossier. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération CreateManagedFolder](createmanagedfolder-operation.md)
  
[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

