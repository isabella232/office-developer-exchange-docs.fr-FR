---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: L’élément GroupingInformation contient une valeur qui est utilisée pour la boîte aux lettres de l’utilisateur pour maintenir l’affinité lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres de groupe.
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827781"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

L’élément **GroupingInformation** contient une valeur qui est utilisée pour regrouper les boîtes aux lettres de l’utilisateur à [mettre à jour l’affinité](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[Protocole (POX)](protocol-pox.md)
  
[GroupingInformation (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour la connexion d’un client sur le serveur Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte est comparée à la valeur de l’élément **GroupingInformation** pour d’autres boîtes aux lettres. Boîtes aux lettres qui ont la même valeur et utilisent le même point de terminaison Exchange Web Services (EWS) peuvent être regroupés pour maintenir l’affinité. Pour plus d’informations, voir [mettre à jour l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).
  
## <a name="remarks"></a>Remarques

L’élément **GroupingInformation** est uniquement applicable à des éléments de **protocole** qui ont un élément enfant de [Type (POX)](type-pox.md) avec la valeur « EXPR ». 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Conserve les affinités entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

