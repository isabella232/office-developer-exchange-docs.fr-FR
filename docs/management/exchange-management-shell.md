---
title: Environnement de ligne de commande Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Découvrez comment utiliser l’Exchange Management Shell pour développer des outils d’administration Exchange serveur.
ms.openlocfilehash: ee1cbcb174c7153ca6cd9bb089580b372bf9029b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516152"
---
# <a name="exchange-management-shell"></a>Environnement de ligne de commande Exchange Management Shell

Découvrez comment utiliser l’Exchange Management Shell pour développer des outils d’administration Exchange serveur.
  
**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365
  
L’Exchange Management Shell fournit un ensemble riche de commandes, basées sur la plateforme Windows PowerShell, pour gérer Exchange Online, Exchange Online dans le cadre de Office 365 ou une version sur site de Exchange à partir de Exchange 2013. Vous pouvez utiliser l’environnement de ligne de commande Exchange Management Shell pour créer deux types d’outils : les scripts de ligne de commande qui fonctionnent dans l’environnement Windows PowerShell et les outils qui utilisent les cmdlets Exchange Management Shell via une interface gérée. Vous pouvez utiliser des applications gérées pour créer une interface utilisateur Windows ou web standard pour administrer un serveur Exchange web. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Ce que vous devez savoir sur Exchange Management Shell

|Si vous vous demandez à propos de|Voici la réponse|
|:-----|:-----|
|Disponibilité  <br/> |Exchange Les commandes Management Shell sont installées sur tous les serveurs exécutant des versions de Exchange à partir de Exchange 2007.<br/>Les applications clientes peuvent être déployées sur n’importe quel ordinateur exécutant Windows PowerShell 2.0.<br/> Pour plus d’informations sur l’accès au shell, [voir Exchange Server PowerShell (Exchange Management Shell).](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  <br/> |
|Langages et outils  <br/> |Vous pouvez créer des scripts Exchange Management Shell dans n’importe quel éditeur de texte.<br/>Vous pouvez utiliser l’un des nombreux outils tiers pour créer Windows PowerShell scripts qui peuvent être utilisés avec Exchange Management Shell.  <br/> Le [Exchange d’objet Management Shell](exchange-management-shell-namespaces.md) est basé sur le .NET Framework.<br/>Vous pouvez utiliser n’importe quel langage .NET pour développer des applications Exchange Management Shell.  <br/> |
|Les outils de test et de débogage disponibles  <br/> |Vous pouvez utiliser l’une des nombreuses applications tierces pour tester et déboguer des scripts Exchange Management Shell.  <br/> Vous pouvez utiliser des Visual Studio et des outils tiers pour tester et déboguer des applications Exchange Management Shell.  <br/> |
|Exigences en matière de plateforme de serveur  <br/> |Vous pouvez utiliser l’Exchange Management Shell sur n’importe quel serveur Exchange sur Windows PowerShell 2.0.  <br/> |
|Exigences en matière de plateforme cliente  <br/> |Exchange Les applications clientes Management Shell nécessitent Windows PowerShell 2.0.  <br/> |
|Autorisations  <br/> |L’exécution d Exchange’application Management Shell nécessite que l’utilisateur a des droits de contrôle d’accès basés sur les rôles pour les données affectées dans Exchange store.<br/>Pour plus d’informations sur le contrôle d’accès basé sur un rôle, voir [Understanding Role Based Access Control](https://technet.microsoft.com/library/dd298183.aspx).  <br/> |
   
Les articles de cette section décrivent les fonctionnalités Exchange Management Shell qui sont importantes pour la création d Exchange outils de gestion. Pour plus d’informations sur la planification, la configuration ou la maintenance Exchange, voir [Exchange](https://docs.microsoft.com/exchange/) site.
  
## <a name="in-this-section"></a>Dans cette section

- [Créer des outils d’environnement de ligne de commande Exchange Management Shell](create-exchange-management-shell-tools.md)
    
- [Espaces de noms de l’environnement de ligne de commande Exchange Management Shell](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>Voir aussi
  
- [Windows PowerShell documentation](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Scripts PowerShell](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

