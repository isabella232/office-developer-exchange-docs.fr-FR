---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: L’élément EmailAddressAttributedValue spécifie une instance d’un tableau d’adresses de messagerie et leurs attributions associées.
ms.openlocfilehash: 2b5e9b431b6a62c63e815bfee190c923f454c867
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519764"
---
# <a name="emailaddressattributedvalue"></a>EmailAddressAttributedValue

**L’élément EmailAddressAttributedValue** spécifie une instance d’un tableau d’adresses de messagerie et leurs attributions associées. 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 **EmailAddressAttributedValueType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Value (EmailAddressType)](value-emailaddresstype.md) <br/> |Spécifie la valeur d’un **emailAddress** associé à un tableau d’attributions.  <br/> |
|[Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |Spécifie un tableau d’attributions pour son élément **Value** associé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Emails1](emails1.md) <br/> |Spécifie un tableau de valeurs de courrier électronique et les identificateurs de leurs attributions source pour le personnage associé.  <br/> |
|[Emails2](emails2.md) <br/> |Spécifie un tableau de valeurs de courrier électronique et les identificateurs de leurs attributions source pour le personnage associé.  <br/> |
|[Emails3](emails3.md) <br/> |Spécifie un tableau de valeurs de courrier électronique et les identificateurs de leurs attributions source pour le personnage associé.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

