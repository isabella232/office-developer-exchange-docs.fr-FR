---
title: Migration et les technologies Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Si vous effectuez une migration depuis une version antérieure d’Exchange, utilisez les informations de cet article pour connaître les technologies de développement sont prises en charge dans les versions actuelles des produits et technologie à migrer vers.
ms.openlocfilehash: 82362b7bcdb79d6ca43603335d51a8bd8c1df239
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755110"
---
# <a name="migrating-to-exchange-technologies"></a>Migration et les technologies Exchange

Si vous effectuez une migration depuis une version antérieure d’Exchange, utilisez les informations de cet article pour connaître les technologies de développement sont prises en charge dans les versions actuelles des produits et technologie à migrer vers.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Déterminer si la technologie est disponible dans les versions actuelles

Utilisez le tableau suivant pour déterminer si une technologie de développement est pris en charge dans Exchange Online ou Exchange 2013. Si la technologie n’est pas pris en charge, voir [Choisir une technologie de développement pour migrer vers](#bk_choose).

<br/> 

**Technologies de développement Exchange et les versions de produits**

|Technologie|Office 365 et Exchange Online|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|
|[Présentation de la plateforme Office 365 API](http://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X   <br/> ||||
|[API managée par EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Services Web Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Applications de messagerie pour Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |||
|[Modèle d’objet Outlook (insuffisante)](http://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Exchange Management Shell](management/exchange-management-shell.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Sauvegarde et restauration](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X   <br/> |X   <br/> |X   <br/> |
|[Agents de transport](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X   <br/> |X   <br/> |X   <br/> |
|Interface de Services Active Directory (ADSI)  <br/> ||||X   <br/> |
|Collaboration Data Objects pour Exchange (CDOEX)  <br/> ||||X   <br/> |
|Collaboration Data Objects pour Windows 2000 (CDOSYS)  <br/> ||||X   <br/> |
|Fournisseur OLE DB d’Exchange (EXOLEDB)  <br/> ||||X   <br/> |
|Récepteurs d’événements de banque d’informations Exchange  <br/> ||||X   <br/> |
|Synchronisation des modifications incrémentielles (ICS)  <br/> ||||X   <br/> |
|LDAP (Lightweight Directory Access Protocol)  <br/> ||||X   <br/> |
|[MAPI (Messaging API)](http://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Personnalisation d’Outlook Web App  <br/> |||X   <br/> ||
|Web distribué Authoring and Versioning (WebDAV)  <br/> ||||X   <br/> |

<a name="bk_choose"> </a>

## <a name="choose-a-development-technology-to-migrate-to"></a>Choisissez une technologie de développement pour migrer vers

Si votre application utilise la technologie de n’est pas pris en charge ou deemphasized dans Exchange Online ou Exchange 2013, utilisez le tableau suivant pour décider de la technologie pour migrer vers.
  
**Chemins de migration de technologie recommandée**

|**Technologie**|**Prise en charge dans Office 365, Exchange Online et Exchange 2013 ?**|**Migrer vers**|**Informations supplémentaires**|
|:-----|:-----|:-----|:-----|
|ADSI  <br/> |Oui, mais deemphasized <br/>|[Exchange Management Shell](management/exchange-management-shell.md)<br/> |Aucun.  <br/> |
|CDOEX  <br/> |Non  <br/> |[API managée API ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Les API managées EWS peut accéder à la même banque d’informations Exchange offrant CDOEX. Contrairement aux applications clientes créées à l’aide de CDOEX, vous pouvez exécuter des applications EWS sur un ordinateur local ou distant.  <br/> |
|CDOEXM  <br/> |Non <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Commandes Exchange Management Shell contrôlent serveurs Exchange, les groupes de stockage, les bases de données et les utilisateurs, il est plus simple que les API CDOEXM correspondant. De plus, vous pouvez facilement migrer vos applications CDOEXM aux commandes Exchange Management Shell.  <br/> |
|CDOSYS<br/> |Non<br/> |[Agents de transport](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Utilisez des agents de transport pour les applications de notification qui fonctionnent avec les versions d’Exchange commençant par Exchange 2010.<br/><br/> CDOSYS est inclus dans les versions actuelles de Windows. La fonctionnalité de CDOSYS est disponible dans .NET Framework.  <br/> |
|CDOWF  <br/> |Non  <br/> |[Windows Workflow Foundation (WWF)](http://msdn.microsoft.com/en-us/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Vous pouvez utiliser WWF pour créer des applications de flux de travail avancées qui fonctionnent avec Exchange 2007.   <br/> |
|ExOLEDB  <br/> |Non  <br/> |[API managée API ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |Les API managées EWS fournir le même accès à la banque d’informations Exchange offrant ExOLEDB. Contrairement aux applications clientes créées à l’aide de ExOLEDB, vous pouvez exécuter des applications EWS sur un ordinateur local ou distant.  <br/> |
|PARTAGE DE CONNEXION INTERNET  <br/> |Oui, mais deemphasized  <br/> |API managée API ou EWS<br/> |Vous pouvez utiliser les API managées EWS pour [vous abonner aux notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) et [synchroniser les données de boîtes aux lettres](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).  <br/> |
|LDAP  <br/> |Oui, mais deemphasized  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Aucun.  <br/> |
|MAPI  <br/> |Oui, mais deemphasized  <br/> |API plateforme présentation d’Office 365, API managées, EWS <br/> |Bien que MAPI est actuellement une technologie de développement pris en charge, vous devrez éventuellement recréer vos applications MAPI d’utiliser une nouvelle technologie.<br/><br/>Si votre application MAPI effectue simple opérations de lecture, écriture et mise à jour sur le courrier, calendrier, ou objets de contact et cibles Office 365, vous pouvez utiliser les [API de REST Office 365 pour la messagerie, des calendriers et des contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Si vous ciblez Exchange local et que vous devez accéder à toutes les propriétés MAPI peut accéder, vous pouvez utiliser l’API managée EWS ou EWS et [schématisé propriétés ou les propriétés étendues](http://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx).<br/><br/>**Remarque**: la classe [ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) fournit l’accès à MAPI à partir de l’API managée EWS et l’élément [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) permet d’accéder aux propriétés MAPI dans EWS.           |
|Personnalisation d’Outlook Web App  <br/> |Non  <br/> |[Applications de messagerie](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Aucun.  <br/> |
|Stocker les récepteurs d’événements  <br/> |Non  <br/> |API managée API ou EWS <br/> |Vous pouvez utiliser les API managées EWS pour [vous abonner aux notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) et [synchroniser les données de boîtes aux lettres](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).<br/><br/>Les notifications dans EWS fournissent le même accès à la banque d’informations Exchange que magasin de récepteurs d’événements. Vous pouvez utiliser les outils Visual Studio pour simplifier le développement d’applications client prenant en charge les événements de banque qui utilisent EWS.  <br/> |
|Diffusion en continu de sauvegarde et restauration  <br/> |Non  <br/> |[Auteur du message Volume Shadow Copy Service (VSS)](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Aucun.  <br/> |
|WebDAV  <br/> |Non  <br/> |Présentation de plateforme Office 365 API, API managées ou EWS <br/> |Si votre application WebDAV effectue simple opérations de lecture, écriture et mise à jour sur le courrier, calendrier ou objets de contact et que vous ciblez Office 365, utilisez les [API de REST Office 365 pour la messagerie, des calendriers et des contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Dans le cas contraire, si vous ciblez Exchange local et vous devez accéder aux propriétés de la banque Exchange même que WebDAV fournit, utilisez les API managées EWS.  <br/> |
|Notifications de WebDAV  <br/> |Non  <br/> |API managée API ou EWS<br/> |Vous pouvez utiliser les API managées EWS pour [vous abonner aux notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md).  <br/> |
|Formulaires Web  <br/> |Non  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Basculez vers ASP.NET et mettre à jour des applications d’accéder aux informations de boîte aux lettres et de serveur à l’aide de EWS.  <br/> |
|Fournisseurs WMI  <br/> |Non  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Aucun.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Sélection d’une API ou une technologie pour le développement de solutions pour Outlook](http://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
    

