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
description: L’élément FreeBusyResponseArray contient les informations de disponibilité des utilisateurs demandés et l’état de la réponse.
ms.openlocfilehash: b45938c19b76a377fca125fb6a19f9d712718db6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457808"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="0c1d2-103">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="0c1d2-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="0c1d2-104">L’élément **FreeBusyResponseArray** contient les informations de disponibilité des utilisateurs demandés et l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="0c1d2-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="0c1d2-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0c1d2-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="0c1d2-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="0c1d2-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="0c1d2-107">**ArrayOfFreeBusyResponse**</span><span class="sxs-lookup"><span data-stu-id="0c1d2-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c1d2-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0c1d2-108">Attributes and elements</span></span>

<span data-ttu-id="0c1d2-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0c1d2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c1d2-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="0c1d2-110">Attributes</span></span>

<span data-ttu-id="0c1d2-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0c1d2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c1d2-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0c1d2-112">Child elements</span></span>

|<span data-ttu-id="0c1d2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0c1d2-113">**Element**</span></span>|<span data-ttu-id="0c1d2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0c1d2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c1d2-115">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="0c1d2-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="0c1d2-116">Contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique et l’état de réponse.</span><span class="sxs-lookup"><span data-stu-id="0c1d2-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c1d2-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0c1d2-117">Parent elements</span></span>

|<span data-ttu-id="0c1d2-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0c1d2-118">**Element**</span></span>|<span data-ttu-id="0c1d2-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="0c1d2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c1d2-120">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0c1d2-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="0c1d2-121">Contient les propriétés qui définissent les informations de disponibilité de l’utilisateur ou les informations sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="0c1d2-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="0c1d2-122">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="0c1d2-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0c1d2-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="0c1d2-123">Remarks</span></span>

<span data-ttu-id="0c1d2-124">Cet élément n’est pas inclus dans une réponse GetUserAvailability si les informations de disponibilité ne sont pas demandées.</span><span class="sxs-lookup"><span data-stu-id="0c1d2-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="0c1d2-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0c1d2-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c1d2-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0c1d2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c1d2-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0c1d2-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0c1d2-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0c1d2-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0c1d2-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0c1d2-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0c1d2-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0c1d2-130">Validation File</span></span>  <br/> |<span data-ttu-id="0c1d2-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0c1d2-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c1d2-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0c1d2-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c1d2-133">False</span><span class="sxs-lookup"><span data-stu-id="0c1d2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c1d2-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0c1d2-134">See also</span></span>



[<span data-ttu-id="0c1d2-135">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0c1d2-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0c1d2-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0c1d2-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0c1d2-137">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="0c1d2-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

