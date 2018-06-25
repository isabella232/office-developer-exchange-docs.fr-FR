---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: L’élément TokenIssuer Spécifie l’Uri (SOAP) et le point de terminaison (SOAP) pour le service d’émission de jeton de sécurité.
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838732"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

L’élément **TokenIssuer** Spécifie [l’Uri (SOAP)](uri-soap.md) et le [Point de terminaison (SOAP)](endpoint-soap.md) pour le service d’émission de jeton de sécurité. 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **TokenIssuer**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[URI (SOAP)](uri-soap.md) <br/> |URI du service de jeton de sécurité qui a émis le jeton de sécurité.  <br/> |
|[Point de terminaison (SOAP)](endpoint-soap.md) <br/> |L’URI du point de terminaison du service web.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Représente une collection de service d’émission de jeton de sécurité [Uri (SOAP)](uri-soap.md) et le [Point de terminaison (SOAP)](endpoint-soap.md).  <br/> |
   
## <a name="remarks"></a>Remarques

Utilisez l’élément **TokenIssuer** pour spécifier le service d’émission de jeton de sécurité lors de l’utilisation de jetons de sécurité. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Éléments du fichier XML Autodiscover SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

