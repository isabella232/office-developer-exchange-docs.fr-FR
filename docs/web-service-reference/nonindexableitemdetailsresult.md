---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: L’élément NonIndexableItemDetailsResult spécifie les résultats de l’opération WSDL GetNonIndexableItemDetails.
ms.openlocfilehash: 6e271f2cf0e37f26b945332c94167b6a42354115
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828535"
---
# <a name="nonindexableitemdetailsresult"></a><span data-ttu-id="68147-103">NonIndexableItemDetailsResult</span><span class="sxs-lookup"><span data-stu-id="68147-103">NonIndexableItemDetailsResult</span></span>

<span data-ttu-id="68147-104">L’élément **NonIndexableItemDetailsResult** spécifie les résultats de l’opération WSDL **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="68147-104">The **NonIndexableItemDetailsResult** element specifies the results of the **GetNonIndexableItemDetails** WSDL operation.</span></span> 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 <span data-ttu-id="68147-105">**NonIndexableItemDetailResultType**</span><span class="sxs-lookup"><span data-stu-id="68147-105">**NonIndexableItemDetailResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68147-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="68147-106">Attributes and elements</span></span>

<span data-ttu-id="68147-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="68147-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68147-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="68147-108">Attributes</span></span>

<span data-ttu-id="68147-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="68147-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68147-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="68147-110">Child elements</span></span>

<span data-ttu-id="68147-111">[Éléments (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="68147-111">[Items (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="68147-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="68147-112">Parent elements</span></span>

<span data-ttu-id="68147-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="68147-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68147-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="68147-114">Remarks</span></span>

<span data-ttu-id="68147-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="68147-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="68147-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="68147-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68147-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="68147-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68147-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="68147-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68147-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="68147-119">Schema name</span></span>  <br/> |<span data-ttu-id="68147-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="68147-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68147-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="68147-121">Validation file</span></span>  <br/> |<span data-ttu-id="68147-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="68147-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68147-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="68147-123">Can be empty</span></span>  <br/> |<span data-ttu-id="68147-124">False</span><span class="sxs-lookup"><span data-stu-id="68147-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68147-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="68147-125">See also</span></span>



[<span data-ttu-id="68147-126">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="68147-126">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)


- [<span data-ttu-id="68147-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68147-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

