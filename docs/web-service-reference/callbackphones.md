---
title: CallbackPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8a7c1377-aac3-42c5-820f-d01cd8e9cf5c
description: L’élément CallbackPhones spécifie un tableau de numéros de téléphone de rappel et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 99a3cec041886a40d4f25fc1c0d272111aae7331
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514752"
---
# <a name="callbackphones"></a>CallbackPhones

**L’élément CallbackPhones** spécifie un tableau de numéros de téléphone de rappel et les identificateurs de leurs attributions source pour le personnage associé. 
  
```XML
<CallbackPhones>
    <Value></Value>
    <Attributions></Attributions>
</CallbackPhones>
```

 **ArrayOfPhoneNumberAttributedValuesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Value (PersonaPhoneNumberType)](value-personaphonenumbertype.md) <br/> |Spécifie un numéro de téléphone et des informations de type et est associé à un ensemble d’attributions.  <br/> |
|[Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md) <br/> |Spécifie un tableau d’attributions pour son élément **Value** associé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Persona](persona.md) <br/> |Spécifie un ensemble de données de personnage renvoyées par une **demande GetPersona.**  <br/> |
   
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

