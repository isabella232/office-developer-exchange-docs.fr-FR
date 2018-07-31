---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: L’élément compte Spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur.
ms.openlocfilehash: 6cd87e678b3a524a69f6dca4d6999a3cff22fa57
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353342"
---
# <a name="account-pox"></a><span data-ttu-id="78f0c-103">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-103">Account (POX)</span></span>

<span data-ttu-id="78f0c-104">L’élément **compte** spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur.</span><span class="sxs-lookup"><span data-stu-id="78f0c-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="78f0c-105">AutoDiscover (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="78f0c-106">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="78f0c-107">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-107">Account (POX)</span></span>](account-pox.md)
  
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

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="78f0c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="78f0c-108">Attributes and elements</span></span>

<span data-ttu-id="78f0c-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="78f0c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78f0c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="78f0c-110">Attributes</span></span>

<span data-ttu-id="78f0c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="78f0c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78f0c-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="78f0c-112">Child elements</span></span>

|<span data-ttu-id="78f0c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78f0c-113">**Element**</span></span>|<span data-ttu-id="78f0c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="78f0c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78f0c-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="78f0c-116">Représente le type de compte.</span><span class="sxs-lookup"><span data-stu-id="78f0c-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-117">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="78f0c-118">Fournit des informations qui sont utilisées pour déterminer si une autre requête de découverte automatique est requise pour retourner les informations de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="78f0c-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="78f0c-120">Contient une valeur qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="78f0c-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="78f0c-122">Contient l’URL de l’ordinateur qui exécute le serveur Exchange qui a le rôle de serveur Client Access installé qui doit être utilisé pour obtenir les paramètres de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="78f0c-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="78f0c-124">Spécifie l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.</span><span class="sxs-lookup"><span data-stu-id="78f0c-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-125">Image (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="78f0c-126">Contient le chemin d’accès d’une image qui est utilisée pour personnaliser l’expérience de configuration.</span><span class="sxs-lookup"><span data-stu-id="78f0c-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="78f0c-128">Contient l’URL de la page d’accueil du fournisseur de services Internet (fournisseur de services Internet).</span><span class="sxs-lookup"><span data-stu-id="78f0c-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="78f0c-129">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="78f0c-130">Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="78f0c-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="78f0c-132">Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="78f0c-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="78f0c-133">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="78f0c-134">Contient une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="78f0c-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78f0c-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="78f0c-135">Parent elements</span></span>

|<span data-ttu-id="78f0c-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78f0c-136">**Element**</span></span>|<span data-ttu-id="78f0c-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="78f0c-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78f0c-138">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="78f0c-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="78f0c-139">Contient la réponse du service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="78f0c-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78f0c-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="78f0c-140">See also</span></span>

- [<span data-ttu-id="78f0c-141">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="78f0c-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

