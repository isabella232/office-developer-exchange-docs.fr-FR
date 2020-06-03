---
title: Contrôler l’accès à EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: Découvrez comment contrôler l’accès à EWS pour les utilisateurs, les applications ou l’ensemble de l’organisation.
localization_priority: Priority
ms.openlocfilehash: bd65b099ab15c1514945d8a1cfa4e9b1428a4755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456877"
---
# <a name="control-access-to-ews-in-exchange"></a>Contrôler l’accès à EWS dans Exchange

Découvrez comment contrôler l’accès à EWS pour les utilisateurs, les applications ou l’ensemble de l’organisation.
  
Que vous utilisiez l’API managée EWS ou EWS directement, dans votre application, vous pouvez contrôler l’accès aux services Web Exchange (EWS). Si vous disposez d’un accès administrateur à votre serveur Exchange, vous pouvez gérer l’accès à EWS à l’aide de l’environnement de commande Exchange Management Shell pour contrôler l’accès au niveau global, pour chaque utilisateur et pour chaque application.
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a>Applets de commande Exchange Management Shell pour la configuration du contrôle d’accès
<a name="bk_Cmdlets"> </a>

Vous pouvez utiliser les cmdlets de l’environnement de commande Exchange Management Shell suivantes pour afficher la configuration d’accès actuelle et définir les contrôles d’accès EWS :
  
- [Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx) -vous indique quels paramètres sont définis pour une boîte aux lettres particulière.   
- [Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx) : définit les paramètres d’une boîte aux lettres particulière.    
- [Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx) -affiche les paramètres de l’ensemble de l’organisation.    
- [Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx) -définit les paramètres pour l’ensemble de l’organisation. 

<a name="bk_Examples"> </a>

## <a name="examples-controlling-access-to-ews"></a>Exemples : contrôler l’accès à EWS

Examinons quelques scénarios qui vous montrent comment vous pouvez contrôler l’accès à votre application.
  
**Tableau 1. Commandes permettant de contrôler l’accès à EWS**

|Si vous souhaitez... |Utilisez cette commande|
|:-----|:-----|
|Bloquer toutes les applications clientes à l’aide d’EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/>Cela permet aux applications figurant dans le AllowList de se connecter. Dans cet exemple, aucune application n’est incluse dans le AllowList, de sorte qu’aucune application ne puisse utiliser EWS. |
|Autoriser une liste d’applications clientes à utiliser EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/>Cela permet à des applications spécifiques d’utiliser EWS. Dans cet exemple, toute application dont la chaîne de l’agent utilisateur commence par « OWA/ » est autorisée à accéder. |
|Autorisez toutes les applications clientes à utiliser EWS, sauf celles qui sont spécifiquement bloquées. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/>Cet exemple empêche uniquement les applications d’utiliser EWS qui ont une chaîne d’agent utilisateur qui commence par « OWA/ ». |
|Autorisez toutes les applications clientes à utiliser EWS. | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> Aucune application de blocage n’étant spécifiée, toutes les applications peuvent utiliser EWS. |
|Bloquer l’ensemble de l’organisation à l’aide d’EWS. | `Set-OrganizationConfig -EwsEnabled:$false` |
|Autorisez l’ensemble de l’organisation à utiliser EWS. | `Set-OrganizationConfig -EwsEnabled:$true`|
|Bloquer une boîte aux lettres individuelle à partir d’EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|Autoriser une boîte aux lettres individuelle à utiliser EWS. | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a>Voir aussi

- [Configuration de votre application EWS](setting-up-your-ews-application.md)    
- [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [Exchange Server PowerShell (environnement de commande Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

