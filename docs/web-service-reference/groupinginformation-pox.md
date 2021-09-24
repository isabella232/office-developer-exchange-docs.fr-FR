---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: L’élément GroupingInformation contient une valeur qui est utilisée pour grouper la boîte aux lettres de l’utilisateur afin de conserver l’affinité lors de l’abonnement aux notifications dans plusieurs boîtes aux lettres.
ms.openlocfilehash: 14e751adcd0b966907ce495a2753b2b26d812a86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525883"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

**L’élément GroupingInformation** contient une valeur qui est utilisée [](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) pour grouper la boîte aux lettres de l’utilisateur afin de conserver l’affinité lors de l’abonnement aux notifications dans plusieurs boîtes aux lettres. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[GroupingInformation (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client au Exchange serveur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est comparée à la valeur de l’élément **GroupingInformation** pour d’autres boîtes aux lettres. Les boîtes aux lettres qui ont la même valeur et utilisent le même point de terminaison Exchange Web Services (EWS) peuvent être regroupées pour conserver l’affinité. Pour plus d’informations, voir [Conserver l’affinité entre un groupe d’abonnements](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)et le serveur de boîtes aux lettres dans Exchange .
  
## <a name="remarks"></a>Remarques

**L’élément GroupingInformation** s’applique uniquement aux éléments **Protocol** qui ont un élément enfant [Type (POX)](type-pox.md) avec la valeur « EXPR ». 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

