---
title: Configuration requise de redistribution pour l’API gérée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Découvrez comment redistribuer les assemblys d’API gérées EWS avec votre application.
ms.openlocfilehash: f43156838c735cfc17106deb7860329d3da6c07a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531329"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Configuration requise de redistribution pour l’API gérée EWS

Découvrez comment redistribuer les assemblys d’API gérées EWS avec votre application.
  
Lorsque vous concevez votre application d’API gérée EWS, vous devez également prendre en compte la façon dont vous allez la publier pour vos utilisateurs. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Redistribuer votre application API gérée EWS

À moins que votre application ne se trouve sur le serveur Exchange, vous devrez redistribuer les assemblys d’API gérée EWS. Le téléchargement de l’API gérée EWS contient deux assemblys que vous pouvez redistribuer : Microsoft.Exchange.WebServices.dll et Microsoft.Exchange.WebServices.Auth.dll. Gardez les informations suivantes à l’esprit lorsque vous concevez la façon dont vous allez publier votre application d’API gérée EWS :
  
- L’API gérée EWS a été conçue de telle manière que vous pouvez la télécharger et la distribuer avec votre application qui cible un Exchange serveur. Sinon, votre application peut télécharger l’API gérée EWS.
    
- Vous pouvez utiliser l’API gérée EWS pour communiquer avec un serveur Exchange exécutant Exchange Online, Exchange Online dans le cadre de Office 365 ou une version sur site de Exchange à partir de Exchange Server 2007.
    
- Dans les versions de l’API gérée EWS à partir de la version 2.1, vous pouvez installer l’API dans le Global Assembly Cache (GAC). Le MSI ajoute automatiquement la DLL au GAC et est accessible par ordinateur, et non par utilisateur.
    
Les termes du contrat de licence sont inclus dans le téléchargement de l’API gérée EWS. Examinez les termes pour obtenir des informations faisant autorité sur ce que vous pouvez faire avec l’API gérée EWS.
  
## <a name="see-also"></a>Voir aussi


- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    
- [API gérée EWS (téléchargement)](https://aka.ms/ews-managed-api-readme)
    

