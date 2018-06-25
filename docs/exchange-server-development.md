---
title: Exchange Online et développement Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Recherchez la documentation de développeur approfondi pour Exchange Server, notamment Exchange Online dans le cadre d’Office 365, Exchange Online, Exchange 2013, l’API managée EWS, Exchange 2010 et Exchange 2007.
ms.openlocfilehash: b933bd1bdc6dfcbe4941f23dbee9a587745c7bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754761"
---
# <a name="exchange-online-and-exchange-development"></a>Exchange Online et développement Exchange

Recherchez la documentation de développeur approfondi pour Exchange Server, notamment Exchange Online dans le cadre d’Office 365, Exchange Online, Exchange 2013, l’API managée EWS, Exchange 2010 et Exchange 2007. 

Vous pouvez utiliser la procédure, prise en main, nouvelle fonctionnalité, et la documentation de référence API pour développer des outils pour accéder et gérer les données de boîtes aux lettres à partir des services, les sites Web, les ordinateurs de bureau et les appareils mobiles et à créer des solutions personnalisées pour le courrier électronique, calendrier, contacts, et autres éléments qui sont stockés dans Exchange Online ou sur un serveur Exchange 2013. 

Vous pouvez utiliser Exchange Web Services (EWS), découverte automatique, les applications de messagerie pour Office ou d’autres API pour développer vos applications. Cette page vous permet de choisir la technologie Exchange de droite.

## <a name="exchange-developer-content"></a>Pour les développeurs Exchange contenu  

Utilisez le tableau suivant pour identifier la technologie et le contenu d’API qui vous aideront à atteindre vos objectifs de développement.  
  
|Si vous créez...|Démarrez ici|
|:-----|:-----|
|Une application basée sur REST pour accéder à Exchange Online dans le cadre d’Office 365|[API REST Office 365 pour la messagerie, les calendriers et les contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Une application contextuelle pour afficher des informations dans Outlook, Outlook Web App ou OWA pour périphériques |[Applications de messagerie pour Outlook et EWS dans Exchange](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|Un client de boîte aux lettres qui n’est pas basé sur le .NET Framework ou Java |[Explorer l'API managée EWS, EWS et les services web dans Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|Un client de boîte aux lettres qui utilise le .NET Framework pour accéder à EWS |[Prise en main des applications clientes d'API managée EWS](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|Un client de boîte aux lettres qui utilise Java pour accéder à EWS |[API de Java EWS sur les référentiels](https://github.com/OfficeDev/ews-java-api) |
|Une application qui personnalise l’interface utilisateur Outlook ou repose sur la logique métier d’Outlook  |[Référence VBA Outlook](https://msdn.microsoft.com/en-us/VBA/VBA-Outlook) |
|Une application qui cible Exchange Online ou Exchange 2013 dont vous avez besoin pour migrer depuis une version antérieure d’Exchange  |[Migration et les technologies Exchange](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|Un outil de gestion personnalisée qui utilise Windows PowerShell à partir du code managé   |[Exchange Management Shell](management/exchange-management-shell.md) |
|Une solution pour sauvegarder ou restaurer des données Exchange  |[Sauvegarde et restauration pour Exchange](backup-restore/backup-and-restore-for-exchange-2013.md) |
|Une extension pour prendre en charge l’accès aux messages dans le pipeline de transport   |[Agents de transport dans Exchange](transport-agents/transport-agents-in-exchange-2013.md)  |
|Un client de boîte aux lettres pour un appareil mobile   |[Exchange ActiveSync](https://technet.microsoft.com/en-us/library/aa998357.aspx) |
   
## <a name="exchange-interactions-with-custom-applications"></a>Interactions d’Exchange avec les applications personnalisées

Certaines de ces technologies permettent à vos applications travailler avec les données stockées dans Exchange, et d’autres personnes sont utilisés pour gérer et contrôler le serveur Exchange. Dans de nombreux cas, vous pouvez utiliser plusieurs technologie ou langage de programmation pour accomplir une tâche, ce qui rend possible d’utiliser les technologies et les langues que vous connaissez. Par exemple, vous pouvez définir des propriétés sur des éléments de la banque d’informations Exchange à l’aide de l’API REST de messagerie, EWS ou l’API managée EWS.
  
Exchange interagit avec les applications personnalisées de diverses manières, en fonction de l’architecture d’application et les fonctionnalités. Fondamentalement, Exchange non seulement les transports de messages, mais gère également les boîtes aux lettres, exécute les applications basées sur un formulaire et bien plus encore.

|Interaction Exchange|Description|
|:-----|:-----|
|**Transport des messages**|Exchange sert à un serveur de messagerie standard pour les applications qui envoient des messages.<br/>Exchange inclut plusieurs API transférer les messages, y compris REST et les API managées EWS.<br/>En outre, les applications peuvent utiliser des agents de transport pour répondre comme messages sont traitées et remis par Exchange. |
|**Stockage de boîtes aux lettres** |Exchange fournit une structure hiérarchique de dossiers, des éléments et des propriétés pour les applications qui accèdent aux données stockées dans les boîtes aux lettres.<br/>Vous pouvez accéder à ces informations stockées à l’aide d’une combinaison de styles d’objet de base de données et le composant.<br/>Vous pouvez exécuter des requêtes sur les données et Exchange gère l’accès aux données stockées en fonction des autorisations utilisateur et de la banque.<br/>Les applications qui prennent en charge les données de boîtes aux lettres généralement utilisent REST, EWS ou l’API managée EWS.|
|**Serveur d’entreprise gérées** |Exchange fonctionne comme un serveur géré pour les applications qui gèrent les banques et les serveurs Exchange.<br/>Les applications peuvent configurer, contrôler et surveiller l’intégrité des serveurs Exchange et l’activité en cours dans l’organisation.<br/>Applications de gestion Exchange utilisent Exchange Management Shell pour gérer des serveurs Exchange. |
   
## <a name="see-also"></a>Voir aussi

- [Référence des API du serveur pour Exchange](https://msdn.microsoft.com/en-us/library/dn186243(v=exchg.150).aspx)
- [En savoir plus sur Exchange sur des Blogs Office](https://www.microsoft.com/en-us/microsoft-365/blog/) 
- [Obtenir les 101 exemples de code pour Exchange 2013](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [Obtenir l’API managée EWS (référentiels)](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Obtenir la prise en charge pour Exchange Server](https://support.microsoft.com/en-us/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)


