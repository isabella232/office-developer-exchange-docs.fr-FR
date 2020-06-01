---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: L’élément PublicFolderInformation contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir les informations de dossier public pour l’utilisateur.
ms.openlocfilehash: e044a1feddfaeb4eb93c289c617dde9adc66f332
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457717"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="7a5dd-103">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="7a5dd-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="7a5dd-104">L’élément **PublicFolderInformation** contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7a5dd-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="7a5dd-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="7a5dd-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="7a5dd-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="7a5dd-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="7a5dd-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="7a5dd-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="7a5dd-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="7a5dd-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="7a5dd-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a5dd-109">Attributes and elements</span></span>

<span data-ttu-id="7a5dd-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a5dd-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a5dd-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a5dd-111">Attributes</span></span>

<span data-ttu-id="7a5dd-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7a5dd-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a5dd-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a5dd-113">Child elements</span></span>

|<span data-ttu-id="7a5dd-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a5dd-114">**Element**</span></span>|<span data-ttu-id="7a5dd-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a5dd-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a5dd-116">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="7a5dd-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="7a5dd-117">Contient l’adresse SMTP attribuée à la Banque de messages de dossiers publics configurée pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7a5dd-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="7a5dd-118">Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une demande de découverte automatique pour découvrir les paramètres de dossier public.</span><span class="sxs-lookup"><span data-stu-id="7a5dd-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a5dd-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a5dd-119">Parent elements</span></span>

|<span data-ttu-id="7a5dd-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a5dd-120">**Element**</span></span>|<span data-ttu-id="7a5dd-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a5dd-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a5dd-122">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="7a5dd-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="7a5dd-123">Spécifie les paramètres de compte de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7a5dd-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a5dd-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a5dd-124">Remarks</span></span>

<span data-ttu-id="7a5dd-125">L’élément **PublicFolderInformation** est un élément enfant facultatif de l’élément **Account** .</span><span class="sxs-lookup"><span data-stu-id="7a5dd-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7a5dd-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a5dd-126">See also</span></span>



[<span data-ttu-id="7a5dd-127">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7a5dd-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

