---
title: Gestion de l’accès des utilisateurs à l’aide d’EWS Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Découvrez les options disponibles pour gérer l’accès des comptes d’utilisateurs à Exchange serveur.
ms.openlocfilehash: 431f61a0cbdfcc522eb1481399ffab1f31df9e62
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520975"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Gestion de l’accès des utilisateurs à l’aide d’EWS Exchange

Découvrez les options disponibles pour gérer l’accès des comptes d’utilisateurs à Exchange serveur.
  
Exchange Les services web (EWS) et l’API gérée EWS fournissent un nombre limité d’opérations que vous pouvez utiliser pour gérer des comptes sur Exchange Online, Exchange Online dans le cadre de Office 365 ou une version de Exchange à partir de Exchange 2013. Vous pouvez utiliser les opérations indiquées dans la figure suivante pour gérer les délégués et définir des autorisations d’accès aux dossiers pour d’autres comptes. 
  
**Opérations EWS pour l’accès délégué et aux dossiers**

![Options de gestion des utilisateurs EWS.](media/Exchange_ManagingUserAccess_1.png)
  
Si votre application a besoin d’un contrôle supplémentaire sur les comptes sur un serveur Exchange, vous pouvez utiliser les cmdlets Exchange Management Shell pour gérer les comptes. Vous pouvez appeler les cmdlets Exchange Management Shell en faisant l’une des choses suivantes :
  
- Écriture d’une application à l C# ou Visual Basic qui appelle les cmdlets Exchange Management Shell. Vous pouvez examiner l’exemple de code de la [documentation de l’API Exchange Management Shell](../management/exchange-management-shell.md) pour savoir comment appeler une cmdlet. 
    
- Utilisation Windows PowerShell et Windows PowerShell scripts pour appeler Exchange cmdlets Management Shell. Vous trouverez une liste complète des Exchange Server [PowerShell (Exchange Management Shell),](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)ainsi que des exemples qui montrent comment les utiliser. 
    
## <a name="see-also"></a>Voir aussi

- [Configuration de votre application EWS](setting-up-your-ews-application.md)   
- [Exchange 2013](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)  
    

