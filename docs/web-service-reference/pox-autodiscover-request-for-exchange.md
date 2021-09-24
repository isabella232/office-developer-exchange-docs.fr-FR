---
title: Demande de découverte automatique POX pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: La demande de découverte automatique contient une requête pour la configuration de l’accès au client d’un utilisateur.
ms.openlocfilehash: 8a0960dcff21276baf723512befacc4eca35950f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523865"
---
# <a name="pox-autodiscover-request-for-exchange"></a>Demande de découverte automatique POX pour Exchange

La demande de découverte automatique contient une requête pour la configuration de l’accès au client d’un utilisateur.
  
## <a name="autodiscover-request-example"></a>Exemple de demande de découverte automatique

### <a name="description"></a>Description

L’exemple XML suivant montre un corps de demande de découverte automatique.
  
### <a name="code"></a>Code

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a>En-têtes de requête

Les en-têtes HTTP suivants sont facultatifs lors de l’envoi de demandes de découverte automatique.
  
**Tableau 1. En-têtes de requête HTTP**

|**Header**|**Description**|
|:-----|:-----|
|X-MapiHttpCapability  <br/> |S’il est présent et qu’il est définie sur « 1 », indique que le client demande des informations qui peuvent être utilisées pour se connecter au serveur à l’aide du protocole MAPI/HTTP. Cet en-tête s’applique aux clients qui implémentent le protocole MAPI/HTTP.  <br/> |
|X-ClientCanHandle  <br/> |Cet en-tête contient une liste de fonctionnalités délimitées par des virgules que le client prend en charge. Les valeurs possibles sont spécifiées dans le tableau 2.  <br/> |
   
**Tableau 2. Valeurs d’en-tête X-ClientCanHandle**

|**Valeur X-ClientCanHandle (ne sensible à la cas)**|**Version minimale du serveur**|**Description**|
|:-----|:-----|:-----|
|Négocier  <br/> |15.00.0995.014  <br/> |Si cette valeur est présente, le serveur retourne la valeur « Negotiate » dans l’élément [AuthPackage (POX)](authpackage-pox.md) si le serveur est configuré pour accepter l’authentification Negotiate. Si cette valeur n’est pas présente, le serveur ne retourne pas la valeur « Negotiate » dans **l’élément AuthPackage.**  <br/> |
|ExHttpInfo  <br/> |15.00.0995.014  <br/> |Si cette valeur est présente, le serveur retourne un élément de protocole [(POX)](protocol-pox.md) avec un élément [Type (POX)](type-pox.md) configuré sur « EXHTTP » si le serveur est configuré pour accepter les connexions RPC/HTTP. Si cette valeur n’est pas présente, le serveur ne retourne pas d’élément **Protocol** dont l’élément **Type** a la valeur « EXHTTP ».  <br/> |
   
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans le corps de la requête :
  
- [AutoDiscover (POX)](autodiscover-pox.md)
    
- [Request (POX)](request-pox.md)
    
- [AcceptableResponseSchema (POX)](acceptableresponseschema-pox.md)
    
- [EMailAddress (POX)](emailaddress-pox.md)
    
> [!NOTE]
> [L’élément LegacyDN (POX)](legacydn-pox.md) peut être utilisé à la place de l’élément [EMailAddress (POX).](emailaddress-pox.md) 
  
### <a name="version-differences"></a>Différences entre les versions

L’en-tête X-MapiHttpCapability est disponible dans les versions Office 365, Exchange Online et sur site de Exchange à partir de la build 15.00.0847.032 (Exchange Server 2013 SP1).
  
L’en-tête X-ClientCanHandle est disponible dans les versions Office 365, Exchange Online et sur site de Exchange à partir de la build 15.00.0995.014.
  
## <a name="see-also"></a>Voir aussi



[Réponse de découverte automatique POX pour Exchange](pox-autodiscover-response-for-exchange.md)


[Référence du service web de découverte automatique POX pour Exchange](pox-autodiscover-web-service-reference-for-exchange.md)
  
[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

