---
title: Demande de découverte automatique variole pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: La demande de découverte automatique contient une requête pour la configuration de l’accès client d’un utilisateur.
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828865"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Demande de découverte automatique variole pour Exchange

La demande de découverte automatique contient une requête pour la configuration de l’accès client d’un utilisateur.
  
## <a name="autodiscover-request-example"></a>Exemple de requête de découverte automatique

### <a name="description"></a>Description

L’exemple XML suivant montre un corps de demande de découverte automatique.
  
### <a name="code"></a>Code

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>En-têtes de demande

Les en-têtes HTTP suivants sont facultatifs lors de l’envoi de demandes de découverte automatique.
  
**Le tableau 1. En-têtes de demande HTTP**

|**Header**|**Description**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |Si présente et définie sur « 1 », indique que le client demande des informations qui peuvent être utilisées pour se connecter au serveur à l’aide du protocole MAPI/HTTP. Cet en-tête est applicable aux clients qui implémentent le protocole MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |Cet en-tête contient une liste délimitée par des fonctions prises en charge par le client. Les valeurs possibles sont spécifiés dans le tableau 2.  <br/> |
   
**Le tableau 2. Valeurs d’en-tête X-ClientCanHandle**

|**Valeur X-ClientCanHandle (pas la casse)**|**Version minimale du serveur**|**Description**|
|:-----|:-----|:-----|
|Négocier  <br/> |15.00.0995.014  <br/> |Si cette valeur est présente, le serveur renvoie une valeur « Negotiate » dans l’élément [AuthPackage (POX)](authpackage-pox.md) si le serveur est configuré pour accepter l’authentification par négociation. Si cette valeur n’est pas présente, le serveur ne sera pas renvoie une valeur de « Négocier » dans l’élément **AuthPackage** .  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Si cette valeur est présente, le serveur renvoie un élément de [Protocole (POX)](protocol-pox.md) avec un élément de [Type (POX)](type-pox.md) la valeur « EXHTTP » si le serveur est configuré pour accepter les connexions RPC/HTTP. Si cette valeur n’est pas présente, le serveur renvoie pas un élément de **protocole** avec un élément de **Type** défini sur « EXHTTP ».  <br/> |
   
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans le corps de la demande :
  
- [Découverte automatique (POX)](autodiscover-pox.md)
    
- [Demande (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> L’élément [LegacyDN (POX)](legacydn-pox.md) peut être utilisé à la place de l’élément [EMailAddress (POX)](emailaddress-pox.md) . 
  
### <a name="version-differences"></a>Différences entre les versions

L’en-tête X-MapiHttpCapability est disponible dans Office 365, Exchange Online et créer des versions d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1) sur site.
  
L’en-tête X-ClientCanHandle est disponible dans Office 365, Exchange Online et créer des versions d’Exchange commençant par 15.00.0995.014 local.
  
## <a name="see-also"></a>Voir aussi



[Réponse de découverte automatique variole pour Exchange](pox-autodiscover-response-for-exchange.md)


[Référence de service web variole découverte automatique pour Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

