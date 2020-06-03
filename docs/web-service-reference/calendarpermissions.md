---
title: CalendarPermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissions
api_type:
- schema
ms.assetid: 9b659d83-45fb-42a2-b052-5bc4dbe3854d
description: L’élément CalendarPermissions contient un tableau d’autorisations de calendrier pour un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: f072339212d0fdff3983fbfb6bc8f53c272350c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529468"
---
# <a name="calendarpermissions"></a>CalendarPermissions

L’élément **CalendarPermissions** contient un tableau d’autorisations de calendrier pour un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<CalendarPermissions>
   <PermissionSet/>
</CalendarPermissions>
```

 **ArrayOfCalendarPermissionsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Définit l’accès d’un utilisateur délégué à un dossier de calendrier.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PermissionSet (CalendarPermissionSetType)](permissionset-calendarpermissionsettype.md) <br/> |Contient toutes les autorisations configurées pour un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
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

