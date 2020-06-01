---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: L’élément InPlaceHoldIdentity spécifie l’identité d’une conservation qui conserve les éléments de boîte aux lettres.
ms.openlocfilehash: a06f72e478e7dc5bd1a499dceefeb352b14d7362
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466093"
---
# <a name="inplaceholdidentity"></a><span data-ttu-id="3e9ef-103">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="3e9ef-103">InPlaceHoldIdentity</span></span>

<span data-ttu-id="3e9ef-104">L’élément **InPlaceHoldIdentity** spécifie l’identité d’une conservation qui conserve les éléments de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3e9ef-104">The **InPlaceHoldIdentity** element specifies the identity of a hold that preserves the mailbox items.</span></span> 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 <span data-ttu-id="3e9ef-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="3e9ef-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e9ef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e9ef-106">Attributes and elements</span></span>

<span data-ttu-id="3e9ef-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e9ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e9ef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e9ef-108">Attributes</span></span>

<span data-ttu-id="3e9ef-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3e9ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e9ef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e9ef-110">Child elements</span></span>

<span data-ttu-id="3e9ef-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e9ef-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3e9ef-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e9ef-112">Parent elements</span></span>

<span data-ttu-id="3e9ef-113">[SetHoldOnMailboxes](setholdonmailboxes.md)  |  [DiscoverySearchConfiguration](discoverysearchconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e9ef-113">[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3e9ef-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3e9ef-114">Text value</span></span>

<span data-ttu-id="3e9ef-115">La valeur de texte de l’élément **InPlaceHoldIdentity** est l’identificateur de conservation de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3e9ef-115">The text value of the **InPlaceHoldIdentity** element is the mailbox hold identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3e9ef-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e9ef-116">Remarks</span></span>

<span data-ttu-id="3e9ef-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3e9ef-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3e9ef-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e9ef-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e9ef-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e9ef-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e9ef-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e9ef-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3e9ef-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e9ef-121">Schema name</span></span>  <br/> |<span data-ttu-id="3e9ef-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3e9ef-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3e9ef-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e9ef-123">Validation file</span></span>  <br/> |<span data-ttu-id="3e9ef-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3e9ef-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3e9ef-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e9ef-125">Can be empty</span></span>  <br/> |<span data-ttu-id="3e9ef-126">False</span><span class="sxs-lookup"><span data-stu-id="3e9ef-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e9ef-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e9ef-127">See also</span></span>



[<span data-ttu-id="3e9ef-128">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3e9ef-128">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)


- [<span data-ttu-id="3e9ef-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e9ef-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

