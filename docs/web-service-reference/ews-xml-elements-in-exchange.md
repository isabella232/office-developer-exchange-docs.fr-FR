---
title: Éléments XML EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Rechercher des informations de référence pour les données XML EWS éléments dans Exchange.
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756238"
---
# <a name="ews-xml-elements-in-exchange"></a>Éléments XML EWS dans Exchange

Rechercher des informations de référence pour les données XML EWS éléments dans Exchange.
  
Exchange Web Services (EWS) est un service web basé sur SOAP, ce qui signifie que les messages de demande et de réponse qui sont envoyés entre le client et le serveur sont composent des éléments XML. La documentation de cette section est basée sur les instances XML qui sont envoyés entre le client et le serveur. Les instances XML sont définies dans les fichiers WSDL et le schéma qui sont trouvent dans le répertoire virtuel qui héberge EWS. Si vous êtes un utilisateur authentifié, vous accédez aux fichiers WSDL et le schéma à l’aide de l’URL suivantes, où \<yourclientaccessserver\> est le nom de votre serveur d’accès au Client :
  
- http://\<yourclientaccessserver\>.com/ews/services.wsdl — l’emplacement du fichier WSDL.
    
- http://\<yourclientaccessserver\>.com/ews/messages.xsd — l’emplacement du schéma des messages.
    
- http://\<yourclientaccessserver\>.com/ews/types.xsd — l’emplacement du schéma de types.
    
Les fichiers de schéma qui décrivent les éléments XML EWS fournissent une feuille de route générale de la structure XML est possible, pour les interactions de message de réponse à la demande. La structure XML réelle qui est envoyée entre client et serveur varie en fonction de l’opération qui est appelée, les informations demandées et les paramètres côté serveur.
  
Le fichier WSDL EWS, services.wsdl, n’est pas entièrement conforme à la norme WSDL, car il n’inclut pas une définition de service WSDL. C’est pourquoi EWS n’est pas conçu pour être hébergé sur un ordinateur disposant d’une adresse prédéfinie. Vous pouvez utiliser le service de découverte automatique pour obtenir l’adresse de point de terminaison EWS. Certains générateurs de modèle objet côté client analyser le fichier WSDL et peuvent rencontrer une condition d’erreur car le fichier WSDL ne contient pas d’une définition de service WSDL. Si votre générateur de modèle d’objet rencontre une erreur, vous pouvez insérer un espace réservé définition WSDL du service.
  
> [!TIP]
> Si vous utilisez le .NET Framework pour développer votre application, nous vous recommandons d’utiliser l' [API managée EWS](http://aka.ms/ews-managed-api-readme), plutôt que d’un générateur de modèle d’objet. L’API managée EWS fournit un modèle d’objet à utiliser pour gérer la sérialisation et la désérialisation XML EWS. Pour plus d’informations, voir [prendre en main des applications clientes API managées](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Le fichier de schéma messages.xsd contient les définitions d’élément pour les éléments de niveau supérieur dans le corps SOAP. À l’exception des codes de réponse d’erreur, la plupart des définitions de messages.xsd sont spécifique à une opération. Le schéma types.xsd contient les définitions pour les en-têtes SOAP et toutes les définitions de courants qui sont partagées entre les opérations.
  
## <a name="see-also"></a>Voir aussi

- [Référence EWS pour Exchange](ews-reference-for-exchange.md)
- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

