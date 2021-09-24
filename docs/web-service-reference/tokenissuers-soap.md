---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Les éléments TokenIssuers représentent la collection TokenIssuer (SOAP).
ms.openlocfilehash: 68ff3ed515b346a84734596fae6fe127768b4476
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520401"
---
# <a name="tokenissuers-soap"></a>TokenIssuers (SOAP)

Les **éléments TokenIssuers** représentent la collection [TokenIssuer (SOAP).](tokenissuer-soap.md) 
  
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
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Spécifie [l’URI (SOAP)](uri-soap.md) et [le point de terminaison (SOAP)](endpoint-soap.md) pour le service de jeton de sécurité.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contient la [réponse SOAP (GetFederationInformation](getfederationinformation-operation-soap.md) operation).  <br/> |
   
## <a name="remarks"></a>Remarques

**TokenIssuers** représente une collection d’éléments [TokenIssuer (SOAP)](tokenissuer-soap.md) à utiliser dans la découverte automatique. 
  
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

