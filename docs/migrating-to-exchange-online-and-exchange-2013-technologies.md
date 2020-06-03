---
title: Migration vers les technologies Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Si vous effectuez une migration à partir d’une version antérieure d’Exchange, utilisez les informations contenues dans cet article pour savoir quelles technologies de développement sont prises en charge dans les versions actuelles du produit, ainsi que la technologie vers laquelle effectuer la migration.
ms.openlocfilehash: d82f1b305fd1cc30e48cddbf9bf2981d3d829a5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459152"
---
# <a name="migrating-to-exchange-technologies"></a>Migration vers les technologies Exchange

Si vous effectuez une migration à partir d’une version antérieure d’Exchange, utilisez les informations contenues dans cet article pour savoir quelles technologies de développement sont prises en charge dans les versions actuelles du produit, ainsi que la technologie vers laquelle effectuer la migration.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Déterminer si votre technologie est disponible dans les versions actuelles

Utilisez le tableau suivant pour déterminer si une technologie de développement est prise en charge dans Exchange Online ou Exchange 2019. Si la technologie n’est pas prise en charge, consultez la rubrique [Choose a Development Technology to migrate](#bk_choose).

<br/> 

**Technologies de développement Exchange et versions du produit**

|Technology|Office 365 et Exchange Online|Exchange 2019|Exchange 2016|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|[Présentation de la plateforme des API Office 365](https://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> |X ²  <br/> |X ¹ ²  <br/> ||
|[API managée EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Services Web Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Applications de messagerie pour Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Modèle objet Outlook (OOM)](https://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange Management Shell](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Sauvegarde et restauration](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Agents de transport](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Interface ADSI (Active Directory Services Interface)  <br/> ||||||X  <br/> |
|CDO (Collaboration Data Objects)  <br/> ||||||X  <br/> |
|CDO (Collaboration Data Objects) pour Windows 2000 (CDOSYS)  <br/> ||||||X  <br/> |
|Fournisseur OLE DB Exchange (EXOLEDB)  <br/> ||||||X  <br/> |
|Récepteurs d’événements de la banque Exchange  <br/> ||||||X  <br/> |
|Synchronisation des modifications incrémentielles (ICS)  <br/> ||||||X  <br/> |
|Protocole LDAP (Lightweight Directory Access Protocol)  <br/> ||||||X  <br/> |
|[API de messagerie (MAPI)](https://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> | 
|Personnalisation d’Outlook Web App  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Web Distributed Authoring and Versioning (WebDAV)  <br/> ||||||X  <br/> |

<a name="bk_choose"> </a>

¹ l’API REST et l’API Graph requièrent la mise à jour cumulative 3 pour Exchange 2016.

² seuls les clients hybrides peuvent tirer parti des API REST pour Office 365 et les boîtes aux lettres locales.

## <a name="choose-a-development-technology-to-migrate-to"></a>Choisir une technologie de développement vers laquelle effectuer la migration

Si la technologie utilisée par votre application n’est pas prise en charge ou déplacée dans Exchange Online ou Exchange 2013, utilisez le tableau suivant pour déterminer la technologie à migrer.
  
**Chemins de migration de technologies recommandés**

|**Technology**|**Prise en charge dans Office 365, Exchange Online et Exchange 2019 ?**|**Migrer vers**|**Plus d’informations**|
|:-----|:-----|:-----|:-----|
|ASDI  <br/> |Oui, mais désouligné <br/>|[Exchange Management Shell](management/exchange-management-shell.md)<br/> |Aucun.  <br/> |
|CDOEX  <br/> |Non  <br/> |[API managée EWS ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |L’API managée EWS et EWS peut accéder à la même banque d’Exchange que celle fournie par CDOEX. Contrairement aux applications clientes créées à l’aide de CDOEX, vous pouvez exécuter des applications EWS sur un ordinateur local ou distant.  <br/> |
|CDOEXM  <br/> |Non <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Les commandes de l’environnement de commande Exchange Management Shell contrôlent les serveurs Exchange, les groupes de stockage, les bases de données et les utilisateurs plus simplement que les API CDOEXM correspondantes. En outre, vous pouvez facilement migrer vos applications CDOEXM vers les commandes Exchange Management Shell.  <br/> |
|CDOSYS<br/> |Non<br/> |[Agents de transport](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Utilisez des agents de transport pour les applications basées sur des notifications qui fonctionnent avec les versions d’Exchange à partir d’Exchange 2010.<br/><br/> CDOSYS est inclus dans les versions actuelles de Windows. La fonctionnalité de CDOSYS est disponible dans .NET Framework.  <br/> |
|CDOWF  <br/> |Non  <br/> |[Windows Workflow Foundation (WWF)](https://msdn.microsoft.com/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Vous pouvez utiliser WWF pour créer des applications de flux de travail avancées qui fonctionnent avec Exchange 2007.   <br/> |
|ExOLEDB  <br/> |Non  <br/> |[API managée EWS ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |L’API managée EWS et EWS fournissent le même accès à la Banque d’Exchange que ExOLEDB fournit. Contrairement aux applications clientes créées à l’aide de ExOLEDB, vous pouvez exécuter des applications EWS sur un ordinateur local ou distant.  <br/> |
|DÛMENT  <br/> |Oui, mais désouligné  <br/> |API managée EWS ou EWS<br/> |Vous pouvez utiliser l’API managée EWS ou EWS pour vous [abonner aux notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) et [synchroniser les données de boîte aux lettres](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).  <br/> |
|LDAP  <br/> |Oui, mais désouligné  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Aucun.  <br/> |
|MAPI  <br/> |Oui, mais désouligné  <br/> |Vue d’ensemble de la plateforme des API Office 365, API managée EWS, EWS <br/> |Bien que MAPI soit actuellement une technologie de développement prise en charge, vous devrez éventuellement reconcevoir vos applications MAPI pour utiliser une technologie plus récente.<br/><br/>Si votre application MAPI effectue des opérations simples de lecture, d’écriture et de mise à jour sur des objets de courrier, de calendrier ou de contact, et des cibles Office 365, Exchange 2019 ² ou Exchange 2016 ¹ ², vous pouvez utiliser les [API REST office 365 pour le courrier, les calendriers et les contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Si vous ciblez Exchange en local et que vous avez besoin d’accéder à toutes les propriétés auxquelles MAPI peut accéder, vous pouvez utiliser l’API managée EWS ou EWS, ainsi que les [propriétés étendues ou schématisées](https://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx).<br/><br/>**Remarque**: la classe [ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) fournit l’accès à MAPI à partir de l’API managée EWS, et l’élément [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) fournit l’accès aux propriétés MAPI à partir d’EWS.           |
|Personnalisation d’Outlook Web App  <br/> |Non  <br/> |[Applications de messagerie](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Aucun.  <br/> |
|Récepteurs d’événements de banque  <br/> |Non  <br/> |API managée EWS ou EWS <br/> |Vous pouvez utiliser l’API managée EWS ou EWS pour vous [abonner aux notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) et [synchroniser les données de boîte aux lettres](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).<br/><br/>Les notifications dans EWS fournissent le même accès à la Banque d’Exchange que celle fournie par les récepteurs d’événements. Vous pouvez utiliser les outils Visual Studio pour simplifier le développement d’applications clientes prenant en charge les événements de magasin qui utilisent EWS.  <br/> |
|Sauvegarde et restauration en continu  <br/> |Non  <br/> |[Enregistreur VSS (Volume Shadow Copy Service)](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Aucun.  <br/> |
|Référentiel  <br/> |Non  <br/> |Vue d’ensemble de la plateforme des API Office 365, API managée EWS ou EWS <br/> |Si votre application WebDAV effectue des opérations de lecture, d’écriture et de mise à jour simples sur des objets de courrier, de calendrier ou de contact, et que vous ciblez Office 365, Exchange 2019 ² ou Exchange 2016 ¹ ², vous pouvez utiliser les [API REST office 365 pour le courrier, les calendriers et les contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Dans le cas contraire, si vous ciblez Exchange en local et que vous avez besoin d’accéder aux mêmes propriétés dans la banque Exchange que fournit WebDAV, utilisez l’API managée EWS ou EWS.  <br/> |
|Notifications WebDAV  <br/> |Non  <br/> |API managée EWS ou EWS<br/> |Vous pouvez utiliser l’API managée EWS ou EWS pour vous [abonner aux notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md).  <br/> |
|Formulaires Web  <br/> |Non  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Basculez vers ASP.NET et mettre à jour les applications pour accéder aux informations de boîte aux lettres et de serveur à l’aide d’EWS.  <br/> |
|Fournisseurs WMI  <br/> |Non  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Aucun.  <br/> |
   
¹ l’API REST et l’API Graph requièrent la mise à jour cumulative 3 pour Exchange 2016.

² seuls les clients hybrides peuvent tirer parti des API REST pour Office 365 et les boîtes aux lettres locales.

## <a name="see-also"></a>Voir aussi

- [Sélection d’une API ou d’une technologie pour le développement de solutions pour Outlook](https://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
- [Exigences en matière d’architecture locale pour l’API REST](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)    
