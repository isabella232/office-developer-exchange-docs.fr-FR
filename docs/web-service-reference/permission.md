---
title: Autorisation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: L’élément Permission définit l’accès d’un utilisateur à un dossier.
ms.openlocfilehash: bc3e140aaf7bd9ea7f1a4993c9bea1dcad8d39fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512666"
---
# <a name="permission"></a>Autorisation

**L’élément Permission** définit l’accès d’un utilisateur à un dossier. 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **PermissionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CanCreateItems](cancreateitems.md) <br/> |Indique si un utilisateur est autorisé à créer des éléments dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Indique si un utilisateur est autorisé à supprimer des éléments dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[EditItems](edititems.md) <br/> |Indique si un utilisateur est autorisé à modifier des éléments dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Indique si un utilisateur est un contact pour un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Indique si un utilisateur est le propriétaire d’un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Indique si un utilisateur peut afficher un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[PermissionLevel](permissionlevel.md) <br/> |Représente la combinaison des autorisations dont dispose un utilisateur sur un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ReadItems (PermissionType)](readitems-permissiontype.md) <br/> |Indique si un utilisateur est autorisé à lire les éléments d’un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[UserId](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur qui dispose d’autorisations d’accès aux dossiers. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Autorisations](permissions.md) <br/> |Contient toutes les autorisations configurées pour un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Différences entre les versions

Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre de Office 365 ou une version sur site de Exchange à partir de Exchange 2013, les autorisations de dossier ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a la valeur **AllProperties** dans [GetFolder](getfolder-operation.md) demande d’opération. Pour récupérer les autorisations de dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément [AdditionalProperties](additionalproperties.md) dans la **demande GetFolder.** 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

