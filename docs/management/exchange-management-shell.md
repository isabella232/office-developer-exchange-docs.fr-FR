---
title: Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Trouvez des informations sur l’utilisation d’Exchange Management Shell pour développer des outils d’administration Exchange server.
ms.openlocfilehash: 1cb0328bdb0eebda0ce4eda929e1bfb21be451f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755080"
---
# <a name="exchange-management-shell"></a>Exchange Management Shell

Trouvez des informations sur l’utilisation d’Exchange Management Shell pour développer des outils d’administration Exchange server.
  
**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365
  
Exchange Management Shell fournit un ensemble complet de commandes, en fonction de la plateforme de Windows PowerShell pour gérer Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange 2013. Vous pouvez utiliser l’environnement Exchange Management Shell pour créer deux types d’outils : scripts de ligne de commande qui fonctionnent dans l’environnement Windows PowerShell et les outils qui utilisent les applets de commande Exchange Management Shell via une interface managée. Vous pouvez utiliser des applications managées pour créer un standard de Windows ou l’interface utilisateur web pour administrer un serveur Exchange. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Vous devez savoir sur Exchange Management Shell

|Si vous vous interrogez sur|Voici la réponse|
|:-----|:-----|
|Disponibilité  <br/> |Commandes d’Exchange Management Shell sont installés sur tous les serveurs exécutant des versions d’Exchange commençant par Exchange 2007.<br/>Applications clientes peuvent être déployées sur tout ordinateur exécutant Windows PowerShell 2.0.<br/> Pour plus d’informations sur l’accès à l’interpréteur de commandes, voir [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).  <br/> |
|Langages et outils  <br/> |Vous pouvez créer des scripts Exchange Management Shell dans n’importe quel éditeur de texte.<br/>Vous pouvez utiliser un des nombreux outils tiers pour la création de scripts Windows PowerShell qui peuvent être utilisés avec Exchange Management Shell.  <br/> Le [modèle d’objet Exchange Management Shell](exchange-management-shell-namespaces.md) est basé sur le .NET Framework.<br/>Vous pouvez utiliser n’importe quel langage .NET pour développer des applications Exchange Management Shell.  <br/> |
|Les outils de test et de débogage disponibles  <br/> |Vous pouvez utiliser une des nombreuses applications tierces pour tester et déboguer des scripts Exchange Management Shell.  <br/> Vous pouvez utiliser Visual Studio et des outils tiers pour tester et déboguer d’Exchange Management Shell applications managées.  <br/> |
|Exigences en matière de plateforme de serveur  <br/> |Vous pouvez utiliser l’environnement Exchange Management Shell sur n’importe quel serveur Exchange qui a installé Windows PowerShell 2.0.  <br/> |
|Exigences en matière de plateforme cliente  <br/> |Les applications de client Exchange Management Shell nécessitent Windows PowerShell 2.0.  <br/> |
|Autorisations  <br/> |Un serveur Exchange Management Shell en cours d’exécution application nécessite que l’utilisateur possède des droits de contrôle d’accès basé sur un rôle de données affectées sur la banque d’informations Exchange.<br/>Pour plus d’informations sur le contrôle d’accès basé sur un rôle, voir [Understanding Role Based Access Control](http://technet.microsoft.com/en-us/library/dd298183.aspx).  <br/> |
   
Les articles de cette section décrivent les fonctionnalités d’Exchange Management Shell qui sont importantes pour la création d’outils de gestion Exchange. Pour plus d’informations sur la planification, la configuration ou la maintenance d’Exchange, consultez le site [Exchange](https://docs.microsoft.com/en-us/exchange/) .
  
## <a name="in-this-section"></a>Dans cette section

- [Créer des outils Exchange Management Shell](create-exchange-management-shell-tools.md)
    
- [Espaces de noms Exchange Management Shell](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>Voir aussi
  
- [Documentation de Windows PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Écriture de scripts PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/powershell-scripting?view=powershell-6)
    

