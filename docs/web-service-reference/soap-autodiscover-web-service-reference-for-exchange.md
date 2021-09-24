---
title: Référence du service web de découverte automatique SOAP pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Recherchez des informations de référence pour le service de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 488862f5797abfd71d33c916fa96970ab300a2c0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521353"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>Référence du service web de découverte automatique SOAP pour Exchange

Recherchez des informations de référence pour le service de découverte automatique SOAP dans Exchange.
  
Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à Exchange serveur. Vous pouvez utiliser le service de découverte automatique SOAP pour envoyer des messages entre l’application cliente et le serveur Exchange afin de localiser les paramètres que l’application utilisera pour se connecter à Exchange. Contrairement au service de découverte automatique POX, le service de découverte automatique SOAP autorise les demandes de découverte automatique par lot pour les paramètres de nombreux utilisateurs et un contrôle plus granulaire des paramètres renvoyés dans la réponse. 
  
> [!NOTE]
> Pour les clients qui ciblent des versions de Exchange à partir de Exchange Server 2010, nous vous recommandons d’utiliser le service de découverte automatique SOAP (au lieu du service de découverte automatique POX). Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique POX. Nous recommandons aux clients qui utilisent le .NET Framework l’API gérée EWS, car elle contient un client de découverte automatique SOAP robuste et bien testé. Pour plus d’informations sur l’API gérée EWS, voir Get [started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur pendant les redirections de demande de découverte automatique SOAP et les paramètres utilisateur renvoyés dans une réponse. La référence d’élément XML contient des résumés de ce que représentent les éléments et une description des hiérarchies d’éléments potentielles qui contiennent l’élément. 
  
Les articles de cette section décrivent les instances XML qui sont envoyées entre le client et le serveur. Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel du serveur qui héberge le service de découverte automatique SOAP.
  
Les rubriques d’opération WSDL de cette section fournissent une vue d’ensemble de ce que fait l’opération, ainsi que des exemples de demande d’opération et de réponse. Vous pouvez utiliser les informations de version fournies pour déterminer si les fonctionnalités que vous souhaitez utiliser sont disponibles dans la version du produit que vous exécutez. Les exemples des rubriques d’opération vous aident également à comprendre la structure du XML inclus dans les messages SOAP envoyés vers et depuis le serveur.
  
Cette section fournit également des exemples et des descriptions des messages utilisés pour récupérer des informations de configuration de découverte automatique à l’aide du service de découverte automatique SOAP. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
    
- [Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
    
- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
    
- [Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi


- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Utiliser la découverte automatique pour trouver des points de connexion](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Obtenir des paramètres de domaine à partir d’un serveur Exchange](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

