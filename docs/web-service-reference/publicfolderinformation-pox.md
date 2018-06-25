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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828927"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="fd530-103">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="fd530-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="fd530-104">L’élément **PublicFolderInformation** contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="fd530-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="fd530-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="fd530-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="fd530-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="fd530-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="fd530-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="fd530-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="fd530-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="fd530-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="fd530-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fd530-109">Attributes and elements</span></span>

<span data-ttu-id="fd530-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fd530-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd530-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="fd530-111">Attributes</span></span>

<span data-ttu-id="fd530-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fd530-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd530-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fd530-113">Child elements</span></span>

|<span data-ttu-id="fd530-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fd530-114">**Element**</span></span>|<span data-ttu-id="fd530-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd530-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd530-116">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="fd530-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="fd530-117">Contient l’adresse SMTP affectée à la banque de messages de dossier public configurée pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="fd530-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="fd530-118">Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une requête de découverte automatique pour découvrir les paramètres des dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="fd530-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd530-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fd530-119">Parent elements</span></span>

|<span data-ttu-id="fd530-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fd530-120">**Element**</span></span>|<span data-ttu-id="fd530-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="fd530-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd530-122">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="fd530-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="fd530-123">Spécifie les paramètres de compte pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="fd530-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd530-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="fd530-124">Remarks</span></span>

<span data-ttu-id="fd530-125">L’élément **PublicFolderInformation** est un élément enfant facultatif de l’élément de **compte** .</span><span class="sxs-lookup"><span data-stu-id="fd530-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fd530-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fd530-126">See also</span></span>



[<span data-ttu-id="fd530-127">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="fd530-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

