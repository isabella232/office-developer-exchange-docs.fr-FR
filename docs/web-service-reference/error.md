---
title: Erreur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: L’élément Error représente une erreur de validation unique sur une valeur de propriété de règle particulière, une valeur de propriété de prédicat ou une valeur de propriété d’action.
ms.openlocfilehash: aeeda25ccc3e657e99bd6f2fea12322fdd3e720d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530860"
---
# <a name="error"></a>Erreur

**L’élément Error** représente une erreur de validation unique sur une valeur de propriété de règle particulière, une valeur de propriété de prédicat ou une valeur de propriété d’action. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldUri (Rule)](fielduri-rule.md) <br/> |Spécifie l’URI du champ de règle à l’origine de l’erreur de validation.  <br/> |
|[ErrorCode](errorcode.md) <br/> |Représente un code d’erreur de validation de règle qui décrit les erreurs de validation pour chaque prédicat ou action de règle.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Représente la raison de l’erreur de validation.  <br/> |
|[FieldValue](fieldvalue.md) <br/> |Représente la valeur du champ à l’origine de l’erreur de validation.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |Représente un tableau d’erreurs de validation de règle sur chaque champ de règle qui a une erreur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

