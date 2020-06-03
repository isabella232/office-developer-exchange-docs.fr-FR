---
title: Contrôle de l'accès aux applications de client pour EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Découvrez les options permettant de gérer l’accès des applications clientes à EWS.
localization_priority: Priority
ms.openlocfilehash: b887b8167e3d38946b1d6caffe12655ded89569f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528460"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a>Contrôle de l'accès aux applications de client pour EWS dans Exchange

Découvrez les options permettant de gérer l’accès des applications clientes à EWS.
  
Toute application cliente EWS que vous créez doit disposer d’un accès à Exchange Online, Exchange Online dans le cadre d’Office 365 ou de la version d’Exchange à partir d’Exchange 2013 avant de pouvoir appeler les opérations EWS. Les administrateurs de serveurs de test ou de production peuvent utiliser l’environnement de commande Exchange Management Shell pour limiter l’accès à EWS pour tous les utilisateurs et toutes les applications, pour des utilisateurs individuels ou pour des applications individuelles. Le contrôle d’accès pour EWS est basé sur les comptes de domaine. Lorsqu’une connexion est établie avec des informations d’identification authentifiées par l’autorité de sécurité locale, le serveur renvoie une erreur qui indique que seuls les comptes de domaine peuvent se connecter. 
  
## <a name="access-control-for-ews-clients-and-users"></a>Contrôle d’accès pour les clients et les utilisateurs EWS
<a name="bk_configure"> </a>

Votre administrateur de serveur de test ou de production peut configurer le contrôle d’accès pour les clients qui se connectent à EWS de l’une des manières suivantes : 
  
- En bloquant toutes les applications clientes de se connecter.
    
- En autorisant des applications clientes spécifiques à se connecter uniquement.
    
- En autorisant toute application cliente à se connecter à l’exception de celles qui sont spécifiquement bloquées.
    
- En autorisant toute application cliente à se connecter.
    
Les applications sont identifiées par la chaîne de l’agent utilisateur qu’elles envoient dans la requête Web HTTP.
  
> [!IMPORTANT]
> Le blocage au niveau de l’application n’est pas une fonctionnalité de sécurité. La chaîne de l’agent utilisateur est facilement usurpée. Si une application est autorisée à accéder à EWS, elle doit toujours présenter les informations d’identification que le serveur authentifie avant que l’application ne puisse se connecter à EWS. 
  
Les administrateurs peuvent également configurer le contrôle d’accès pour les propriétaires de boîtes aux lettres qui se connectent à EWS de la manière suivante : 
  
- En bloquant ou en autorisant une organisation entière.
    
- En bloquant ou en autorisant un groupe d’utilisateurs identifié par une étendue d’authentification basée sur un rôle qui inclut ou exclut les propriétaires de boîtes aux lettres qui n’ont pas accès à EWS.
    
- En bloquant ou en autorisant un propriétaire de boîte aux lettres individuelle.
    
Les paramètres de contrôle d’accès spécifiques remplacent les paramètres de contrôle d’accès généraux. Par exemple, si une organisation refuse l’accès EWS mais qu’un propriétaire de boîte aux lettres individuel est autorisé à accéder aux applications, le paramètre individuel est prioritaire et l’accès est autorisé. 
  
## <a name="delegation-and-ews-access-management"></a>Délégation et gestion de l’accès EWS
<a name="bk_delegation"> </a>

Lorsque les utilisateurs délégués qui n’ont pas accès à EWS utilisent votre application cliente, ils ne pourront pas accéder à la boîte aux lettres de l’utilisateur principal à l’aide d’EWS, même si l’utilisateur principal dispose d’un accès EWS. Si l’utilisateur délégué dispose d’un accès EWS, le délégué pourra utiliser votre application cliente EWS pour accéder à la boîte aux lettres de l’utilisateur principal même si l’utilisateur principal ne dispose pas d’un accès EWS. 
  
## <a name="impersonation-and-ews-access-management"></a>Emprunt d’identité et gestion des accès EWS
<a name="bk_impersonation"> </a>

Les applications clientes qui se connectent à EWS pour le compte de propriétaires de boîtes aux lettres risquent de ne pas pouvoir utiliser les paramètres EWS du propriétaire de la boîte aux lettres. Par exemple, une application qui archive les messages électroniques d’une société doit se connecter à EWS indépendamment de ce que sont les paramètres des utilisateurs de la boîte aux lettres. D’autres applications, telles que les clients de messagerie, doivent utiliser les paramètres EWS du propriétaire de la boîte aux lettres. 
  
Les administrateurs doivent créer un compte d’emprunt d’identité pour chaque application ou classe d’application qu’ils utilisent sur leur serveur. Cela permet à l’administrateur de configurer l’étendue de contrôle d’accès basée sur un rôle pour tous les utilisateurs qui ne disposent pas d’autorisations EWS. 
  
Pour activer les comptes d’emprunt d’identité, votre administrateur de serveur de test ou de production doit effectuer l’une des opérations suivantes : 
  
- Ajoutez le groupe utilisateurs authentifiés au groupe d’accès compatible pré-Win2K. 
    
- Ajoutez le groupe serveurs Exchange au groupe d’accès d’autorisation Windows. 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a>Applets de commande Exchange Management Shell pour la gestion des accès
<a name="bk_cmdlets"> </a>

Les administrateurs utilisent les cmdlets Exchange Management Shell suivantes pour configurer les contrôles d’accès EWS : 
  
- [Get-CASMailbox](https://technet.microsoft.com/library/bb124754.aspx)   
- [Set-CASMailbox](https://technet.microsoft.com/library/bb125264.aspx)   
- [Get-OrganizationConfig](https://technet.microsoft.com/library/aa997571.aspx)   
- [Set-OrganizationConfig](https://technet.microsoft.com/library/aa997443.aspx)
    
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)  
- [Contrôler l’accès à EWS dans Exchange](how-to-control-access-to-ews-in-exchange.md)
- [Exchange Server PowerShell (environnement de commande Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

