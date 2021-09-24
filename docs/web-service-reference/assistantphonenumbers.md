---
title: AssistantPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f9bd9ac1-7db3-44ea-9117-18488dddde15
description: L’élément AssistantPhoneNumbers spécifie un tableau de numéros de téléphone d’assistant et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 5653cb5ec10aeac20d43a65116af9dabebfc15e3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540222"
---
# <a name="assistantphonenumbers"></a>AssistantPhoneNumbers

**L’élément AssistantPhoneNumbers** spécifie un tableau de numéros de téléphone d’assistant et les identificateurs de leurs attributions source pour le personnage associé. 
  
```XML
<AssistantPhoneNumbers>
    <PhoneNumberAttributedValue></PhoneNumberAttributedValue>
</AssistantPhoneNumbers>
```

 **ArrayOfPhoneNumberAttributedValuesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |Spécifie une instance d’un tableau de numéros de téléphone et leurs attributions associées.  <br/> |
   
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

