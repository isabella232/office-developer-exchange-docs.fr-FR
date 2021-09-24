---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: L’élément IsInline représente si la pièce jointe apparaît en ligne dans un élément.
ms.openlocfilehash: 0bf51c981f3c9d2a4e38939d349fe662a57b29ac
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518273"
---
# <a name="isinline"></a>IsInline

**L’élément IsInline** représente si la pièce jointe apparaît en ligne dans un élément. 
  
```xml
<IsInline>true or false</IsInline>
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
|[FileAttachment](fileattachment.md) <br/> |Représente un fichier joint à un élément dans la Exchange store.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Cet élément peut être **vrai** ou **faux**. La valeur par défaut est **false**.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

