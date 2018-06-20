---
title: Types d’applications EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ca4e8b90-d0d8-4d55-aa92-19e21659d4f5
description: Découvrez les principaux types d'applications que vous pouvez créer à l'aide des services web Exchange dans Exchange.
ms.openlocfilehash: 1ce739f453ba1bc6f1b5d38edae3776daa562ffb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754769"
---
# <a name="ews-application-types"></a>Types d’applications EWS

Découvrez les principaux types d'applications que vous pouvez créer à l'aide des services web Exchange dans Exchange.
  
L' [architecture EWS et Exchange](ews-applications-and-the-exchange-architecture.md) fournit un modèle de développement uniforme que vous pouvez utiliser pour créer les types les plus courantes des applications de manière cohérente, notamment les suivantes : 
  
- [Applications clientes](#bk_clientapps) , des applications autonomes par EWS pour accéder aux données Exchange. Outlook et Outlook Web App sont des exemples d’applications clientes. 
    
- [Applications portail](#bk_portalapps) : Applications qui étendent une page web existante en incluant des informations récupérées à partir d’Exchange, telles que les informations de disponibilité ou de contact. Un composant WebPart SharePoint qui Récupère les données Exchange est un exemple d’une application de portail. 
    
- [Applications de service](#bk_serviceapps) — tâches permet d’intégrer ou synchroniser les données à partir d’Exchange dans un système existant. Par exemple, une application qui synchronise les informations de contact à partir d’Exchange dans une application CRM. 
    
Chacun de ces modèles d’application peut utiliser une base de code courantes pour récupérer des informations à partir d’Exchange - afin que vous n’avez pas besoin de modifier le code EWS permet de récupérer des informations entre un client, un portail ou une application de service. Ce qui peut changer d’une application à l’autre est le mécanisme d’accès et l’authentification de boîte aux lettres. Par exemple, les applications clientes utilisent couramment accès direct des utilisateurs et basic ou l’authentification NTLM, tandis que d’une application de service probablement utilise l’emprunt d’identité pour l’accès aux boîtes aux lettres et l’authentification OAuth.
  
## <a name="client-applications"></a>Applications clientes
<a name="bk_clientapps"> </a>

Une application cliente EWS est n’importe quelle application autonome qui utilise EWS pour récupérer des informations à partir de la banque d’informations Exchange. Les applications clientes EWS utilisent accès direct client ou l’accès délégué à extraire des données de la banque de boîtes aux lettres. Voici quelques exemples d’applications clientes qui utilisent EWS :
  
- Outlook, telles que l’état d’absence du bureau Infos-courrier, disponibilité et d’utilisateur
    
- OWA pour les périphériques
    
- Outlook pour Mac 2011
    
- Lync, des informations de disponibilité
    
Applications clientes utilisent généralement un accès direct et basic ou l’authentification NTLM, afin que les utilisateurs sont limitées à accéder aux informations dans leur propre boîte aux lettres avec leurs propres informations d’identification d’ouverture de session. Les applications clientes doivent prennent également en charge l’accès pour les utilisateurs qui disposent de l’autorisation d’accéder aux boîtes aux lettres d’un autre utilisateur délégué.
  
## <a name="portal-applications"></a>Applications de portail
<a name="bk_portalapps"> </a>

Une application de portail étend une page web existante ou un portail pour inclure des informations de boîte aux lettres Exchange comme un composant personnalisé de la page. Composants WebPart SharePoint sont les plus courantes applications portails et fournissent aux utilisateurs une expérience personnalisée en fournissant des affichages dans les données de boîte aux lettres Exchange, tels que les messages non lus, les messages plus récentes et les événements du calendrier, ainsi que leurs visualisées Page du portail SharePoint. Applications de portail EWS peuvent utiliser des accès au client direct, accès délégué ou emprunt d’identité pour récupérer des données à partir de la banque de boîtes aux lettres. Étant donné que Exchange 2013 et SharePoint 2013 prend en charge le protocole d’autorisation OAuth pour l’authentification de serveur à serveur, OAuth fournit la méthode d’authentification plus sécurisée et transparente.
  
## <a name="service-applications"></a>Applications de service
<a name="bk_serviceapps"> </a>

Une application de service est généralement une tâche en arrière-plan intégrée à une application existante qui s’étend jusqu'à Exchange à corréler les données entre le système et la banque d’informations Exchange. Applications de service généralement ne pas avoir une interface utilisateur et utiliser l’emprunt d’identité ou OAuth pour l’authentification et l’accès. Création d’un compte de service pour emprunter l’identité des utilisateurs est souvent dans les applications de service EWS, car vous pouvez autoriser un compte unique pour emprunter l’identité d’un ensemble d’utilisateurs et d’effectuer des opérations de boîte aux lettres pour ces comptes. Par exemple, une application de service EWS synchroniser les données entre les listes marketing dans une solution CRM et les groupes de distribution Exchange en utilisant un compte de service et l’emprunt d’identité.
  
## <a name="see-also"></a>Voir aussi


- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Applications EWS et l’architecture Exchange](ews-applications-and-the-exchange-architecture.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

