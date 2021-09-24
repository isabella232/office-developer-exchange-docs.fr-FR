---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: L’élément CalendarPermission définit l’accès dont dispose un utilisateur à un dossier Calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7794cab261653f8cb6421d4e0633d496ba347a5f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514801"
---
# <a name="calendarpermission"></a>CalendarPermission

**L’élément CalendarPermission** définit l’accès dont dispose un utilisateur à un dossier Calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **CalendarPermissionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarPermissionLevel](calendarpermissionlevel.md) <br/> |Représente le niveau d’autorisation d’un utilisateur sur un dossier Calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[CanCreateItems](cancreateitems.md) <br/> |Indique si un utilisateur est autorisé à créer des éléments dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Indique si un utilisateur est autorisé à supprimer des éléments dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[EditItems](edititems.md) <br/> |Indique si un utilisateur est autorisé à modifier des éléments dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Indique si un utilisateur est un contact pour un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Indique si un utilisateur est le propriétaire d’un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Indique si un utilisateur peut afficher un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ReadItems (CalendarPermissionType)](readitems-calendarpermissiontype.md) <br/> |Indique si un utilisateur est autorisé à lire des éléments dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[UserId](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur qui dispose d’autorisations d’accès aux dossiers. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Contient un tableau d’autorisations de calendrier pour un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
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

