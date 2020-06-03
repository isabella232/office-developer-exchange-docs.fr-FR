---
title: Besoins de redistribution pour l'API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Découvrez comment vous pouvez redistribuer les assemblys d’API managée EWS avec votre application.
ms.openlocfilehash: e64b4cdb8938caa819ba30621112a25946ef0424
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463824"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Besoins de redistribution pour l'API managée EWS

Découvrez comment vous pouvez redistribuer les assemblys d’API managée EWS avec votre application.
  
Lors de la conception de votre application d’API managée EWS, vous devez également prendre en compte la manière dont vous allez la libérer pour vos utilisateurs. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Redistribution de votre application d’API managée EWS

À moins que votre application se trouve sur le serveur Exchange, vous devrez redistribuer les assemblys de l’API managée EWS. Le téléchargement de l’API managée EWS contient deux assemblys que vous pouvez redistribuer : Microsoft. Exchange. WebServices. dll et Microsoft. Exchange. WebServices. auth. dll. Gardez les informations suivantes à l’esprit lors de la conception de votre application d’API managée EWS :
  
- L’API managée EWS a été conçue de sorte que vous pouvez la télécharger et la distribuer avec votre application qui cible un serveur Exchange. Par ailleurs, votre application peut télécharger l’API managée EWS.
    
- Vous pouvez utiliser l’API managée EWS pour communiquer avec un serveur Exchange exécutant Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange à partir d’Exchange Server 2007.
    
- Dans les versions de l’API managée EWS à partir de la version 2,1, vous pouvez installer l’API dans le global assembly cache (GAC). Le MSI ajoutera automatiquement la DLL au GAC et sera accessible par ordinateur, et non par utilisateur.
    
Les termes du contrat de licence sont inclus dans le téléchargement de l’API managée EWS. Passez en revue les termes des informations faisant autorité sur ce que vous pouvez faire avec l’API managée EWS.
  
## <a name="see-also"></a>Voir aussi


- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    
- [API managée EWS (téléchargement)](https://aka.ms/ews-managed-api-readme)
    

