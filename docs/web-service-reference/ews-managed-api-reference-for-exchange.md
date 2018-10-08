---
title: Référence d’API managée des services web Exchange (EWS)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6ca36f4-a67c-4e3c-aae7-9ead7b704e15
description: En savoir plus sur les espaces de noms qui sont inclus dans l’API managée EWS.
ms.openlocfilehash: 78797ba5124cb47da5430491d3be23bbaf0371a7
ms.sourcegitcommit: 25cbbc6707e4ec0621c5c46baf7fe49be42d3297
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/07/2018
ms.locfileid: "25440982"
---
# <a name="ews-managed-api-reference"></a>Référence d’API managée EWS

**S’applique à** : API managée EWS | Exchange Online | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 | Office 365

L’API managée des services web Exchange (EWS) inclut deux API : Microsoft.Exchange.WebServices.dll et Microsoft.Exchange.WebServices.Auth.dll.

## <a name="ews-managed-api-namespaces"></a>Espaces de noms d’API managée EWS

|Espace de noms |Description |
|:---------|:-----------|
|[Microsoft.Exchange.WebServices.Auth.Validation](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.auth.validation?view=exchange-ews-api) |Contient les types et les méthodes utilisés pour valider les jetons d’identité utilisateur envoyés à partir d’un serveur Exchange. L’espace de noms Microsoft.Exchange.WebServices.Auth.Validation est applicable aux clients qui ciblent Exchange Online et les versions d’Exchange à partir d’Exchange Server 2013. Cet espace de noms est inclus dans l’API Microsoft.Exchange.WebServices.Auth.dll.|
|[Microsoft.Exchange.WebServices.Autodiscover](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover?view=exchange-ews-api)|Contient des types utilisés pour communiquer avec le service de découverte automatique hébergé par un serveur Exchange. Cet espace de noms est également utilisé pour rechercher des objets de point de connexion de service dans les services de domaine Active Directory (AD DS). Les services de découverte automatique fournissent des informations de configuration aux clients EWS. Ainsi, les clients peuvent cibler l’URL du service approprié.<br/><br/>La fonctionnalité d’espace de noms peut servir à cibler le service de découverte automatique POX introduit dans Microsoft Exchange Server 2007, la recherche d’objet de point de connexion de service si le client est joint au domaine, ou le point de terminaison de découverte automatique SOAP introduit dans Exchange Server 2010. Le type principal dans cet espace de noms est la classe [AutodiscoverService](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover.autodiscoverservice?view=exchange-ews-api). Cet espace de noms est inclus dans l’API Microsoft.Exchange.WebServices.dll.|
|[Microsoft.Exchange.WebServices.Data](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data?view=exchange-ews-api)| Contient des types utilisés pour communiquer avec un serveur Exchange grâce à EWS. Cet espace de noms fournit la fonctionnalité clé d’API managée EWS. Le type principal dans cet espace de noms est la classe [ExchangeService](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice?view=exchange-ews-api).|

## <a name="see-also"></a>Voir aussi

- [Référence des services web pour Exchange](web-services-reference-for-exchange.md)
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Nouveautés dans EWS et autres services web dans Exchange](../exchange-web-services/whats-new-in-ews-and-other-web-services-in-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Développer des clients de service web pour Exchange](../exchange-web-services/develop-web-service-clients-for-exchange.md)

