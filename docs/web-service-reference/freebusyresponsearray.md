---
title: FreeBusyResponseArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponseArray
api_type:
- schema
ms.assetid: 5592a37e-cf4b-4643-8a2a-fa58c40345b9
description: L’élément FreeBusyResponseArray contient des informations de disponibilité de l’utilisateur demandé et l’état de réponse.
ms.openlocfilehash: cc6022c28213667c40dc00b5627ed88c4f78e2f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756484"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="7f4be-103">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="7f4be-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="7f4be-104">L’élément **FreeBusyResponseArray** contient des informations de disponibilité de l’utilisateur demandé et l’état de réponse.</span><span class="sxs-lookup"><span data-stu-id="7f4be-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="7f4be-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7f4be-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7f4be-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="7f4be-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="7f4be-107">**ArrayOfFreeBusyResponse**</span><span class="sxs-lookup"><span data-stu-id="7f4be-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f4be-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7f4be-108">Attributes and elements</span></span>

<span data-ttu-id="7f4be-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7f4be-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f4be-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7f4be-110">Attributes</span></span>

<span data-ttu-id="7f4be-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7f4be-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f4be-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7f4be-112">Child elements</span></span>

|<span data-ttu-id="7f4be-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7f4be-113">**Element**</span></span>|<span data-ttu-id="7f4be-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7f4be-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f4be-115">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="7f4be-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="7f4be-116">Contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique et l’état de réponse.</span><span class="sxs-lookup"><span data-stu-id="7f4be-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7f4be-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7f4be-117">Parent elements</span></span>

|<span data-ttu-id="7f4be-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7f4be-118">**Element**</span></span>|<span data-ttu-id="7f4be-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="7f4be-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f4be-120">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7f4be-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="7f4be-121">Contient les propriétés qui définissent les informations de disponibilité utilisateur ou suggérés informations d’heure de la réunion.</span><span class="sxs-lookup"><span data-stu-id="7f4be-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="7f4be-122">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="7f4be-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7f4be-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="7f4be-123">Remarks</span></span>

<span data-ttu-id="7f4be-124">Cet élément n’est pas inclus dans une réponse GetUserAvailability si les informations de disponibilité ne sont pas demandées.</span><span class="sxs-lookup"><span data-stu-id="7f4be-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="7f4be-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7f4be-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f4be-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7f4be-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f4be-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7f4be-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f4be-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7f4be-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7f4be-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7f4be-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f4be-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7f4be-130">Validation File</span></span>  <br/> |<span data-ttu-id="7f4be-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f4be-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f4be-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7f4be-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f4be-133">False</span><span class="sxs-lookup"><span data-stu-id="7f4be-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f4be-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7f4be-134">See also</span></span>



[<span data-ttu-id="7f4be-135">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7f4be-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7f4be-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7f4be-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7f4be-137">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="7f4be-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

