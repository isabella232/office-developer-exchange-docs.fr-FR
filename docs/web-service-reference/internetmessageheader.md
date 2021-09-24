---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: L’élément InternetMessageHeader représente l’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes. Pour obtenir l’ensemble de la collection d’en-têtes de messages Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur les en-têtes de message Internet et EWS, voir En-têtes de message Internet EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 4b3072611e8a3debf87ce2a023f4f68ee4487185
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541082"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

**L’élément InternetMessageHeader** représente l’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes. Pour obtenir l’ensemble de la collection d’en-têtes de messages Internet, utilisez **la PR_TRANSPORT_MESSAGE_HEADERS** internet. Pour plus d’informations sur EWS et les en-têtes de message Internet, voir « Obtention d’en-têtes de message Internet dans [EWS, MIME](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)et les en-têtes de message Internet manquants .
  
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

Voici la définition de propriété étendue de l’API gérée EWS pour **PR_TRANSPORT_MESSAGE_HEADERS** propriété. 
  
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


[EWS, MIME et en-têtes de message Internet manquants](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

