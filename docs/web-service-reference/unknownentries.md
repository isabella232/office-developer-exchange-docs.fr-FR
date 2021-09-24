---
title: UnknownEntries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: L’élément UnknownEntries contient un tableau d’entrées d’autorisation inconnues qui ne peuvent pas être résolues par rapport au service d’annuaire Active Directory. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 9ada724abbecddf192b5f345c1800ac38a8b41aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514080"
---
# <a name="unknownentries"></a>UnknownEntries

**L’élément UnknownEntries** contient un tableau d’entrées d’autorisation inconnues qui ne peuvent pas être résolues par rapport au service d’annuaire Active Directory. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 **ArrayOfUnknownEntriesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UnknownEntry](unknownentry.md) <br/> |Représente une seule entrée d’autorisation inconnue qui ne peut pas être résolue par rapport à Active Directory. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Contient toutes les autorisations configurées pour un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[PermissionSet (CalendarPermissionSetType)](permissionset-calendarpermissionsettype.md) <br/> |Contient toutes les autorisations configurées pour un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Remarques

Vous pouvez supprimer des entrées inconnues d’un dossier à l’aide de l’opération UpdateFolder avec [l’élément SetFolderField.](setfolderfield.md) Les entrées inconnues sont supprimées lorsque vous réinitialisez PermissionSet à l’aide de l’option SetFolderField de l’opération UpdateFolder. Exchange Les services Web ne prend pas en charge la suppression d’entrées individuelles. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération UpdateFolder](updatefolder-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

