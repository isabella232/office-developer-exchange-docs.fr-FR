---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: L’élément NonIndexableItemDetailsResult spécifie les résultats de l’opération WSDL GetNonIndexableItemDetails.
ms.openlocfilehash: 6e271f2cf0e37f26b945332c94167b6a42354115
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828535"
---
# <a name="nonindexableitemdetailsresult"></a>NonIndexableItemDetailsResult

L’élément **NonIndexableItemDetailsResult** spécifie les résultats de l’opération WSDL **GetNonIndexableItemDetails** . 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 **NonIndexableItemDetailResultType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Éléments (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

