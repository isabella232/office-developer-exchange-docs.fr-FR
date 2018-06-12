---
title: ConvertIdResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponse
api_type:
- schema
ms.assetid: ac1f044f-04a4-42ef-b762-cac5cd37894d
description: L’élément ConvertIdResponse contient une réponse à une demande de ConvertId. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 80299afebcebf15546b0fdbe14f0b08960527a47
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755654"
---
# <a name="convertidresponse"></a><span data-ttu-id="0b12a-104">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="0b12a-104">ConvertIdResponse</span></span>

<span data-ttu-id="0b12a-105">L’élément **ConvertIdResponse** contient une réponse à une demande de ConvertId.</span><span class="sxs-lookup"><span data-stu-id="0b12a-105">The **ConvertIdResponse** element contains a response to a ConvertId request.</span></span> <span data-ttu-id="0b12a-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0b12a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertIdResponse>
   <ResponseMessages/>
</ConvertIdResponse>
```

 <span data-ttu-id="0b12a-107">**ConvertIdResponseType**</span><span class="sxs-lookup"><span data-stu-id="0b12a-107">**ConvertIdResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b12a-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0b12a-108">Attributes and elements</span></span>

<span data-ttu-id="0b12a-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0b12a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b12a-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="0b12a-110">Attributes</span></span>

<span data-ttu-id="0b12a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0b12a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b12a-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0b12a-112">Child elements</span></span>

|<span data-ttu-id="0b12a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0b12a-113">**Element**</span></span>|<span data-ttu-id="0b12a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0b12a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b12a-115">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0b12a-115">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0b12a-116">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b12a-116">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b12a-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0b12a-117">Parent elements</span></span>

<span data-ttu-id="0b12a-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0b12a-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b12a-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="0b12a-119">Remarks</span></span>

<span data-ttu-id="0b12a-120">Les messages de réponse qui sont contenues dans l’élément [ResponseMessages](responsemessages.md) seront des instances de ConvertIdResponseMessageType.</span><span class="sxs-lookup"><span data-stu-id="0b12a-120">The response messages that are contained within the [ResponseMessages](responsemessages.md) element will be instances of ConvertIdResponseMessageType.</span></span> 
  
<span data-ttu-id="0b12a-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0b12a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b12a-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0b12a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b12a-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0b12a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b12a-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0b12a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0b12a-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0b12a-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0b12a-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0b12a-126">Validation File</span></span>  <br/> |<span data-ttu-id="0b12a-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0b12a-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b12a-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0b12a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b12a-129">False</span><span class="sxs-lookup"><span data-stu-id="0b12a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b12a-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0b12a-130">See also</span></span>



[<span data-ttu-id="0b12a-131">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="0b12a-131">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="0b12a-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b12a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0b12a-133">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="0b12a-133">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

