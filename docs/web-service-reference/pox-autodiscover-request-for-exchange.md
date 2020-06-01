---
title: Demande de découverte automatique POX pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: La demande de découverte automatique contient une requête pour la configuration d’accès client d’un utilisateur.
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461666"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Demande de découverte automatique POX pour Exchange

La demande de découverte automatique contient une requête pour la configuration d’accès client d’un utilisateur.
  
## <a name="autodiscover-request-example"></a>Exemple de requête de découverte automatique

### <a name="description"></a>Description

L’exemple de code XML suivant montre un corps de demande de découverte automatique.
  
### <a name="code"></a>Code

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>En-têtes de demande

Les en-têtes HTTP suivants sont facultatifs lors de l’envoi de demandes de découverte automatique.
  
**Tableau 1. En-têtes de requête HTTP**

|**Header**|**Description**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |Si présent et défini sur « 1 », indique que le client demande des informations qui peuvent être utilisées pour se connecter au serveur à l’aide du protocole MAPI/HTTP. Cet en-tête s’applique aux clients qui implémentent le protocole MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |Cet en-tête contient une liste délimitée par des virgules des fonctionnalités prises en charge par le client. Les valeurs possibles sont spécifiées dans le tableau 2.  <br/> |
   
**Tableau 2. Valeurs d’en-tête X-ClientCanHandle**

|**Valeur X-ClientCanHandle (ne respectant pas la casse)**|**Version de serveur minimale**|**Description**|
|:-----|:-----|:-----|
|Poursuivre  <br/> |15.00.0995.014  <br/> |Si cette valeur est présente, le serveur renvoie la valeur « Negotiate » dans l’élément [package (POX)](authpackage-pox.md) si le serveur est configuré pour accepter l’authentification par négociation. Si cette valeur n’est pas présente, le serveur ne renvoie pas la valeur « Negotiate » dans l’élément **package** .  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Si cette valeur est présente, le serveur renvoie un élément [Protocol (POX)](protocol-pox.md) avec un élément [type (POX)](type-pox.md) défini sur « exhttp » si le serveur est configuré pour accepter les connexions RPC/HTTP. Si cette valeur n’est pas présente, le serveur ne renvoie pas un élément de **protocole** dont l’élément **type** est défini sur « exhttp ».  <br/> |
   
### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans le corps de la demande :
  
- [Découverte automatique (POX)](autodiscover-pox.md)
    
- [Demande (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> L’élément [LegacyDN (POX)](legacydn-pox.md) peut être utilisé à la place de l’élément [EMailAddress (POX)](emailaddress-pox.md) . 
  
### <a name="version-differences"></a>Différences entre les versions

L’en-tête X-MapiHttpCapability est disponible dans Office 365, Exchange Online et les versions locales d’Exchange à partir de la version 15.00.0847.032 (Exchange Server 2013 SP1).
  
L’en-tête X-ClientCanHandle est disponible dans Office 365, Exchange Online et les versions locales d’Exchange à partir de la version 15.00.0995.014.
  
## <a name="see-also"></a>Voir aussi



[Réponse de découverte automatique POX pour Exchange](pox-autodiscover-response-for-exchange.md)


[Référence du service Web de découverte automatique POX pour Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

