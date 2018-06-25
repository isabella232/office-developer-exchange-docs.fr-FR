---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: L’élément SmtpAddress contient l’adresse SMTP affectée à la banque de messages de dossier public configurée pour l’utilisateur.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829507"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="54f9b-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="54f9b-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="54f9b-104">L’élément **SmtpAddress** contient l’adresse SMTP affectée à la banque de messages de dossier public configurée pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54f9b-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="54f9b-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="54f9b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="54f9b-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="54f9b-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="54f9b-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="54f9b-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="54f9b-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="54f9b-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="54f9b-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="54f9b-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="54f9b-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="54f9b-110">Attributes and elements</span></span>

<span data-ttu-id="54f9b-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="54f9b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54f9b-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="54f9b-112">Attributes</span></span>

<span data-ttu-id="54f9b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54f9b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54f9b-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="54f9b-114">Child elements</span></span>

<span data-ttu-id="54f9b-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54f9b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54f9b-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="54f9b-116">Parent elements</span></span>

|<span data-ttu-id="54f9b-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54f9b-117">**Element**</span></span>|<span data-ttu-id="54f9b-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="54f9b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f9b-119">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="54f9b-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="54f9b-120">Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54f9b-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54f9b-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="54f9b-121">Text value</span></span>

<span data-ttu-id="54f9b-122">La valeur de text représente l’adresse SMTP affectée à la banque de dossiers publics configurée pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54f9b-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="54f9b-123">Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une requête de découverte automatique pour découvrir les paramètres des dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="54f9b-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="54f9b-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="54f9b-124">Remarks</span></span>

<span data-ttu-id="54f9b-125">L’élément **SmtpAddress** est un élément enfant requis de l’élément **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="54f9b-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="54f9b-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="54f9b-126">See also</span></span>

- [<span data-ttu-id="54f9b-127">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="54f9b-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

