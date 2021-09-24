---
title: FilterHtmlContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: L’élément FilterHtmlContent spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’un élément ou d’une pièce jointe.
ms.openlocfilehash: 9400c86465db994251a00164517590268e7e4ad1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510084"
---
# <a name="filterhtmlcontent"></a>FilterHtmlContent

**L’élément FilterHtmlContent** spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’un élément ou d’une pièce jointe. 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | Identifie les propriétés supplémentaires à renvoyer en réponse à une [demande GetAttachment.](getattachment.md)  <br/><br/>  Voici l’expression XPath de cet élément : <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés et le contenu de l’élément à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.  <br/> <br/> Les expressions XPath de cet élément sont les suivantes : <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Cet élément peut être **vrai** ou **faux**. La valeur par défaut est **false**. Il s’agit d’un type de données booléen.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle serveur d’accès au client installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

