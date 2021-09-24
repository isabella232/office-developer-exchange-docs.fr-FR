---
title: Migration vers les technologies Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Si vous migrez à partir d’une version antérieure de Exchange, utilisez les informations de cet article pour connaître les technologies de développement qui sont pris en charge dans les versions actuelles du produit et la technologie vers laquelle migrer.
ms.openlocfilehash: 3885d6789cedf5de028b64a0658b336bd021b9ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527000"
---
# <a name="migrating-to-exchange-technologies"></a>Migration vers les technologies Exchange

Si vous migrez à partir d’une version antérieure de Exchange, utilisez les informations de cet article pour connaître les technologies de développement qui sont pris en charge dans les versions actuelles du produit et la technologie vers laquelle migrer.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Déterminer si votre technologie est disponible dans les versions actuelles

Utilisez le tableau suivant pour déterminer si une technologie de développement est prise en charge dans Exchange Online ou Exchange 2019. Si la technologie n’est pas prise en charge, voir [Choisir une technologie de développement vers qui migrer.](#bk_choose)

<br/> 

**Exchange technologies de développement et versions de produits**

|Technologie|Office 365 et Exchange Online|Exchange 2019|Exchange 2016|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|[Présentation de la plateforme des API Office 365](https://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> |X²  <br/> |X¹ ²  <br/> ||
|[API managée EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Services Web Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Applications de messagerie pour Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Outlook Modèle objet (OOM)](https://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange Management Shell](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Sauvegarde et restauration](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Agents de transport](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Interface ADSI (Active Directory Services Interface)  <br/> ||||||X  <br/> |
|Collaborative Data Objects for Exchange (CDOEX)  <br/> ||||||X  <br/> |
|Collaborative Data Objects for Windows 2000 (CDOSYS)  <br/> ||||||X  <br/> |
|Exchange Fournisseur OLE DB (EXOLEDB)  <br/> ||||||X  <br/> |
|Exchange Store Event Sinks  <br/> ||||||X  <br/> |
|Synchronisation incrémentielle des changements (ICS)  <br/> ||||||X  <br/> |
|Protocole LDAP (Lightweight Directory Access Protocol)  <br/> ||||||X  <br/> |
|[API de messagerie (MAPI)](https://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> | 
|Outlook Personnalisation de Web App  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Web Distributed Authoring and Versioning (WebDAV)  <br/> ||||||X  <br/> |

<a name="bk_choose"> </a>

L’API ¹REST et Graph API de base nécessitent la mise à jour cumulative 3 Exchange 2016.

²Only hybrid customers are able to take advantage of the REST APIs for both Office 365 and on-premises mailboxes.

## <a name="choose-a-development-technology-to-migrate-to"></a>Choisir une technologie de développement vers qui migrer

Si la technologie utilisée par votre application n’est pas prise en charge ou déphasée dans Exchange Online ou Exchange 2013, utilisez le tableau suivant pour déterminer la technologie vers laquelle migrer.
  
**Chemins de migration de technologie recommandés**

|**Technologie**|**Pris en charge Office 365, Exchange Online et Exchange 2019 ?**|**Migrer vers**|**Plus d’informations**|
|:-----|:-----|:-----|:-----|
|ADSI  <br/> |Oui, mais deemphasized <br/>|[Exchange Management Shell](management/exchange-management-shell.md)<br/> |Aucun.  <br/> |
|CDOEX  <br/> |Non  <br/> |[API gérée EWS ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |L’API gérée EWS et EWS peuvent accéder au même magasin Exchange que CDOEX fournit. Contrairement aux applications clientes conçues à l’aide de CDOEX, vous pouvez exécuter des applications EWS sur un ordinateur local ou distant.  <br/> |
|CDOEXM  <br/> |Non <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Exchange Les commandes management Shell contrôlent Exchange serveurs, groupes de stockage, bases de données et utilisateurs plus simplement que les API CDOEXM correspondantes. De plus, vous pouvez facilement migrer vos applications CDOEXM vers Exchange commandes management Shell.  <br/> |
|CDOSYS<br/> |Non<br/> |[Agents de transport](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Utilisez des agents de transport pour les applications basées sur les notifications qui fonctionnent avec les versions de Exchange à partir Exchange 2010.<br/><br/> CDOSYS est inclus dans les versions actuelles de Windows. La fonctionnalité de CDOSYS est disponible dans le .NET Framework.  <br/> |
|CDOWF  <br/> |Non  <br/> |[Windows Workflow Foundation (WWF)](https://msdn.microsoft.com/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Vous pouvez utiliser WWF pour créer des applications de flux de travail avancées qui fonctionnent avec Exchange 2007.   <br/> |
|ExOLEDB  <br/> |Non  <br/> |[API gérée EWS ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |L’API gérée EWS et EWS fournissent le même accès au magasin Exchange que celui fourni par ExOLEDB. Contrairement aux applications clientes conçues à l’aide d’ExOLEDB, vous pouvez exécuter des applications EWS sur un ordinateur local ou distant.  <br/> |
|ICS  <br/> |Oui, mais deemphasized  <br/> |API gérée EWS ou EWS<br/> |Vous pouvez utiliser l’API gérée EWS ou EWS pour vous abonner aux [notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) et synchroniser [les données de boîte aux lettres.](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)  <br/> |
|LDAP  <br/> |Oui, mais deemphasized  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Aucun.  <br/> |
|MAPI  <br/> |Oui, mais deemphasized  <br/> |Office 365 Vue d’ensemble de la plateforme api, API gérée EWS, EWS <br/> |Bien que MAPI soit actuellement une technologie de développement prise en charge, vous de aurez à redéfinir vos applications MAPI pour utiliser une technologie plus récente.<br/><br/>Si votre application MAPI effectue des opérations simples de lecture, d’écriture et de mise à jour sur des objets de messagerie, de calendrier ou de contact, et cible Office 365, Exchange 2019² ou Exchange 2016¹ ², vous pouvez utiliser les API REST Office 365 pour la messagerie, les calendriers et les [contacts.](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)<br/><br/>Si vous ciblez Exchange en local et que vous devez accéder à toutes les propriétés accessibles par MAPI, [](https://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx)vous pouvez utiliser l’API gérée EWS ou EWS et les propriétés schématisées ou étendues.<br/><br/>**REMARQUE**: la classe [ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) fournit l’accès à MAPI à partir de l’API gérée EWS, et l’élément [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) fournit l’accès aux propriétés MAPI à partir d’EWS.           |
|Outlook Personnalisation de Web App  <br/> |Non  <br/> |[Applications de messagerie](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Aucun.  <br/> |
|Store event sinks  <br/> |Non  <br/> |API gérée EWS ou EWS <br/> |Vous pouvez utiliser l’API gérée EWS ou EWS pour vous abonner aux [notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) et synchroniser [les données de boîte aux lettres.](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)<br/><br/>Les notifications dans EWS fournissent le même accès au magasin Exchange que les réceptions d’événements de magasin fournissent. Vous pouvez utiliser Visual Studio pour simplifier le développement d’applications clientes sensibles aux événements du store qui utilisent EWS.  <br/> |
|Sauvegarde et restauration en continu  <br/> |Non  <br/> |[Rédacteur vsS (Volume Shadow Copy Service)](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Aucun.  <br/> |
|WebDAV  <br/> |Non  <br/> |Office 365 Vue d’ensemble de la plateforme API, API gérée EWS ou EWS <br/> |Si votre application WebDAV effectue des opérations simples de lecture, d’écriture et de mise à jour sur des objets de messagerie, de calendrier ou de contact, et que vous ciblez Office 365, Exchange 2019² ou Exchange 2016¹ ², vous pouvez utiliser les API REST Office 365 pour le courrier, les calendriers et les [contacts.](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)<br/><br/>Dans le cas contraire, si vous ciblez Exchange en local et que vous avez besoin d’accéder aux mêmes propriétés dans le magasin Exchange que webDAV fournit, utilisez l’API gérée EWS ou EWS.  <br/> |
|Notifications WebDAV  <br/> |Non  <br/> |API gérée EWS ou EWS<br/> |Vous pouvez utiliser l’API gérée EWS ou EWS pour vous [abonner aux notifications.](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)  <br/> |
|Formulaires Web  <br/> |Non  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Basculez vers ASP.NET et mettez à jour les applications pour accéder aux informations de boîte aux lettres et de serveur à l’aide d’EWS.  <br/> |
|Fournisseurs WMI  <br/> |Non  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Aucun.  <br/> |
   
L’API ¹REST et Graph API de base nécessitent la mise à jour cumulative 3 Exchange 2016.

²Only hybrid customers are able to take advantage of the REST APIs for both Office 365 and on-premises mailboxes.

## <a name="see-also"></a>Voir aussi

- [Sélection d’une API ou d’une technologie pour le développement de solutions pour Outlook](https://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
- [Exigences en matière d’architecture locale pour l’API REST](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)    
