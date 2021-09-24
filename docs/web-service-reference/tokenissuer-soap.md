---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: L’élément TokenIssuer spécifie l’URI (SOAP) et le point de terminaison (SOAP) pour le service de jeton de sécurité.
ms.openlocfilehash: ea1c93493e4f47a6f2551c24586e54614f4f45e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527264"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

**L’élément TokenIssuer** spécifie l’URI [(SOAP)](uri-soap.md) et le point de terminaison [(SOAP)](endpoint-soap.md) pour le service de jeton de sécurité. 
  
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
|[Uri (SOAP)](uri-soap.md) <br/> |URI du service d’émission de jeton de sécurité qui a émis le jeton de sécurité.  <br/> |
|[Point de terminaison (SOAP)](endpoint-soap.md) <br/> |URI du point de terminaison du service web.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Représente une collection d’URI de service d’uri de jeton de sécurité [(SOAP)](uri-soap.md) et [de point de terminaison (SOAP).](endpoint-soap.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Utilisez **l’élément TokenIssuer** pour spécifier le service de jeton de sécurité lors de l’utilisation de jetons de sécurité. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

