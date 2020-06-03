---
title: Éléments XML de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Recherchez des informations de référence pour les éléments XML EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526115"
---
# <a name="ews-xml-elements-in-exchange"></a>Éléments XML de EWS dans Exchange

Recherchez des informations de référence pour les éléments XML EWS dans Exchange.
  
Les services Web Exchange (EWS) sont un service Web basé sur SOAP, ce qui signifie que les messages de demande et de réponse échangés entre le client et le serveur sont constitués d’éléments XML. La documentation de cette section est basée sur les instances XML qui sont envoyées entre le client et le serveur. Les instances XML sont définies dans les fichiers WSDL et de schéma qui se trouvent dans le répertoire virtuel qui héberge EWS. Si vous êtes un utilisateur authentifié, vous pouvez accéder aux fichiers WSDL et de schéma à l’aide des URL suivantes, où \<yourclientaccessserver\> est le nom de votre serveur d’accès au client :
  
- http:// \<yourclientaccessserver\> . com/EWS/services. wsdl : emplacement du fichier WSDL.
    
- http:// \<yourclientaccessserver\> . com/EWS/messages. xsd — l’emplacement du schéma des messages.
    
- http:// \<yourclientaccessserver\> . com/EWS/types. xsd — l’emplacement du schéma de types.
    
Les fichiers de schéma qui décrivent les éléments XML EWS fournissent une feuille de route générale de la structure XML qui est possible pour les interactions entre les messages demande-réponse. La structure XML réelle qui est envoyée entre le client et le serveur varie en fonction de l’opération qui est appelée, des informations demandées et des paramètres côté serveur.
  
Le fichier WSDL EWS, services. wsdl, n’est pas entièrement conforme à la norme WSDL, car il n’inclut pas de définition de service WSDL. En effet, EWS n’est pas conçu pour être hébergé sur un ordinateur disposant d’une adresse prédéfinie. Vous pouvez utiliser le service de découverte automatique pour obtenir l’adresse du point de terminaison EWS. Certains générateurs de modèle objet côté client analysent le WSDL et peuvent rencontrer une condition d’erreur car le fichier WSDL ne contient pas de définition de service WSDL. Si votre générateur de modèle objet rencontre une erreur, vous pouvez insérer une définition de service WSDL d’espace réservé.
  
> [!TIP]
> Si vous utilisez .NET Framework pour développer votre application, nous vous recommandons d’utiliser l' [API managée EWS](http://aka.ms/ews-managed-api-readme), plutôt qu’un générateur de modèle objet. L’API managée EWS fournit un modèle objet facile à utiliser pour gérer la sérialisation et la désérialisation du XML EWS. Pour plus d’informations, consultez la rubrique [prise en main des applications clientes d’API managée EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Le fichier de schéma messages. xsd contient les définitions d’élément pour les éléments de niveau supérieur dans le corps SOAP. À l’exception des codes de réponse d’erreur, la plupart des définitions dans messages. xsd sont propres à une opération. Le schéma types. xsd contient les définitions des en-têtes SOAP et toutes les définitions communes qui sont partagées entre les opérations.
  
## <a name="see-also"></a>Voir aussi

- [Référence EWS pour Exchange](ews-reference-for-exchange.md)
- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
- [Explorer l'API managée EWS, l’EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Commencer à utiliser les services web dans Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Découverte automatique pour Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

