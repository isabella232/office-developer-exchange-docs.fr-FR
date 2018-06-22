---
title: FreeBusyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponse
api_type:
- schema
ms.assetid: 3038d106-9ac9-4ac7-bb43-96c783edbef5
description: L’élément FreeBusyResponse contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique.
ms.openlocfilehash: 73e3972bb53d6bf59e5156098bad06bcde5f0155
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756481"
---
# <a name="freebusyresponse"></a><span data-ttu-id="42669-103">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="42669-103">FreeBusyResponse</span></span>

<span data-ttu-id="42669-104">L’élément **FreeBusyResponse** contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="42669-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="42669-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="42669-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="42669-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="42669-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="42669-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="42669-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="42669-108">**FreeBusyResponseType**</span><span class="sxs-lookup"><span data-stu-id="42669-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42669-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="42669-109">Attributes and elements</span></span>

<span data-ttu-id="42669-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="42669-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42669-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="42669-111">Attributes</span></span>

<span data-ttu-id="42669-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="42669-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42669-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="42669-113">Child elements</span></span>

|<span data-ttu-id="42669-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="42669-114">**Element**</span></span>|<span data-ttu-id="42669-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="42669-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42669-116">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="42669-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="42669-117">Fournit des informations descriptives concernant l’état de réponse.</span><span class="sxs-lookup"><span data-stu-id="42669-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="42669-118">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="42669-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="42669-119">Contient des informations de disponibilité pour un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="42669-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="42669-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="42669-120">Parent elements</span></span>

|<span data-ttu-id="42669-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="42669-121">**Element**</span></span>|<span data-ttu-id="42669-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="42669-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42669-123">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="42669-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="42669-124">Contient des informations de disponibilité de l’utilisateur demandé et l’état de réponse.</span><span class="sxs-lookup"><span data-stu-id="42669-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="42669-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="42669-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="42669-126">Note</span><span class="sxs-lookup"><span data-stu-id="42669-126">Remarks</span></span>

<span data-ttu-id="42669-127">Cet élément n’est pas inclus dans une réponse GetUserAvailability si les informations de disponibilité ne sont pas demandées.</span><span class="sxs-lookup"><span data-stu-id="42669-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="42669-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="42669-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42669-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="42669-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42669-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="42669-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="42669-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="42669-131">Schema Name</span></span>  <br/> |<span data-ttu-id="42669-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="42669-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="42669-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="42669-133">Validation File</span></span>  <br/> |<span data-ttu-id="42669-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="42669-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="42669-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="42669-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="42669-136">False</span><span class="sxs-lookup"><span data-stu-id="42669-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42669-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="42669-137">See also</span></span>



[<span data-ttu-id="42669-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="42669-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="42669-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="42669-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="42669-140">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="42669-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

