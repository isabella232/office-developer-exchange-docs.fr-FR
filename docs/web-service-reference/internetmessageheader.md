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
description: L’élément InternetMessageHeader représente l’en-tête de message Internet d’un en-tête donné dans la collection headers. Pour obtenir la collection entière des en-têtes de message Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur EWS et les en-têtes de message Internet, obtention les en-têtes de message Internet dans EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 7b662617e0b1a1fcdcce3449b729485ba6e0956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459306"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

L’élément **InternetMessageHeader** représente l’en-tête de message Internet d’un en-tête donné dans la collection headers. Pour obtenir la collection entière des en-têtes de message Internet, utilisez la propriété **PR_TRANSPORT_MESSAGE_HEADERS** . Pour plus d’informations sur EWS et les en-têtes de message Internet, consultez les rubriques «obtenir des en-têtes de message Internet dans [EWS, MIME et les en-têtes de messages Internet manquants](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**HeaderName** <br/> |Identifie le nom de l’en-tête.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente la valeur de l’en-tête.
  
## <a name="remarks"></a>Remarques

Voici la définition de la propriété étendue de l’API managée EWS pour la propriété **PR_TRANSPORT_MESSAGE_HEADERS** . 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[EWS, MIME et les en-têtes de message Internet manquants](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

