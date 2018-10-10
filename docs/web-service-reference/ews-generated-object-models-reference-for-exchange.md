---
title: Modèles d’objet générés par les services Web Exchange (EWS) pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 67d7d831-9c53-46da-80e4-18f562e71284
description: Si vous utilisez la référence des modèles d’objet générés par EWS pour développer des applications pour Exchange, découvrez les autres options pour le développement EWS.
ms.openlocfilehash: 94735a205748116457cb74efc2a75b0b2aa2c9ec
ms.sourcegitcommit: 4221fd619bc309d2f8ab0497ec780b427acc6530
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/08/2018
ms.locfileid: "25441532"
---
# <a name="ews-generated-object-models-for-exchange"></a>Modèles d’objet générés par EWS pour Exchange

**S’applique à** : Exchange Online | Exchange Server 2013 | Office 365

Le modèle objet Exchange Web Services (EWS) généré par wsdl.exe fourni initialement un modèle d’objet pratique pour travailler avec Exchange 2007. Toutefois, la mise à disposition de l’API managée EWS a fourni un certain nombre d’avantages pour les développeurs qui utilisent du code managé. 

L’API managée EWS :

- fournit un modèle d’objet plus intuitif ;

- contient une validation des données et une logique métier côté client ;

- est entièrement prise en charge et mise à jour régulièrement ;

- contient un client de découverte automatique ;

- implémente des fonctionnalités client telles que la journalisation, la gestion des cookies et les rapports de diagnostic dans Exchange.

La documentation pour la référence managée EWS basée sur wsdl.exe a été supprimée, car l’API managée EWS remplace la plupart des fonctionnalités fournies par les modèles d’objet générés. En même temps, nous savons que l’API managée EWS n’est pas pour tout le monde. La plupart du temps, il est recommandé de créer des clients EWS pour .NET, mais il existe quelques exceptions ; par exemple :

- Lorsque vous décidez d’utiliser des fonctionnalités qui [n’ont pas été implémentées dans l’API managée EWS](../exchange-web-services/web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md#bk_apifeatures).

- Lorsque vous utilisez une plateforme de développement différente de .NET.

Si vous ne pouvez pas utiliser l’API managée EWS pour développer votre application, vous pouvez procéder comme suit :

- Utiliser une API client EWS tierce

- Créer votre propre modèle d’objet client EWS

- Utiliser un générateur de modèle d’objet Des générateurs de modèles d’objet prenant en charge la plupart des langues et plateformes sont disponibles.

Si vous prévoyez d’utiliser un générateur de modèle d’objet, vous pouvez utiliser la référence XML afin de comprendre le modèle d’objet généré. Le modèle d’objet est généré à partir de structures XML décrites dans le schéma. En règle générale, les classes créées par des générateurs de modèles d’objet correspondent aux types complexes dans le schéma. Les propriétés correspondent généralement aux éléments XML.

Affichez l’[espace de noms ExchangeWebServices](https://docs.microsoft.com/dotnet/api/exchangewebservices?view=exchange-ews-proxy).

## <a name="see-also"></a>Voir aussi

- [Référence des services web pour Exchange](web-services-reference-for-exchange.md)
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Nouveautés dans EWS et autres services web dans Exchange](../exchange-web-services/whats-new-in-ews-and-other-web-services-in-exchange.md)
