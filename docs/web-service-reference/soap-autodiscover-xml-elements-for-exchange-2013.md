---
title: Éléments XML de découverte automatique SOAP pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Recherchez des informations de référence sur les éléments XML pour le service Web de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465183"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Éléments XML de découverte automatique SOAP pour Exchange 2013

Recherchez des informations de référence sur les éléments XML pour le service Web de découverte automatique SOAP dans Exchange.
  
La documentation de cette section est basée sur les instances d’éléments XML de découverte automatique SOAP qui sont envoyées entre le client et le serveur. La documentation de cette instance XML est basée sur les fichiers WSDL et de schéma qui se trouvent dans le répertoire virtuel qui héberge le service de découverte automatique SOAP. Les utilisateurs authentifiés peuvent accéder aux fichiers WSDL et de schéma à l’aide d’une URL semblable à l’une des suivantes :
  
- Emplacement du fichier WSDL : `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- Emplacement du schéma des messages : `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
L’emplacement des fichiers de schéma et WSDL de découverte automatique SOAP varie en fonction de l’installation d’Exchange.
  
Le fichier de schéma messages. xsd décrit les éléments XML qui peuvent être envoyés dans un en-tête SOAP de découverte automatique et un corps SOAP. Ce fichier fournit une feuille de route générale sur ce que peut être la structure XML pour une interaction de message demande-réponse donnée. La structure XML réelle qui est envoyée entre le client et le serveur est basée sur les options et le contexte dans lequel elle est utilisée. Les fichiers de schéma définissent les données XML possibles. La plage réelle de code XML envoyé sur le réseau est basée sur l’opération appelée, les informations demandées et les paramètres côté serveur. 
  
## <a name="related-sections"></a>Sections connexes

- [Référence de service Web de découverte automatique SOAP pour Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)    
- [Référence du service Web de messagerie unifiée pour Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

