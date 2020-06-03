---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: L’élément GroupingInformation contient une valeur qui est utilisée pour regrouper la boîte aux lettres de l’utilisateur afin de préserver l’affinité lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres.
ms.openlocfilehash: 7cab5d68f7dd5ec1f6caded5b9da6cfee03f3a67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530077"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

L’élément **GroupingInformation** contient une valeur qui est utilisée pour regrouper la boîte aux lettres de l’utilisateur afin de [préserver l’affinité](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client au serveur Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est comparée à la valeur de l’élément **GroupingInformation** pour d’autres boîtes aux lettres. Les boîtes aux lettres qui ont la même valeur et utilisent le même point de terminaison des services Web Exchange (EWS) peuvent être regroupées pour maintenir l’affinité. Pour plus d’informations, consultez [la rubrique maintenir l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).
  
## <a name="remarks"></a>Remarques

L’élément **GroupingInformation** s’applique uniquement aux éléments de **protocole** qui ont un élément enfant [type (POX)](type-pox.md) avec la valeur « Expr ». 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

