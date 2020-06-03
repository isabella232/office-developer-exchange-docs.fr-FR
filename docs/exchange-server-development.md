---
title: Développement Exchange Online et Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Recherchez une documentation développeur détaillée pour Exchange Server, notamment Exchange Online dans le cadre des versions locales d’Office 365 et d’Exchange Server.
localization_priority: Priority
ms.openlocfilehash: 12a29ca07801561e7a746603d795468d9cb7491f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528495"
---
# <a name="exchange-online-and-exchange-development"></a>Développement Exchange Online et Exchange

Recherchez une documentation développeur détaillée pour Exchange Server, notamment Exchange Online dans le cadre des versions locales d’Office 365 et d’Exchange Server.

Vous pouvez utiliser la documentation de référence sur les procédures, la fonctionnalité de démarrage, la nouvelle fonctionnalité et l’API pour développer des outils permettant d’accéder aux données de boîtes aux lettres et de les gérer à partir de services, de sites Web, d’ordinateurs de bureau et de périphériques mobiles, et de créer des solutions personnalisées pour la messagerie, 2016 2013 2010 le calendrier, les contacts et les serveurs 2019.

Vous pouvez utiliser l’API Graph, l’API REST, les services Web Exchange (EWS), la découverte automatique, les compléments Outlook ou d’autres API pour développer vos applications. Cette page vous permet de choisir la technologie Exchange adaptée.

## <a name="exchange-developer-content"></a>Contenu de développeur Exchange

Utilisez le tableau suivant pour identifier la technologie et le contenu API associé qui vous permettront d’atteindre vos objectifs de développement.

> [!IMPORTANT]
> Microsoft Graph est l’API recommandée à utiliser pour accéder aux données Exchange Online. Les nouvelles applications conçues pour accéder aux données Exchange Online doivent utiliser Microsoft Graph.

|Si vous créez...|Démarrez ici|
|:-----|:-----|
|Une application basée sur REST pour accéder à Exchange Online comme composant d’Office 365|[API REST Microsoft Graph pour la messagerie, les calendriers et les contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Une application contextuelle pour afficher des informations dans Outlook, Outlook Web App ou OWA pour les Appareils |[Compléments Outlook et EWS dans Exchange](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|Un client de boîte aux lettres qui n’est pas basé sur .NET Framework ou Java. |[Explorer l'API managée EWS, l’EWS et les services web dans Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|Un client de boîte aux lettres qui utilise .NET Framework pour accéder à EWS |[Prise en main des applications clientes d'API managée EWS](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|Un client de boîte aux lettres qui utilise Java pour accéder à EWS. |[API Java EWS sur GitHub](https://github.com/OfficeDev/ews-java-api) |
|Une application qui personnalise l’interface utilisateur d’Outlook ou s’appuie sur la logique métier d’Outlook.  |[Référence VBA Outlook](https://msdn.microsoft.com/VBA/VBA-Outlook) |
|Une application qui cible Exchange Online ou Exchange 2013 et avec laquelle vous devez migrer depuis une version antérieure d’Exchange.  |[Migration vers les technologies Exchange](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|Un outil de gestion personnalisée qui utilise Windows PowerShell à partir du code managé.   |[Exchange Management Shell](management/exchange-management-shell.md) |
|Une solution pour sauvegarder ou restaurer des données Exchange  |[Sauvegarde et restauration pour Exchange](backup-restore/backup-and-restore-for-exchange-2013.md) |
|Une extension pour la prise en charge de l’accès aux messages dans le pipeline de transport.   |[Agents de transport dans Exchange](transport-agents/transport-agents-in-exchange-2013.md)  |
|Un client de boîte aux lettres pour un périphérique mobile   |[Exchange ActiveSync](https://technet.microsoft.com/library/aa998357.aspx) |

## <a name="exchange-interactions-with-custom-applications"></a>Interactions Exchange avec les applications personnalisées

Certaines de ces technologies permettent à vos applications d’utiliser des données stockées dans Exchange et d’autres sont utilisées pour gérer et contrôler le serveur Exchange. Dans de nombreux cas, vous pouvez utiliser plusieurs technologies ou langages de programmation pour accomplir une tâche, ce qui vous permet d’utiliser les technologies et langages avec lesquels vous êtes le plus à l’aise. Par exemple, vous pouvez définir des propriétés sur des éléments dans la banque d’informations Exchange à l’aide de l’API REST Courrier, EWS ou l’API managée EWS.

Exchange interagit avec les applications personnalisées de différentes manières, en fonction de l’architecture et les fonctionnalités de l’application. Concrètement, Exchange ne transporte pas seulement des messages mais met également à jour les boîtes aux lettres, exécute des applications basées sur des formulaires et bien plus encore.

|Interaction Exchange|Description|
|:-----|:-----|
|**Transport des messages**|Exchange sert de serveur de courrier classique pour les applications qui envoient des messages.<br/>Exchange inclut plusieurs API qui transfèrent les messages, notamment les API REST, EWS et l’API managée EWS.<br/>En outre, les applications peuvent utiliser les agents de transport pour répondre tandis que les messages sont traités et remis par Exchange. |
|**Stockage de boîtes aux lettres** |Exchange présente une structure hiérarchique des dossiers, éléments et propriétés pour les applications qui accèdent aux données stockées dans les boîtes aux lettres.<br/>Vous pouvez accéder à ces informations stockées en utilisant une combinaison de styles d’objet de base de données et de composant.<br/>Vous pouvez effectuer des requêtes sur les données et Exchange gère l’accès aux données stockées en fonction des autorisations utilisateur et de stockage.<br/>Les applications qui traitent les données de boîte aux lettres utilisent généralement les API REST, EWS ou l’API managée EWS.|
|**Serveur d'entreprise Exchange** |Exchange fonctionne comme un serveur géré pour les applications qui gèrent les serveurs et banques Exchange.<br/>Les applications peuvent configurer, contrôler et surveiller l’activité en cours et l’état des serveurs Exchange au sein de l’organisation.<br/>Les applications de gestion Exchange utilisent l’environnement de ligne de commande Exchange Management Shell pour gérer les serveurs Exchange. |

## <a name="see-also"></a>Voir aussi

- 
  [Référence de l’API serveur pour Exchange](https://msdn.microsoft.com/library/dn186243(v=exchg.150).aspx)
- [En savoir plus sur Exchange sur les Blogs Office](https://www.microsoft.com/microsoft-365/blog/)
- [Obtenez des exemples de code pour Exchange 2013 en guise d’initiation](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [Obtenez l’API managée EWS (GitHub)](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Obtenez une assistance pour le serveur Exchange](https://support.microsoft.com/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)
