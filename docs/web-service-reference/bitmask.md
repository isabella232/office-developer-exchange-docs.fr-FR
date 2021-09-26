---
title: Bitmask
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: L’élément Bitmask représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction Excludes.
ms.openlocfilehash: 83307fc7f5ba328c5d6f7574a8b3be1ea25595f3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543589"
---
# <a name="bitmask"></a>Bitmask

**L’élément Bitmask** représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction [Excludes.](excludes.md) 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Valeur** | Représente un masque de bits décimal ou hexadécimal. La valeur est représentée par l’expression régulière suivante :<br/>`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.<br/><br/>Voici des exemples de valeurs hexadécimales pour cet attribut :<br/>- 0x12AF<br/>- 0X334AE<br/><br/>Voici des exemples de valeurs décimales pour cet attribut :<br/>- 10<br/>- 255<br/>- 4562 |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Excludes](excludes.md) <br/> |Effectue un masque de propriétés au sens du bit.  <br/> |
   
## <a name="remarks"></a>Remarques

Les valeurs hexadécimales doivent avoir un préfixe de 0x ou 0X. Si ce préfixe n’existe pas, la valeur est supposée être un nombre décimal.
  
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

