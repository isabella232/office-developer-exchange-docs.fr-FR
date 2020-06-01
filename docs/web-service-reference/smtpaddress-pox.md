---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: L’élément SmtpAddress contient l’adresse SMTP attribuée à la Banque de messages de dossiers publics configurée pour l’utilisateur.
ms.openlocfilehash: 48703a11fb056967c6c76073c2e928d5f6efa264
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468641"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="d61b5-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="d61b5-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="d61b5-104">L’élément **SmtpAddress** contient l’adresse SMTP attribuée à la Banque de messages de dossiers publics configurée pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d61b5-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="d61b5-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="d61b5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="d61b5-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="d61b5-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="d61b5-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="d61b5-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="d61b5-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="d61b5-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="d61b5-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="d61b5-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d61b5-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d61b5-110">Attributes and elements</span></span>

<span data-ttu-id="d61b5-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d61b5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d61b5-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d61b5-112">Attributes</span></span>

<span data-ttu-id="d61b5-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d61b5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d61b5-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d61b5-114">Child elements</span></span>

<span data-ttu-id="d61b5-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d61b5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d61b5-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d61b5-116">Parent elements</span></span>

|<span data-ttu-id="d61b5-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d61b5-117">**Element**</span></span>|<span data-ttu-id="d61b5-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="d61b5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d61b5-119">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="d61b5-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="d61b5-120">Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d61b5-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d61b5-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d61b5-121">Text value</span></span>

<span data-ttu-id="d61b5-122">La valeur de texte représente l’adresse SMTP attribuée à la Banque de dossiers publics configurée pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d61b5-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="d61b5-123">Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une demande de découverte automatique pour découvrir les paramètres de dossier public.</span><span class="sxs-lookup"><span data-stu-id="d61b5-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d61b5-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="d61b5-124">Remarks</span></span>

<span data-ttu-id="d61b5-125">L’élément **SmtpAddress** est un élément enfant obligatoire de l’élément **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="d61b5-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d61b5-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d61b5-126">See also</span></span>

- [<span data-ttu-id="d61b5-127">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d61b5-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

