---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: L’élément FieldURIOrConstant représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété.
ms.openlocfilehash: bc7edb4542c68e02e9661ff0a4c7066362a04081
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535240"
---
# <a name="fielduriorconstant"></a>FieldURIOrConstant

**L’élément FieldURIOrConstant** représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété. 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
    <IndexedFieldURI/> 
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <FieldURI/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <ExtendedFieldURI/> 
</FieldURIOrConstant>
```

**FieldURIOrConstantType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Constante](constant.md) <br/> |Identifie une valeur constante dans une restriction.  <br/> |
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencés par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[IsEqualTo](isequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et qui est évaluée à true si elles sont égales.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie true si la première propriété est supérieure.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie true si la première propriété est supérieure ou égale à la deuxième valeur ou propriété.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si la première propriété est inférieure à la deuxième valeur ou propriété.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si la première propriété est inférieure ou égale à la deuxième valeur ou propriété.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie true si les valeurs ne sont pas identiques.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple XML suivant montre l’élément FieldURIOrConstant utilisé avec une constante et un URI de champ.
  
```xml
<Restriction>
  <Or xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

