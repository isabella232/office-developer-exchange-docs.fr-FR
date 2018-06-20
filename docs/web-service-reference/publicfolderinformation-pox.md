---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: L’élément PublicFolderInformation contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828927"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="2307b-103">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="2307b-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="2307b-104">L’élément **PublicFolderInformation** contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2307b-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="2307b-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="2307b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="2307b-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="2307b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="2307b-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="2307b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="2307b-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="2307b-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2307b-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2307b-109">Attributes and elements</span></span>

<span data-ttu-id="2307b-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2307b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2307b-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="2307b-111">Attributes</span></span>

<span data-ttu-id="2307b-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2307b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2307b-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2307b-113">Child elements</span></span>

|<span data-ttu-id="2307b-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2307b-114">**Element**</span></span>|<span data-ttu-id="2307b-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="2307b-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2307b-116">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="2307b-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="2307b-117">Contient l’adresse SMTP affectée à la banque de messages de dossier public configurée pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2307b-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="2307b-118">Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une requête de découverte automatique pour découvrir les paramètres des dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="2307b-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2307b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2307b-119">Parent elements</span></span>

|<span data-ttu-id="2307b-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2307b-120">**Element**</span></span>|<span data-ttu-id="2307b-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2307b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2307b-122">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="2307b-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="2307b-123">Spécifie les paramètres de compte pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2307b-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2307b-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="2307b-124">Remarks</span></span>

<span data-ttu-id="2307b-125">L’élément **PublicFolderInformation** est un élément enfant facultatif de l’élément de **compte** .</span><span class="sxs-lookup"><span data-stu-id="2307b-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2307b-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2307b-126">See also</span></span>



[<span data-ttu-id="2307b-127">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="2307b-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

