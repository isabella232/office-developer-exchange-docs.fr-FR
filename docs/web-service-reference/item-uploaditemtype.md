---
title: Élément (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: L’élément item représente un élément unique à télécharger dans une boîte aux lettres.
ms.openlocfilehash: 82c0fdf89c06ddfb812c2b2f1899b589eedeb7d8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467549"
---
# <a name="item-uploaditemtype"></a>Élément (UploadItemType)

L’élément **Item** représente un élément unique à télécharger dans une boîte aux lettres. 
  
[UploadItems](uploaditems.md)
  
[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**CreateAction** <br/> |Spécifie l’action de téléchargement d’un élément dans une boîte aux lettres. Cet attribut est obligatoire.  <br/> |
|**IsAssociated** <br/> |Indique si l’élément téléchargé est un élément associé à un dossier. Cet attribut est une valeur booléenne. La valeur **true** indique que l’élément est un élément associé à un dossier. Cet attribut est facultatif.  <br/> |
   
#### <a name="createaction-attribute"></a>Attribut CreateAction

|**Valeur**|**Description**|
|:-----|:-----|
|**CreateNew** <br/> |Indique qu’une nouvelle copie de l’élément d’origine est téléchargée vers la boîte aux lettres. L’élément [ItemId](itemid.md) ne doit pas être présent si la valeur CreateNew est utilisée. Le nouvel identificateur d’élément est renvoyé dans la réponse.  <br/> |
|**Mettre à jour** <br/> |Spécifie que l’élément indiqué par l’élément **ItemId** sera mis à jour. Une erreur est renvoyée si l’élément **ItemId** n’est pas présent ou si l’élément n’existe pas dans le dossier identifié par l’élément [ParentFolderId](parentfolderid.md) .  <br/> |
|**UpdateOrCreate** <br/> |Indique qu’une tentative est d’abord effectuée pour mettre à jour l’élément. Si l’élément n’existe pas dans le dossier spécifié par l’élément **ParentFolderId** , un nouvel élément est créé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier parent dans lequel un nouvel élément est créé ou qui contient l’élément à mettre à jour.  <br/> |
|[ItemId](itemid.md) <br/> |Contient l’identificateur unique et la clé de modification d’un élément à créer ou mettre à jour dans la Banque d’Exchange.  <br/> |
|[Données (base64Binary)](data-base64binary.md) <br/> |Contient les données d’un élément unique à télécharger dans une boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Items (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md) <br/> |Contient un tableau d’éléments à charger dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ExportItems](exportitems-operation.md)
  
[Opération UploadItems](uploaditems-operation.md)

