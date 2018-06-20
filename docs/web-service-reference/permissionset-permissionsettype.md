---
title: PermissionSet (PermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: L’élément PermissionSet contient toutes les autorisations qui sont configurées pour un dossier.
ms.openlocfilehash: 0fa0ac78a0db2bf382ad413cbb8bd072aa88c6fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828732"
---
# <a name="permissionset-permissionsettype"></a>PermissionSet (PermissionSetType)

L’élément **PermissionSet** contient toutes les autorisations qui sont configurées pour un dossier. 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **PermissionSetType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Autorisations](permissions.md) <br/> |Contient la collection des autorisations pour un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Contient un tableau d’entrées inconnus qui ne peut pas être résolu sur le service d’annuaire Active Directory. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Définit un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche qui se trouve dans une boîte aux lettres.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts qui se trouve dans une boîte aux lettres.  <br/> |
|[Dossier tâches](tasksfolder.md) <br/> |Représente un dossier de tâches qui se trouve dans une boîte aux lettres.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément a été introduit dans Exchange Server 2007 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Différences entre les versions

Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange 2013, les autorisations de dossier ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la requête d’opération [GetFolder](getfolder-operation.md) . Pour récupérer les autorisations du dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément de [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** . 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

