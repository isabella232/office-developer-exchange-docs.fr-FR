---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: L’élément TokenIssuer spécifie l’URI (SOAP) et le point de terminaison (SOAP) pour le service d’émission de jeton de sécurité.
ms.openlocfilehash: e9c0b4140de26c7ff05daf4e863b3e8a17fedc62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526325"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

L’élément **TokenIssuer** spécifie l' [URI (SOAP)](uri-soap.md) et le [point de terminaison (SOAP)](endpoint-soap.md) pour le service d’émission de jeton de sécurité. 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **TokenIssuer**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[URI (SOAP)](uri-soap.md) <br/> |URI du service d’émission de jeton de sécurité qui a émis le jeton de sécurité.  <br/> |
|[Point de terminaison (SOAP)](endpoint-soap.md) <br/> |URI du point de terminaison du service Web.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Représente une collection de [protocole SOAP (](uri-soap.md) Security Token Service URI) et de [point de terminaison (SOAP)](endpoint-soap.md).  <br/> |
   
## <a name="remarks"></a>Remarques

Utilisez l’élément **TokenIssuer** pour spécifier le service d’émission de jeton de sécurité lors de l’utilisation de jetons de sécurité. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

