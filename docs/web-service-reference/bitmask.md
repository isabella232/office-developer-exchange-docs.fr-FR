---
title: Composé
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: L’élément masque binaire représente un masque hexadécimal ou décimal à utiliser pendant une opération de restriction exclusions.
ms.openlocfilehash: f05be466d05b13f8f362afb5fc0552653a532475
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458809"
---
# <a name="bitmask"></a>Composé

L’élément **masque binaire** représente un masque hexadécimal ou décimal à utiliser pendant une opération de restriction [exclusions](excludes.md) . 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Valeur** | Représente un masque de réfixe décimal ou hexadécimal. La valeur est représentée par l’expression régulière suivante :<br/>`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.<br/><br/>Voici des exemples de valeurs hexadécimales pour cet attribut :<br/>- 0x12AF<br/>- 0X334AE<br/><br/>Voici des exemples de valeurs décimales pour cet attribut :<br/>-10<br/>-255<br/>-4562 |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Exclut](excludes.md) <br/> |Effectue un masque de bits des propriétés.  <br/> |
   
## <a name="remarks"></a>Remarques

Les valeurs hexadécimales doivent avoir un préfixe 0x ou 0X. Si ce préfixe n’existe pas, la valeur est supposée être un nombre décimal.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

