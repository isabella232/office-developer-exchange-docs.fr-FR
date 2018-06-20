---
title: Gestion de l’accès utilisateur à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Découvrez quelles sont vos options pour la gestion de compte d’utilisateur accès à votre serveur Exchange.
ms.openlocfilehash: d93f521f08f93b44b4ecc1f258b03ed24ebdd3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754973"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Gestion de l’accès utilisateur à l’aide de EWS dans Exchange

Découvrez quelles sont vos options pour la gestion de compte d’utilisateur accès à votre serveur Exchange.
  
API gérée d’Exchange Web Services (EWS) et le EWS fournissent un nombre limité d’opérations que vous pouvez utiliser pour gérer les comptes dans Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version d’Exchange commençant par Exchange 2013. Vous pouvez utiliser les opérations indiquées dans la figure suivante pour gérer les délégués et pour définir des autorisations d’accès au dossier pour les autres comptes. 
  
**Opérations EWS pour l’accès délégué et de dossier**

![Options de gestion des utilisateurs EWS.](media/Exchange_ManagingUserAccess_1.png)
  
Si votre application a besoin d’un contrôle supplémentaire sur les comptes sur un serveur Exchange, vous pouvez utiliser les applets de commande Exchange Management Shell pour gérer les comptes. Vous pouvez appeler les applets de commande Exchange Management Shell en effectuant l’une des options suivantes :
  
- Écriture d’une application à l’aide de c# ou Visual Basic qui appelle les applets de commande Exchange Management Shell. Vous pouvez consulter l’exemple de code dans la [documentation sur Exchange Management Shell API](../management/exchange-management-shell.md) pour découvrir comment appeler une applet de commande. 
    
- À l’aide de Windows PowerShell et les scripts Windows PowerShell pour appeler les applets de commande Exchange Management Shell. Vous trouverez une liste complète de la [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), ainsi que des exemples qui montrent comment les utiliser. 
    
## <a name="see-also"></a>Voir aussi

- [La configuration de vos applications EWS](setting-up-your-ews-application.md)   
- [Applets de commande Exchange 2013](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

