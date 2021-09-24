---
title: Éléments XML de découverte automatique SOAP pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Recherchez des informations de référence sur les éléments XML pour le service web de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 5dcf4d6cd7a2b0b2987e59530dfbaae7b9993242
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539093"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Éléments XML de découverte automatique SOAP pour Exchange 2013

Recherchez des informations de référence sur les éléments XML pour le service web de découverte automatique SOAP dans Exchange.
  
La documentation de cette section est basée sur les instances de l’élément XML de découverte automatique SOAP qui sont envoyées entre le client et le serveur. Cette documentation d’instance XML est basée sur les fichiers WSDL et de schéma situés dans le répertoire virtuel qui héberge le service de découverte automatique SOAP. Les utilisateurs authentifiés peuvent accéder au fichier WSDL et aux fichiers de schéma à l’aide d’une URL semblable à l’une des suivantes :
  
- Emplacement du fichier WSDL : `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- Emplacement du schéma des messages : `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
L’emplacement du WSDL de découverte automatique SOAP et des fichiers de schéma varie en fonction de la Exchange’installation.
  
Le fichier de schéma messages.xsd décrit les éléments XML qui peuvent être envoyés dans un en-tête SOAP de découverte automatique et un corps SOAP. Ce fichier fournit une feuille de route générale sur ce que peut être la structure XML pour une interaction de message de demande-réponse donnée. La structure XML réelle qui est envoyée entre le client et le serveur est basée sur les options et le contexte dans lequel elle est utilisée. Les fichiers de schéma définissent ce que XML est possible. La plage réelle de données XML envoyées sur le réseau est basée sur l’opération appelée, les informations demandées et les paramètres côté serveur. 
  
## <a name="related-sections"></a>Sections connexes

- [Référence du service web de découverte automatique SOAP pour Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)    
- [Référence du service web de messagerie unifiée pour Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

