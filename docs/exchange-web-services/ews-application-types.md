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
# <a name="ews-application-types"></a><span data-ttu-id="f8e3b-103">Types d’applications EWS</span><span class="sxs-lookup"><span data-stu-id="f8e3b-103">EWS application types</span></span>

<span data-ttu-id="f8e3b-104">Découvrez les principaux types d'applications que vous pouvez créer à l'aide des services web Exchange dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-104">Find out about the most common types of applications that you can create by using EWS in Exchange.</span></span>
  
<span data-ttu-id="f8e3b-105">L' [architecture EWS et Exchange](ews-applications-and-the-exchange-architecture.md) fournit un modèle de développement uniforme que vous pouvez utiliser pour créer les types les plus courantes des applications de manière cohérente, notamment les suivantes :</span><span class="sxs-lookup"><span data-stu-id="f8e3b-105">The [EWS and Exchange architecture](ews-applications-and-the-exchange-architecture.md) provides a uniform development model that you can use to create the most common types of applications in a consistent way, including the following:</span></span> 
  
- <span data-ttu-id="f8e3b-106">[Applications clientes](#bk_clientapps) , des applications autonomes par EWS pour accéder aux données Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-106">[Client applications](#bk_clientapps) — Standalone applications that use EWS to access Exchange data.</span></span> <span data-ttu-id="f8e3b-107">Outlook et Outlook Web App sont des exemples d’applications clientes.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-107">Outlook and Outlook Web App are examples of client applications.</span></span> 
    
- <span data-ttu-id="f8e3b-108">[Applications portail](#bk_portalapps) : Applications qui étendent une page web existante en incluant des informations récupérées à partir d’Exchange, telles que les informations de disponibilité ou de contact.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-108">[Portal applications](#bk_portalapps) — Applications that extend an existing web page by including information retrieved from Exchange, such as free/busy or contact information.</span></span> <span data-ttu-id="f8e3b-109">Un composant WebPart SharePoint qui Récupère les données Exchange est un exemple d’une application de portail.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-109">A SharePoint web part that retrieves Exchange data is an example of a portal application.</span></span> 
    
- <span data-ttu-id="f8e3b-110">[Applications de service](#bk_serviceapps) — tâches permet d’intégrer ou synchroniser les données à partir d’Exchange dans un système existant.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-110">[Service applications](#bk_serviceapps) — Background jobs used to integrate or synchronize data from Exchange into an existing system.</span></span> <span data-ttu-id="f8e3b-111">Par exemple, une application qui synchronise les informations de contact à partir d’Exchange dans une application CRM.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-111">For example, an application that synchronizes contact information from Exchange into a CRM application.</span></span> 
    
<span data-ttu-id="f8e3b-112">Chacun de ces modèles d’application peut utiliser une base de code courantes pour récupérer des informations à partir d’Exchange - afin que vous n’avez pas besoin de modifier le code EWS permet de récupérer des informations entre un client, un portail ou une application de service.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-112">Each of these application models can use a common code base to retrieve information from Exchange - so you don't need to change the EWS code used to retrieve item information between a client, portal, or service application.</span></span> <span data-ttu-id="f8e3b-113">Ce qui peut changer d’une application à l’autre est le mécanisme d’accès et l’authentification de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-113">What might change from one application to the next is the mailbox access and authentication mechanism.</span></span> <span data-ttu-id="f8e3b-114">Par exemple, les applications clientes utilisent couramment accès direct des utilisateurs et basic ou l’authentification NTLM, tandis que d’une application de service probablement utilise l’emprunt d’identité pour l’accès aux boîtes aux lettres et l’authentification OAuth.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-114">For example, client applications commonly use direct user access and basic or NTLM authentication, whereas a service application likely uses impersonation for mailbox access and OAuth authentication.</span></span>
  
## <a name="client-applications"></a><span data-ttu-id="f8e3b-115">Applications clientes</span><span class="sxs-lookup"><span data-stu-id="f8e3b-115">Client applications</span></span>
<span data-ttu-id="f8e3b-116"><a name="bk_clientapps"> </a></span><span class="sxs-lookup"><span data-stu-id="f8e3b-116"></span></span>

<span data-ttu-id="f8e3b-117">Une application cliente EWS est n’importe quelle application autonome qui utilise EWS pour récupérer des informations à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-117">An EWS client application is any standalone application that uses EWS to retrieve information from the Exchange store.</span></span> <span data-ttu-id="f8e3b-118">Les applications clientes EWS utilisent accès direct client ou l’accès délégué à extraire des données de la banque de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-118">EWS client applications use direct client access or delegate access to retrieve data from the mailbox store.</span></span> <span data-ttu-id="f8e3b-119">Voici quelques exemples d’applications clientes qui utilisent EWS :</span><span class="sxs-lookup"><span data-stu-id="f8e3b-119">The following are some examples of client applications that use EWS:</span></span>
  
- <span data-ttu-id="f8e3b-120">Outlook, telles que l’état d’absence du bureau Infos-courrier, disponibilité et d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="f8e3b-120">Outlook, in features such as MailTips, availability, and user OOF status</span></span>
    
- <span data-ttu-id="f8e3b-121">OWA pour les périphériques</span><span class="sxs-lookup"><span data-stu-id="f8e3b-121">OWA for Devices</span></span>
    
- <span data-ttu-id="f8e3b-122">Outlook pour Mac 2011</span><span class="sxs-lookup"><span data-stu-id="f8e3b-122">Outlook for Mac 2011</span></span>
    
- <span data-ttu-id="f8e3b-123">Lync, des informations de disponibilité</span><span class="sxs-lookup"><span data-stu-id="f8e3b-123">Lync, for availability information</span></span>
    
<span data-ttu-id="f8e3b-124">Applications clientes utilisent généralement un accès direct et basic ou l’authentification NTLM, afin que les utilisateurs sont limitées à accéder aux informations dans leur propre boîte aux lettres avec leurs propres informations d’identification d’ouverture de session.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-124">Client applications commonly use direct access and basic or NTLM authentication, so that users are limited to accessing information in their own mailbox with their own logon credentials.</span></span> <span data-ttu-id="f8e3b-125">Les applications clientes doivent prennent également en charge l’accès pour les utilisateurs qui disposent de l’autorisation d’accéder aux boîtes aux lettres d’un autre utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-125">Client applications should also support delegate access for users who have been given permission to access another user's mailbox.</span></span>
  
## <a name="portal-applications"></a><span data-ttu-id="f8e3b-126">Applications de portail</span><span class="sxs-lookup"><span data-stu-id="f8e3b-126">Portal applications</span></span>
<span data-ttu-id="f8e3b-127"><a name="bk_portalapps"> </a></span><span class="sxs-lookup"><span data-stu-id="f8e3b-127"></span></span>

<span data-ttu-id="f8e3b-128">Une application de portail étend une page web existante ou un portail pour inclure des informations de boîte aux lettres Exchange comme un composant personnalisé de la page.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-128">A portal application extends an existing web page or portal to include Exchange mailbox information as a personalized component of the page.</span></span> <span data-ttu-id="f8e3b-129">Composants WebPart SharePoint sont les plus courantes applications portails et fournissent aux utilisateurs une expérience personnalisée en fournissant des affichages dans les données de boîte aux lettres Exchange, tels que les messages non lus, les messages plus récentes et les événements du calendrier, ainsi que leurs visualisées Page du portail SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-129">SharePoint web parts are the most common portal applications and provide users with a personalized experience by providing views into Exchange mailbox data, such as unread messages, most recent messages, and calendar events, alongside their commonly viewed SharePoint portal page.</span></span> <span data-ttu-id="f8e3b-130">Applications de portail EWS peuvent utiliser des accès au client direct, accès délégué ou emprunt d’identité pour récupérer des données à partir de la banque de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-130">EWS portal applications can use direct client access, delegate access, or impersonation to retrieve data from the mailbox store.</span></span> <span data-ttu-id="f8e3b-131">Étant donné que Exchange 2013 et SharePoint 2013 prend en charge le protocole d’autorisation OAuth pour l’authentification de serveur à serveur, OAuth fournit la méthode d’authentification plus sécurisée et transparente.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-131">Because Exchange 2013 and SharePoint 2013 both support the OAuth authorization protocol for server-to-server authentication, OAuth provides the most seamless and secure authentication method.</span></span>
  
## <a name="service-applications"></a><span data-ttu-id="f8e3b-132">Applications de service</span><span class="sxs-lookup"><span data-stu-id="f8e3b-132">Service applications</span></span>
<span data-ttu-id="f8e3b-133"><a name="bk_serviceapps"> </a></span><span class="sxs-lookup"><span data-stu-id="f8e3b-133"></span></span>

<span data-ttu-id="f8e3b-134">Une application de service est généralement une tâche en arrière-plan intégrée à une application existante qui s’étend jusqu'à Exchange à corréler les données entre le système et la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-134">A service application is usually a background job built into an existing application that extends to Exchange to correlate data between the system and the Exchange store.</span></span> <span data-ttu-id="f8e3b-135">Applications de service généralement ne pas avoir une interface utilisateur et utiliser l’emprunt d’identité ou OAuth pour l’authentification et l’accès.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-135">Service applications typically do not have a user interface and use impersonation or OAuth for authentication and access.</span></span> <span data-ttu-id="f8e3b-136">Création d’un compte de service pour emprunter l’identité des utilisateurs est souvent dans les applications de service EWS, car vous pouvez autoriser un compte unique pour emprunter l’identité d’un ensemble d’utilisateurs et d’effectuer des opérations de boîte aux lettres pour ces comptes.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-136">Creating a service account to impersonate users is common in EWS service apps because you can grant a single account permission to impersonate a set of users and perform mailbox operations for those accounts.</span></span> <span data-ttu-id="f8e3b-137">Par exemple, une application de service EWS synchroniser les données entre les listes marketing dans une solution CRM et les groupes de distribution Exchange en utilisant un compte de service et l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="f8e3b-137">For example, an EWS service application can synchronize data between marketing lists in a CRM solution and Exchange distribution groups by using a service account and impersonation.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="f8e3b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f8e3b-138">See also</span></span>


- [<span data-ttu-id="f8e3b-139">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f8e3b-139">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="f8e3b-140">Applications EWS et l’architecture Exchange</span><span class="sxs-lookup"><span data-stu-id="f8e3b-140">EWS applications and the Exchange architecture</span></span>](ews-applications-and-the-exchange-architecture.md)
    
- [<span data-ttu-id="f8e3b-141">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="f8e3b-141">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
