---
title: Contrôler l’accès à EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Découvrez comment contrôler l’accès à EWS pour les utilisateurs, des applications ou l’organisation toute entière.
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754812"
---
# <a name="control-access-to-ews-in-exchange"></a>Contrôler l’accès à EWS dans Exchange

Découvrez comment contrôler l’accès à EWS pour les utilisateurs, des applications ou l’organisation toute entière.
  
Si vous utilisez l’API managée EWS ou EWS directement dans votre application, vous pouvez contrôler l’accès à Exchange Web Services (EWS). Si vous avez accès d’administrateur sur votre serveur Exchange, vous pouvez gérer l’accès aux EWS à l’aide de l’environnement Exchange Management Shell pour contrôler l’accès au niveau global, pour chaque utilisateur et pour chaque application.
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a>Applets de commande Exchange Management Shell pour configurer le contrôle d’accès
<a name="bk_Cmdlets"> </a>

Vous pouvez utiliser les applets de commande Exchange Management Shell suivante pour afficher la configuration d’accès actuel et définir des contrôles d’accès EWS :
  
- [Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - affiche les paramètres sont définis pour une boîte aux lettres spécifique.   
- [Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - paramètres ensembles pour une boîte aux lettres spécifique.    
- [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - affiche les paramètres de l’organisation toute entière.    
- [Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - définit les paramètres de l’organisation toute entière. 

<a name="bk_Examples"> </a>

## <a name="examples-controlling-access-to-ews"></a>Exemples : Contrôler l’accès à EWS

Examinons quelques scénarios qui montrent comment vous pouvez contrôler l’accès à votre application.
  
**Le tableau 1. Commandes pour contrôler l’accès à EWS**

|Si vous souhaitez |Utilisez cette commande|
|:-----|:-----|
|Bloquer toutes les applications clientes d’utiliser EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/>Cela permet aux applications répertoriées dans le AllowList pour se connecter. Dans cet exemple, aucune application n’est incluse dans le AllowList, aucune application peut utiliser EWS. |
|Autoriser une liste de client applications afin d’utiliser EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/>Cela permet à des applications spécifiques à utiliser EWS. Dans cet exemple, n’importe quelle application qui a un agent utilisateur de chaîne qui commence par « OWA / » est autorisé à accéder. |
|Autoriser toutes les applications clientes à utiliser EWS, à l’exception de ceux qui sont spécifiquement bloqués. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/>Cet exemple montre comment bloque uniquement les applications à l’aide de EWS ayant une chaîne d’agent utilisateur qui commence par « OWA / ». |
|Autoriser toutes les applications clientes à utiliser EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> Étant donné qu’aucune liste de blocage n’est spécifié, toutes les applications peuvent utiliser EWS. |
|Bloquer l’organisation toute entière à partir de l’aide de EWS. | `Set-OrganizationConfig -EwsEnabled:$false` |
|Autoriser l’organisation toute entière à utiliser EWS. | `Set-OrganizationConfig -EwsEnabled:$true`|
|Bloquer une boîte aux lettres à partir de l’aide de EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|Autoriser une boîte aux lettres à utiliser EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a>Voir aussi

- [La configuration de vos applications EWS](setting-up-your-ews-application.md)    
- [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

