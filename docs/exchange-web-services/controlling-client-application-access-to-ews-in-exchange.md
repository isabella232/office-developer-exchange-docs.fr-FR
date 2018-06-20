---
title: Contrôle de l’accès aux applications de client pour EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: Découvrez les options de gestion des accès aux applications de client à EWS.
ms.openlocfilehash: 29a640178afc9814a0b2232225ae4307e49afed2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754764"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a>Contrôle de l’accès aux applications de client pour EWS dans Exchange

Découvrez les options de gestion des accès aux applications de client à EWS.
  
N’importe quelle application client EWS que vous créez doit avoir accès à Exchange Online, Exchange Online dans le cadre d’Office 365, ou une version d’Exchange, commençant par Exchange 2013 avant de pouvoir appeler des opérations EWS. Administrateurs de serveur de test ou de production peuvent utiliser Exchange Management Shell pour limiter l’accès à EWS pour tous les utilisateurs et des applications, pour des utilisateurs individuels ou pour des applications individuelles. Contrôle d’accès pour EWS est basé sur les comptes de domaine. Lorsqu’une connexion est établie avec les informations d’identification qui sont authentifiées par l’autorité de sécurité locale, le serveur renvoie une erreur indiquant que seuls les comptes de domaine peuvent se connecter. 
  
## <a name="access-control-for-ews-clients-and-users"></a>Contrôle d’accès pour les utilisateurs et les clients EWS
<a name="bk_configure"> </a>

Votre administrateur de serveur de test ou de production permettre configurer le contrôle d’accès pour les clients qui se connectent à EWS comme suit : 
  
- En bloquant toutes les applications clientes de se connecter.
    
- Par ainsi que pour la connexion client spécifique.
    
- En autorisant n’importe quelle application client à se connecter à l’exception de ceux qui sont spécifiquement bloqués.
    
- En autorisant n’importe quelle application client à se connecter.
    
Les applications sont identifiées par la chaîne d’agent utilisateur qu’ils envoient dans la requête web HTTP.
  
> [! Remarque sur la sécurité] niveau Application blocage n’est pas une fonctionnalité de sécurité. La chaîne d’agent utilisateur est facilement usurpée. Si une application est autorisée à accéder à EWS, l’application doit toujours présenter des informations d’identification que le serveur authentifie avant de l’application peut se connecter à EWS. 
  
Les administrateurs peuvent configurer également le contrôle d’accès pour les propriétaires de boîte aux lettres qui se connectent à EWS comme suit : 
  
- Bloquer ou autoriser un ensemble de l’organisation.
    
- Bloquer ou autoriser un groupe d’utilisateurs identifié par une étendue de l’authentification basée sur les rôles qui inclut ou exclut les propriétaires de boîte aux lettres qui n’ont pas accès à EWS.
    
- Bloquer ou autoriser un propriétaire de boîte aux lettres.
    
Paramètres de contrôle d’accès spécifiques remplacent les paramètres de contrôle d’accès général. Par exemple, si une organisation refuse l’accès EWS, mais un propriétaire de boîte aux lettres est autorisé l’accès de l’application, le paramètre prévaut et l’accès est autorisé. 
  
## <a name="delegation-and-ews-access-management"></a>Délégation et gestion des accès EWS
<a name="bk_delegation"> </a>

Lorsque les utilisateurs délégués qui n’ont pas accès à EWS utiliser votre application cliente, ils ne pourront accéder aux boîtes aux lettres de l’utilisateur principal à l’aide de EWS, même si l’utilisateur principal a EWS accéder. Si l’utilisateur délégué dispose d’un accès EWS, le délégué sera en mesure d’utiliser votre application de client EWS pour accéder aux boîtes aux lettres de l’utilisateur principal, même si l’utilisateur principal n’a pas EWS access. 
  
## <a name="impersonation-and-ews-access-management"></a>Emprunt d’identité et de gestion de l’accès EWS
<a name="bk_impersonation"> </a>

Applications clientes qui se connectent à EWS part propriétaires de boîte aux lettres ne peuvent pas être en mesure d’utiliser les paramètres EWS du propriétaire de boîte aux lettres. Par exemple, une application qui archive les e-mails les messages pour une société a pour se connecter à EWS indépendamment des paramètres de rôle la boîte aux lettres des utilisateurs sont. Autres applications, telles que les clients de messagerie, n’ont pas à utiliser les paramètres de EWS du propriétaire de la boîte aux lettres. 
  
Les administrateurs doivent créer un compte d’emprunt d’identité pour chaque application ou une classe d’application qu’ils utilisent sur leur serveur. Cela permettra à l’administrateur de configurer l’étendue de contrôle d’accès basé sur un rôle pour tous les utilisateurs qui n’ont pas d’autorisations EWS. 
  
Pour activer des comptes d’emprunt d’identité, votre administrateur de serveur de test ou de production doit effectuer une des options suivantes : 
  
- Ajoutez le groupe utilisateurs authentifiés au groupe accès Compatible pré-Win2K. 
    
- Ajoutez le groupe de serveurs Exchange pour le groupe d’accès d’autorisation Windows. 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a>Applets de commande Exchange Management Shell pour la gestion des accès
<a name="bk_cmdlets"> </a>

Les administrateurs utiliser les applets de commande Exchange Management Shell suivante pour configurer les contrôles d’accès EWS : 
  
- [Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx)
    
- [Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx)
    
- [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx)
    
- [Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx)
    
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)  
- [Contrôler l’accès à EWS dans Exchange](how-to-control-access-to-ews-in-exchange.md)
- [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

