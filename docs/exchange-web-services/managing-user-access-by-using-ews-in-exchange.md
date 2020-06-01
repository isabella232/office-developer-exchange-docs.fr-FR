---
title: Gestion de l’accès des utilisateurs à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Découvrez les options disponibles pour la gestion de l’accès aux comptes d’utilisateurs à votre serveur Exchange.
ms.openlocfilehash: 476292d4db206f22cd84134ce2b46957e9fe85fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456242"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Gestion de l’accès des utilisateurs à l’aide d’EWS dans Exchange

Découvrez les options disponibles pour la gestion de l’accès aux comptes d’utilisateurs à votre serveur Exchange.
  
Les services Web Exchange (EWS) et l’API managée EWS fournissent un nombre limité d’opérations que vous pouvez utiliser pour gérer les comptes sur Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version d’Exchange à partir d’Exchange 2013. Vous pouvez utiliser les opérations illustrées dans la figure suivante pour gérer les délégués et définir des autorisations d’accès aux dossiers pour d’autres comptes. 
  
**Opérations EWS pour l’accès aux délégués et aux dossiers**

![Options de gestion des utilisateurs EWS.](media/Exchange_ManagingUserAccess_1.png)
  
Si votre application a besoin d’un contrôle supplémentaire sur les comptes sur un serveur Exchange, vous pouvez utiliser les cmdlets Exchange Management Shell pour gérer les comptes. Vous pouvez appeler les cmdlets de l’environnement de commande Exchange Management Shell en effectuant l’une des opérations suivantes :
  
- Écriture d’une application à l’aide de C# ou de Visual Basic qui appelle les cmdlets de l’environnement de commande Exchange Management Shell. Vous pouvez consulter l’exemple de code de la documentation de l’API de l’environnement de commande [Exchange Management Shell](../management/exchange-management-shell.md) pour savoir comment appeler une cmdlet. 
    
- Utilisation de scripts Windows PowerShell et Windows PowerShell pour appeler des applets de commande Exchange Management Shell. Vous trouverez une liste complète d' [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), ainsi que des exemples qui montrent comment les utiliser. 
    
## <a name="see-also"></a>Voir aussi

- [Configuration de votre application EWS](setting-up-your-ews-application.md)   
- [Applets de commande Exchange 2013](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)  
    

