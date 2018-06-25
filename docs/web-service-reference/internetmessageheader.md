---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: L’élément InternetMessageHeader représente l’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes. Pour obtenir l’ensemble des en-têtes de message Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur les en-têtes de message Internet et EWS, en-têtes de message Internet seeGetting dans EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827952"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

L’élément **InternetMessageHeader** représente l’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes. Pour obtenir l’ensemble des en-têtes de message Internet, utilisez la propriété **PR_TRANSPORT_MESSAGE_HEADERS** . Pour plus d’informations à propos des en-têtes de message Internet et EWS, voir « en-têtes de message Internet mise en route dans [EWS, MIME et les en-têtes de message Internet manquants](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**HeaderName** <br/> |Identifie le nom d’en-tête.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente la valeur de l’en-tête.
  
## <a name="remarks"></a>Remarques

Vous trouverez ci-dessous l’API managée EWS étendu de définition de la propriété pour la propriété **PR_TRANSPORT_MESSAGE_HEADERS** . 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[EWS, MIME et les en-têtes de message Internet manquants](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

