---
title: Erreur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: L’élément Error représente une seule erreur de validation sur une valeur de la propriété règle particulière, la valeur de propriété prédicat ou la valeur de la propriété action.
ms.openlocfilehash: adb2de56b7610aa92b5bf5b8d43ac22f35021b64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756205"
---
# <a name="error"></a>Erreur

L’élément **Error** représente une seule erreur de validation sur une valeur de la propriété règle particulière, la valeur de propriété prédicat ou la valeur de la propriété action. 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 **RuleValidationErrorType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldUri (règle)](fielduri-rule.md) <br/> |Spécifie l’URI pour le champ règle qui a provoqué l’erreur de validation.  <br/> |
|[Code d’erreur](errorcode.md) <br/> |Représente un code d’erreur de validation de règle qui décrit ce qui a échoué validation pour chaque action ou au prédicat de la règle.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Représente la raison de l’erreur de validation.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Représente la valeur du champ qui a provoqué l’erreur de validation.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |Représente un tableau règle des erreurs de validation sur chaque champ de règle qui comporte une erreur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

