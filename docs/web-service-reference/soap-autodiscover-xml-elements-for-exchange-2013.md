---
title: Éléments du fichier XML Autodiscover SOAP pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Trouvez des informations de référence d’élément XML pour le service web de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353391"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Éléments du fichier XML Autodiscover SOAP pour Exchange 2013

Trouvez des informations de référence d’élément XML pour le service web de découverte automatique SOAP dans Exchange.
  
La documentation de cette section est basée sur les instances d’élément XML de découverte automatique SOAP qui sont envoyés entre le client et le serveur. Cette documentation d’instance XML est basée sur les fichiers qui sont trouvent dans le répertoire virtuel qui héberge le service de découverte automatique SOAP WSDL et le schéma. Les utilisateurs authentifiés peuvent parcourir les fichiers WSDL et le schéma à l’aide d’une URL qui est similaire à une des options suivantes :
  
- L’emplacement du fichier WSDL : `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- L’emplacement du schéma des messages : `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
L’emplacement des fichiers de schéma et SOAP Autodiscover WSDL varie en fonction de l’installation d’Exchange.
  
Le fichier de schéma messages.xsd décrit les éléments XML qui peuvent être envoyés dans un en-tête SOAP de découverte automatique et le corps SOAP. Ce fichier fournit un guide général de la structure XML qui peut être pour une interaction de message de demande-réponse donnée. La structure XML réelle échangées entre le client et le serveur est basée sur les options et le contexte dans lequel il est utilisé. Les fichiers de schéma définissent ce que XML est possible. La plage de code XML qui est transmis sur le réseau est basé sur l’opération est appelé, les informations demandées et les paramètres côté serveur. 
  
## <a name="related-sections"></a>Sections associées

- [SOAP de référence de service web de découverte automatique pour Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)    
- [Référence au service web messagerie unifiée pour Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

