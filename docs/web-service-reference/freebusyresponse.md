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
ms.openlocfilehash: 45a3e12756f3cbf29b76b442f7103abc5fb9a833
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461925"
---
# <a name="freebusyresponse"></a><span data-ttu-id="ad027-103">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="ad027-103">FreeBusyResponse</span></span>

<span data-ttu-id="ad027-104">L’élément **FreeBusyResponse** contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="ad027-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="ad027-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ad027-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ad027-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ad027-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ad027-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="ad027-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="ad027-108">**FreeBusyResponseType**</span><span class="sxs-lookup"><span data-stu-id="ad027-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad027-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad027-109">Attributes and elements</span></span>

<span data-ttu-id="ad027-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad027-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad027-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad027-111">Attributes</span></span>

<span data-ttu-id="ad027-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ad027-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad027-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad027-113">Child elements</span></span>

|<span data-ttu-id="ad027-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad027-114">**Element**</span></span>|<span data-ttu-id="ad027-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad027-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad027-116">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ad027-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="ad027-117">Fournit des informations descriptives sur l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ad027-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="ad027-118">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ad027-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="ad027-119">Contient les informations de disponibilité d’un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="ad027-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad027-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad027-120">Parent elements</span></span>

|<span data-ttu-id="ad027-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad027-121">**Element**</span></span>|<span data-ttu-id="ad027-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad027-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad027-123">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ad027-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="ad027-124">Contient les informations de disponibilité des utilisateurs demandés et l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="ad027-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="ad027-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="ad027-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad027-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad027-126">Remarks</span></span>

<span data-ttu-id="ad027-127">Cet élément n’est pas inclus dans une réponse GetUserAvailability si les informations de disponibilité ne sont pas demandées.</span><span class="sxs-lookup"><span data-stu-id="ad027-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="ad027-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ad027-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad027-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad027-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad027-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad027-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad027-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad027-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ad027-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ad027-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad027-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad027-133">Validation File</span></span>  <br/> |<span data-ttu-id="ad027-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ad027-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad027-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad027-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad027-136">False</span><span class="sxs-lookup"><span data-stu-id="ad027-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad027-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad027-137">See also</span></span>



[<span data-ttu-id="ad027-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ad027-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ad027-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ad027-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ad027-140">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="ad027-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

