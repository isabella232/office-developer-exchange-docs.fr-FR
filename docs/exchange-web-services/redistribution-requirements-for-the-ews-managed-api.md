---
title: Configuration requise de redistribution pour l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Découvrez comment vous pouvez redistribuer les assemblys d’API managées avec votre application.
ms.openlocfilehash: d8fc57c4a2b3ed7d6218aeeed0fe88c2d3e0fbe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755062"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Configuration requise de redistribution pour l’API managée EWS

Découvrez comment vous pouvez redistribuer les assemblys d’API managées avec votre application.
  
Lorsque vous concevez votre application d’API managées, vous souhaiterez également à prendre en compte la façon dont vous serez la version à vos utilisateurs. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Redistribution votre application d’API managées

Sauf si votre application se trouve sur le serveur Exchange, vous devrez redistribuer les assemblys d’API managées. Le téléchargement d’API managées contient deux assemblys que vous pouvez redistribuer : Microsoft.Exchange.WebServices.dll et Microsoft.Exchange.WebServices.Auth.dll. Gardez les informations suivantes à l’esprit lorsque vous concevez comment vous libère votre application d’API managées :
  
- L’API managée EWS a été conçu de sorte que vous pouvez télécharger et distribuer avec votre application ciblant un serveur Exchange. Autrement, votre application peut télécharger l’API managée EWS.
    
- Vous pouvez utiliser l’API managée EWS pour communiquer avec un serveur Exchange exécutant Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange Server 2007.
    
- Dans les versions de l’API managée EWS depuis la version 2.1, vous pouvez installer l’API dans le Global Assembly Cache (GAC). Le fichier MSI ajoute automatiquement la DLL dans le GAC et est accessible sur chaque ordinateur, et non sur chaque utilisateur.
    
Les termes du contrat de licence est inclus dans le téléchargement d’API managées. Passez en revue les termes pour les informations de référence sur ce que vous pouvez faire avec l’API managée EWS.
  
## <a name="see-also"></a>Voir aussi


- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    
- [API managée EWS (télécharger)](http://aka.ms/ews-managed-api-readme)
    

