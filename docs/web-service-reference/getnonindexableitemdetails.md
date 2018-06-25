---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: L’élément GetNonIndexableItemDetails spécifie une requête pour récupérer les détails de l’élément nonindexable.
ms.openlocfilehash: 0aeda85973aa78eff240a017db58ffb57fc0de06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756676"
---
# <a name="getnonindexableitemdetails"></a>GetNonIndexableItemDetails

L’élément **GetNonIndexableItemDetails** spécifie une requête pour récupérer les détails de l’élément nonindexable. 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 **GetNonIndexableItemDetailsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |Spécifie un tableau d’éléments de **boîte aux lettres** .  <br/> |
|[PageSize](pagesize.md) <br/> |Contient le nombre d’éléments à renvoyer dans une seule page pour un résultat de recherche.  <br/> |
|[PageItemReference](pageitemreference.md) <br/> |Spécifie la référence pour un élément de page.  <br/> |
|[PageDirection](pagedirection.md) <br/> |Indique la direction de la pagination dans le résultat de recherche.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

