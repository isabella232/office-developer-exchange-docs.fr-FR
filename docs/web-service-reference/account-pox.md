---
title: Compte (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: L’élément compte Spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur.
ms.openlocfilehash: 88911aad41816f7cefbffef151e066fe5d4da192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756321"
---
# <a name="account-pox"></a><span data-ttu-id="54d39-103">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-103">Account (POX)</span></span>

<span data-ttu-id="54d39-104">L’élément **compte** spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur.</span><span class="sxs-lookup"><span data-stu-id="54d39-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="54d39-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="54d39-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="54d39-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-107">Account (POX)</span></span>](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="54d39-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="54d39-108">Attributes and elements</span></span>

<span data-ttu-id="54d39-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="54d39-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54d39-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="54d39-110">Attributes</span></span>

<span data-ttu-id="54d39-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54d39-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54d39-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="54d39-112">Child elements</span></span>

|<span data-ttu-id="54d39-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54d39-113">**Element**</span></span>|<span data-ttu-id="54d39-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="54d39-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54d39-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="54d39-116">Représente le type de compte.</span><span class="sxs-lookup"><span data-stu-id="54d39-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="54d39-117">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="54d39-118">Fournit des informations qui sont utilisées pour déterminer si une autre requête de découverte automatique est requise pour retourner les informations de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54d39-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="54d39-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="54d39-120">Contient une valeur qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="54d39-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="54d39-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="54d39-122">Contient l’URL de l’ordinateur qui exécute le serveur Exchange qui a le rôle de serveur Client Access installé qui doit être utilisé pour obtenir les paramètres de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="54d39-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="54d39-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="54d39-124">Spécifie l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.</span><span class="sxs-lookup"><span data-stu-id="54d39-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="54d39-125">Image (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="54d39-126">Contient le chemin d’accès d’une image qui est utilisée pour personnaliser l’expérience de configuration.</span><span class="sxs-lookup"><span data-stu-id="54d39-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="54d39-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="54d39-128">Contient l’URL de la page d’accueil du fournisseur de services Internet (fournisseur de services Internet).</span><span class="sxs-lookup"><span data-stu-id="54d39-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="54d39-129">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="54d39-130">Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="54d39-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="54d39-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="54d39-132">Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54d39-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="54d39-133">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="54d39-134">Contient une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="54d39-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54d39-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="54d39-135">Parent elements</span></span>

|<span data-ttu-id="54d39-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54d39-136">**Element**</span></span>|<span data-ttu-id="54d39-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="54d39-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54d39-138">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="54d39-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="54d39-139">Contient la réponse du service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="54d39-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54d39-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="54d39-140">See also</span></span>

- [<span data-ttu-id="54d39-141">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="54d39-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

