---
title: Masque de bits
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
description: L’élément de masque de bits représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction des exclusions.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755401"
---
# <a name="bitmask"></a>Masque de bits

L’élément de **masque de bits** représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction des [exclusions](excludes.md) . 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Valeur** | Représente un masque de bits décimal ou hexadécimal. La valeur est représentée par l’expression régulière suivante :<br/>« ((0 x|0X)[0-9A-FA-f]*)|([0-9] *) ».<br/><br/>Voici des exemples de valeurs hexadécimales pour cet attribut :<br/>-0x12AF<br/>-0X334AE<br/><br/>Voici des exemples de valeurs décimales de cet attribut :<br/>-10<br/>-255<br/>-4562 |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Exclut](excludes.md) <br/> |Effectue un masque de bits des propriétés.  <br/> |
   
## <a name="remarks"></a>Remarques

Des valeurs hexadécimales doivent avoir un préfixe 0 x ou 0 X. Si ce préfixe n’existe pas, la valeur est supposée être un nombre décimal.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

