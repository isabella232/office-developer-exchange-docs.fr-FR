---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: L’élément IsInline représente si la pièce jointe apparaît en ligne au sein d’un élément.
ms.openlocfilehash: f2f9093777a3914de067ef63827de6cf354fc12d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828042"
---
# <a name="isinline"></a>IsInline

L’élément **IsInline** représente si la pièce jointe apparaît en ligne au sein d’un élément. 
  
```xml
<IsInline>true or false</IsInline>
```

 **boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FileAttachment](fileattachment.md) <br/> |Représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Cet élément peut être **true** ou **false**. La valeur par défaut est **false**.
  
## <a name="remarks"></a>Note

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

