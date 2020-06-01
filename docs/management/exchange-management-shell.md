---
title: Environnement de ligne de commande Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Trouvez des informations sur l’utilisation de l’environnement de commande Exchange Management Shell pour développer des outils pour l’administration d’Exchange Server.
ms.openlocfilehash: 38e75339a4ad97cf8ff99e1cbe9c01059e157941
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435806"
---
# <a name="exchange-management-shell"></a>Environnement de ligne de commande Exchange Management Shell

Trouvez des informations sur l’utilisation de l’environnement de commande Exchange Management Shell pour développer des outils pour l’administration d’Exchange Server.
  
**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365
  
L’environnement de ligne de commande Exchange Management Shell fournit un ensemble complet de commandes, basées sur la plateforme Windows PowerShell, pour la gestion d’Exchange Online, Exchange Online dans le cadre d’Office 365 ou d’une version locale d’Exchange à partir d’Exchange 2013. Vous pouvez utiliser l’environnement de ligne de commande Exchange Management Shell pour créer deux types d’outils : les scripts de ligne de commande qui fonctionnent dans l’environnement Windows PowerShell, ainsi que les outils qui utilisent les cmdlets de l’environnement de ligne de commande Exchange Management Shell via une interface managée. Vous pouvez utiliser des applications gérées pour créer une interface utilisateur Windows ou Web standard pour administrer un serveur Exchange. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Ce que vous devez savoir sur l’environnement de commande Exchange Management Shell

|Si vous vous posez des informations sur|Voici la réponse|
|:-----|:-----|
|Disponibilité  <br/> |Les commandes de l’environnement de commande Exchange Management Shell sont installées sur tous les serveurs exécutant des versions d’Exchange à partir d’Exchange 2007.<br/>Les applications clientes peuvent être déployées sur n’importe quel ordinateur exécutant Windows PowerShell 2,0.<br/> Pour plus d’informations sur l’accès à l’environnement de commande Exchange Management Shell, consultez la rubrique [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).  <br/> |
|Langages et outils  <br/> |Vous pouvez créer des scripts Exchange Management Shell dans n’importe quel éditeur de texte.<br/>Vous pouvez utiliser l’un des nombreux outils tiers pour créer des scripts Windows PowerShell qui peuvent être utilisés avec l’environnement de commande Exchange Management Shell.  <br/> Le [modèle objet de l’environnement de commande Exchange Management Shell](exchange-management-shell-namespaces.md) repose sur .NET Framework.<br/>Vous pouvez utiliser n’importe quel langage .NET pour développer des applications Exchange Management Shell.  <br/> |
|Les outils de test et de débogage disponibles  <br/> |Vous pouvez utiliser l’une des nombreuses applications tierces pour tester et déboguer les scripts Exchange Management Shell.  <br/> Vous pouvez utiliser Visual Studio et des outils tiers pour tester et déboguer des applications Exchange Management Shell gérées.  <br/> |
|Exigences en matière de plateforme de serveur  <br/> |Vous pouvez utiliser l’environnement de commande Exchange Management Shell sur n’importe quel serveur Exchange sur lequel Windows PowerShell 2,0 est installé.  <br/> |
|Exigences en matière de plateforme cliente  <br/> |Les applications clientes de l’environnement de commande Exchange Management Shell requièrent Windows PowerShell 2,0.  <br/> |
|Autorisations  <br/> |L’exécution d’une application Exchange Management Shell nécessite que l’utilisateur dispose de droits de contrôle d’accès basé sur un rôle sur les données affectées dans la Banque d’informations Exchange.<br/>Pour plus d’informations sur le contrôle d’accès basé sur un rôle, voir [Understanding Role Based Access Control](https://technet.microsoft.com/library/dd298183.aspx).  <br/> |
   
Les Articles de cette section décrivent les fonctionnalités de l’environnement de commande Exchange Management Shell qui sont importantes pour la création d’outils de gestion Exchange. Pour plus d’informations sur la planification, la configuration ou la maintenance d’Exchange, consultez la rubrique site [Exchange](https://docs.microsoft.com/exchange/) .
  
## <a name="in-this-section"></a>Dans cette section

- [Créer des outils d’environnement de commande Exchange Management Shell](create-exchange-management-shell-tools.md)
    
- [Espaces de noms Exchange Management Shell](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>Voir aussi
  
- [Documentation Windows PowerShell](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Scripts PowerShell](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

