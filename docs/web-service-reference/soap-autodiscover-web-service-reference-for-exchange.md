---
title: SOAP de référence de service web de découverte automatique pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Trouvez des informations de référence pour le service de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>SOAP de référence de service web de découverte automatique pour Exchange

Trouvez des informations de référence pour le service de découverte automatique SOAP dans Exchange.
  
Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange. Vous pouvez utiliser le service de découverte automatique SOAP pour envoyer des messages entre l’application cliente et le serveur Exchange pour rechercher les paramètres de que l’application utilise pour se connecter à Exchange. Contrairement au service de découverte automatique variole, le service de découverte automatique SOAP permet pour les demandes de découverte automatique par lots pour les paramètres de nombreux utilisateurs et un contrôle plus précis sur les paramètres sont retournés dans la réponse. 
  
> [!NOTE]
> Pour les clients qui ciblent les versions d’Exchange commençant par Exchange Server 2010, il est recommandé que vous utilisez le service de découverte automatique SOAP (plutôt que le service de découverte automatique variole). Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique variole. Il est recommandé que les clients qui utilisent le .NET Framework utilisent l’API managée EWS, car il contient un client SOAP Autodiscover robuste et bien testé. Pour plus d’informations sur l’API managée EWS, voir [prendre en main des applications clientes API managées](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur au cours des redirections de demande SOAP Autodiscover et les paramètres utilisateur sont retournés dans une réponse. Référence à l’élément XML contient les résumés de ce qui représentent les éléments et une description des hiérarchies potentiels d’élément qui contient l’élément. 
  
Les articles de cette section décrivent les instances XML qui sont envoyés entre le client et le serveur. Vous trouverez le schéma qui décrit les éléments suivants dans le répertoire virtuel du serveur qui héberge le service de découverte automatique SOAP.
  
L’opération WSDL rubriques de cette section fournissent qu'une vue d’ensemble de l’opération qui est et des exemples de requête et de réponse opération. Vous pouvez utiliser les informations de version fournies pour déterminer si les fonctionnalités que vous souhaitez utiliser sont disponibles dans la version du produit que vous exécutez. Les exemples dans les rubriques opération également vous aident à comprendre la structure du code XML qui est inclus dans les messages SOAP qui sont envoyés vers ou à partir du serveur.
  
Cette section fournit des exemples et une description des messages qui sont utilisées pour extraire des informations de configuration de découverte automatique en utilisant le service de découverte automatique SOAP. 
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_InThisSection"> </a>

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
    
- [Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
    
- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
    
- [Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Éléments du fichier XML Autodiscover SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi


- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Utiliser la découverte automatique pour rechercher les points de connexion](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Obtenir les paramètres de domaine à partir d’un serveur Exchange](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

