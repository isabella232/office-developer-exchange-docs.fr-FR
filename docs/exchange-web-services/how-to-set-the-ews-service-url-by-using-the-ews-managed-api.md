---
title: Définir l’URL du service EWS à l’aide de l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: Trouver des informations sur la manière de définir l’URL du service EWS dans votre application API managée EWS.
localization_priority: Priority
ms.openlocfilehash: 5ba79b48d4eb4fec62110448c5924de16b67ce10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456728"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a>Définir l’URL du service EWS à l’aide de l’API managée EWS

Trouver des informations sur la manière de définir l’URL du service EWS dans votre application API managée EWS.
  
L'URL du service est l'adresse qu'Exchange utilise pour communiquer avec les services web Exchange (EWS). Une fois que votre application d'API managée EWS a cette adresse et qu'elle dispose d'un accès approprié pour [communiquer avec EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md), elle peut effectuer des appels vers la [classe ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). L'URL du service pour un serveur Exchange local peut se présenter comme suit. 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

Vous pouvez définir l'URL EWS dans votre application de deux manières. Nous vous conseillons d'utiliser le [service de découverte automatique](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx) pour obtenir l'URL, car dans une vaste forêt de serveurs, l'URL peut changer si la boîte aux lettres est migrée vers un autre serveur. Toutefois, comme l'appel du service de découverte automatique peut prendre du temps et ralentir votre application, si vous devez effectuer plusieurs appels sur une courte période, vous devrez peut-être mettre en cache la valeur de l'URL obtenue grâce à la découverte automatique et définir manuellement l'URL du service EWS à l'aide de cette valeur mise en cache. Cela améliore les performances de votre application ; veillez simplement à utiliser la découverte automatique pour mettre à jour régulièrement la valeur mise en cache, au cas où la valeur soit modifiée sur le serveur. 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a>Définir l'URL du service EWS en utilisant le service de découverte automatique
<a name="bk_SetURLusingAutoDiscover"> </a>

La méthode [AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) utilise l'adresse électronique pour définir le point de terminaison [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et elle permet à votre application d'utiliser toutes les méthodes incluses dans les classes proxy **ExchangeService**. L'exemple qui suit illustre l'utilisation de la méthode **AutodiscoverURL**. 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a>Définir manuellement l'URL du service Exchange
<a name="bk_SetURLmanually"> </a>

L'exemple qui suit illustre la définition de l'URL du service EWS à l'aide d'une valeur mise en cache. Avant cela, veillez à utiliser le service de découverte automatique pour obtenir l'URL EWS.
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a>Voir aussi

- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md)   
- [Configuration de votre environnement de développement d’application Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Contrôler l’accès à EWS dans Exchange](how-to-control-access-to-ews-in-exchange.md) 
- [Communiquer avec EWS à l'aide de l'API managée EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [Utilisation de la découverte automatique pour trouver des points de connexion](how-to-use-autodiscover-to-find-connection-points.md)
    

