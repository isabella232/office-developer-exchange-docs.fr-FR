---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Les éléments TokenIssuers représentent la collection de TokenIssuer (SOAP).
ms.openlocfilehash: 352487ad3fd9c1ee7de756a109fb98a49d0cdcd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457073"
---
# <a name="tokenissuers-soap"></a>TokenIssuers (SOAP)

Les éléments **TokenIssuers** représentent la collection de [TokenIssuer (SOAP)](tokenissuer-soap.md) . 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 **TokenIssuers**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Spécifie l' [URI (SOAP)](uri-soap.md) et le [point de terminaison (SOAP)](endpoint-soap.md) pour le service d’émission de jeton de sécurité.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contient la réponse [SOAP (GetFederationInformation Operation)](getfederationinformation-operation-soap.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Le **TokenIssuers** représente une collection d’éléments [TokenIssuer (SOAP)](tokenissuer-soap.md) à utiliser dans le service de découverte automatique. 
  
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

