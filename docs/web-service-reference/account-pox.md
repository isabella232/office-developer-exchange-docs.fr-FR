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
description: L’élément Account spécifie les paramètres de compte de l’utilisateur ou contient des réponses d’erreur.
ms.openlocfilehash: ffd8ebe4b7bd9d4b3f6a9b42fc557ac6189a068d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462317"
---
# <a name="account-pox"></a><span data-ttu-id="a2eef-103">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-103">Account (POX)</span></span>

<span data-ttu-id="a2eef-104">L’élément **Account** spécifie les paramètres de compte de l’utilisateur ou contient des réponses d’erreur.</span><span class="sxs-lookup"><span data-stu-id="a2eef-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="a2eef-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="a2eef-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="a2eef-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-107">Account (POX)</span></span>](account-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="a2eef-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a2eef-108">Attributes and elements</span></span>

<span data-ttu-id="a2eef-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a2eef-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2eef-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a2eef-110">Attributes</span></span>

<span data-ttu-id="a2eef-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a2eef-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2eef-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a2eef-112">Child elements</span></span>

|<span data-ttu-id="a2eef-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2eef-113">**Element**</span></span>|<span data-ttu-id="a2eef-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2eef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2eef-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="a2eef-116">Représente le type de compte.</span><span class="sxs-lookup"><span data-stu-id="a2eef-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-117">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="a2eef-118">Fournit des informations qui permettent de déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a2eef-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="a2eef-120">Contient une valeur qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="a2eef-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="a2eef-122">Contient l’URL de l’ordinateur qui exécute Exchange Server sur lequel le rôle serveur d’accès au client est installé et qui doit être utilisé pour obtenir les paramètres de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="a2eef-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="a2eef-124">Spécifie l’adresse de messagerie à utiliser pour une demande de découverte automatique ultérieure.</span><span class="sxs-lookup"><span data-stu-id="a2eef-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-125">Image (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="a2eef-126">Contient le chemin d’accès d’une image utilisée pour personnaliser l’expérience de configuration.</span><span class="sxs-lookup"><span data-stu-id="a2eef-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="a2eef-128">Contient l’URL de la page d’accueil du fournisseur de services Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="a2eef-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="a2eef-129">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a2eef-130">Contient les spécifications relatives à la connexion d’un client au serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="a2eef-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="a2eef-132">Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a2eef-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="a2eef-133">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="a2eef-134">Contient une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="a2eef-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2eef-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a2eef-135">Parent elements</span></span>

|<span data-ttu-id="a2eef-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2eef-136">**Element**</span></span>|<span data-ttu-id="a2eef-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2eef-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2eef-138">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="a2eef-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="a2eef-139">Contient la réponse du service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="a2eef-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2eef-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2eef-140">See also</span></span>

- [<span data-ttu-id="a2eef-141">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="a2eef-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

