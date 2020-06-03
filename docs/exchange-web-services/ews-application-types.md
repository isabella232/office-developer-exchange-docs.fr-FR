---
title: Types d'applications EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: ca4e8b90-d0d8-4d55-aa92-19e21659d4f5
description: Découvrez les principaux types d’applications que vous pouvez créer à l’aide des services web Exchange dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 02bbe039adaec1054ab33f642f3bf14a7ba22b90
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455428"
---
# <a name="ews-application-types"></a>Types d'applications EWS

Découvrez les principaux types d’applications que vous pouvez créer à l’aide des services web Exchange dans Exchange.
  
L' [architecture EWS et Exchange](ews-applications-and-the-exchange-architecture.md) fournit un modèle de développement uniforme que vous pouvez utiliser pour créer les types d’applications les plus courants de manière cohérente, notamment les suivantes : 
  
- [Applications clientes](#bk_clientapps) — applications autonomes qui utilisent EWS pour accéder aux données Exchange. Outlook et Outlook Web App sont des exemples d’applications clientes. 
    
- [Applications de portail](#bk_portalapps) : applications qui étendent une page Web existante en incluant des informations extraites d’Exchange, telles que la disponibilité ou les informations de contact. Un composant WebPart SharePoint qui récupère les données Exchange est un exemple d’application de portail. 
    
- [Applications de service](#bk_serviceapps) : travaux d’arrière-plan utilisés pour intégrer ou synchroniser des données à partir d’Exchange dans un système existant. Par exemple, une application qui synchronise les informations de contact à partir d’Exchange dans une application CRM. 
    
Chacun de ces modèles d’application peut utiliser une base de code commune pour récupérer des informations à partir d’Exchange, de sorte que vous n’avez pas besoin de modifier le code EWS utilisé pour extraire les informations d’élément entre un client, un portail ou une application de service. Ce qui peut changer d’une application à la suivante est le mécanisme d’authentification et d’accès aux boîtes aux lettres. Par exemple, les applications clientes utilisent généralement l’authentification directe par les utilisateurs et l’authentification de base ou NTLM, tandis qu’une application de service utilise vraisemblablement l’emprunt d’identité pour l’accès aux boîtes aux lettres et l’authentification OAuth.
  
## <a name="client-applications"></a>Applications clientes
<a name="bk_clientapps"> </a>

Une application cliente EWS est une application autonome qui utilise EWS pour extraire des informations de la Banque d’informations Exchange. Les applications clientes EWS utilisent un accès direct au client ou un accès délégué pour extraire les données de la Banque de boîtes aux lettres. Voici quelques exemples d’applications clientes qui utilisent EWS :
  
- Outlook, dans les fonctionnalités telles que les infos-courrier, la disponibilité et l’état de l’utilisateur absent
    
- OWA pour les périphériques
    
- Outlook pour Mac 2011
    
- Lync, pour les informations de disponibilité
    
Les applications clientes utilisent couramment l’accès direct et l’authentification de base ou NTLM, afin que les utilisateurs soient limités à accéder aux informations de leur propre boîte aux lettres avec leurs propres informations d’identification d’ouverture de session. Les applications clientes doivent également prendre en charge l’accès délégué pour les utilisateurs qui ont reçu l’autorisation d’accéder à la boîte aux lettres d’un autre utilisateur.
  
## <a name="portal-applications"></a>Applications de portail
<a name="bk_portalapps"> </a>

Une application portail étend une page Web ou un portail existant pour inclure les informations de boîte aux lettres Exchange en tant que composant personnalisé de la page. Les composants WebPart SharePoint sont les applications de portail les plus courantes et fournissent aux utilisateurs une expérience personnalisée en fournissant des vues dans les données de boîte aux lettres Exchange, telles que les messages non lus, les messages les plus récents et les événements de calendrier, à côté de leur page de portail SharePoint. Les applications de portail EWS peuvent utiliser l’accès au client direct, l’accès délégué ou l’emprunt d’identité pour récupérer des données de la Banque de boîtes aux lettres. Étant donné que les versions Exchange 2013 et SharePoint 2013 prennent en charge le protocole d’autorisation OAuth pour l’authentification de serveur à serveur, OAuth offre la méthode d’authentification la plus transparente et la plus sécurisée.
  
## <a name="service-applications"></a>Applications de service
<a name="bk_serviceapps"> </a>

Une application de service est généralement un travail d’arrière-plan intégré à une application existante qui s’étend à Exchange pour corréler les données entre le système et la Banque d’informations Exchange. Les applications de service n’ont généralement pas d’interface utilisateur et utilisent l’emprunt d’identité ou OAuth pour l’authentification et l’accès. La création d’un compte de service pour emprunter l’identité des utilisateurs est fréquente dans les applications de service EWS car vous pouvez accorder une autorisation de compte unique pour emprunter l’identité d’un ensemble d’utilisateurs et effectuer des opérations de boîte aux lettres pour ces comptes. Par exemple, une application de service EWS peut synchroniser des données entre des listes marketing dans une solution CRM et des groupes de distribution Exchange à l’aide d’un compte de service et de l’emprunt d’identité.
  
## <a name="see-also"></a>Voir aussi


- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Applications EWS et architecture Exchange](ews-applications-and-the-exchange-architecture.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

