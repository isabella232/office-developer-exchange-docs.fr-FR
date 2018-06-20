---
title: Élément (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: L’élément représente un seul élément à télécharger dans une boîte aux lettres.
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828138"
---
# <a name="item-uploaditemtype"></a>Élément (UploadItemType)

**L’élément** représente un seul élément à télécharger dans une boîte aux lettres. 
  
[UploadItems](uploaditems.md)
  
[Éléments (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
[Élément (UploadItemType)](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 **UploadItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**CreateAction** <br/> |Spécifie l’action de téléchargement d’un élément dans une boîte aux lettres. Cet attribut est requis.  <br/> |
|**IsAssociated** <br/> |Indique si l’élément téléchargé est un élément de dossier associé. Cet attribut est une valeur de type Boolean. La valeur **true** indique que l’élément est un dossier associé item. Cet attribut est facultatif.  <br/> |
   
#### <a name="createaction-attribute"></a>Attribut CreateAction

|**Valeur**|**Description**|
|:-----|:-----|
|**CreateNew** <br/> |Indique qu’une nouvelle copie de l’élément d’origine est téléchargée vers la boîte aux lettres. L’élément [ItemId](itemid.md) ne doit pas être présent si la valeur CreateNew est utilisée. L’identificateur d’élément est retournée dans la réponse.  <br/> |
|**Mettre à jour** <br/> |Spécifie que l’élément indiqué par l’élément **ItemId** est mis à jour. Une erreur est renvoyée si l’élément **ItemId** n’est pas présent ou si l’élément n’existe pas dans le dossier identifié par l’élément [ParentFolderId](parentfolderid.md) .  <br/> |
|**UpdateOrCreate** <br/> |Indique qu’une tentative est tout d’abord à mettre à jour l’élément. Si l’élément n’existe pas dans le dossier spécifié par l’élément **ParentFolderId** , un nouvel élément est créé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier parent où un nouvel élément est créé ou qui contient l’élément à mettre à jour.  <br/> |
|[ID d’élément](itemid.md) <br/> |Contient la clé unique identificateur et modification d’un élément pour créer ou mettre à jour dans la banque d’informations Exchange.  <br/> |
|[Données (base64Binary)](data-base64binary.md) <br/> |Contient les données d’un seul élément à télécharger dans une boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Éléments (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |Contient un tableau d’éléments à télécharger dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ExportItems](exportitems-operation.md)
  
[Opération UploadItems](uploaditems-operation.md)

