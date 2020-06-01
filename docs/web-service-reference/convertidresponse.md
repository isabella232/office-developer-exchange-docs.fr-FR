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
description: L’élément ConvertIdResponse contient une réponse à une demande ConvertId. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 690f0f2109dfc36dd8f359b7cef1e65beb47fc6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452523"
---
# <a name="convertidresponse"></a><span data-ttu-id="50204-104">ConvertIdResponse</span><span class="sxs-lookup"><span data-stu-id="50204-104">ConvertIdResponse</span></span>

<span data-ttu-id="50204-105">L’élément **ConvertIdResponse** contient une réponse à une demande ConvertId.</span><span class="sxs-lookup"><span data-stu-id="50204-105">The **ConvertIdResponse** element contains a response to a ConvertId request.</span></span> <span data-ttu-id="50204-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="50204-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertIdResponse>
   <ResponseMessages/>
</ConvertIdResponse>
```

 <span data-ttu-id="50204-107">**ConvertIdResponseType**</span><span class="sxs-lookup"><span data-stu-id="50204-107">**ConvertIdResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50204-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="50204-108">Attributes and elements</span></span>

<span data-ttu-id="50204-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="50204-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50204-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="50204-110">Attributes</span></span>

<span data-ttu-id="50204-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="50204-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50204-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="50204-112">Child elements</span></span>

|<span data-ttu-id="50204-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50204-113">**Element**</span></span>|<span data-ttu-id="50204-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="50204-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50204-115">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="50204-115">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="50204-116">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="50204-116">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50204-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="50204-117">Parent elements</span></span>

<span data-ttu-id="50204-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="50204-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="50204-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="50204-119">Remarks</span></span>

<span data-ttu-id="50204-120">Les messages de réponse contenus dans l’élément [ResponseMessages](responsemessages.md) seront des instances de ConvertIdResponseMessageType.</span><span class="sxs-lookup"><span data-stu-id="50204-120">The response messages that are contained within the [ResponseMessages](responsemessages.md) element will be instances of ConvertIdResponseMessageType.</span></span> 
  
<span data-ttu-id="50204-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="50204-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50204-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="50204-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50204-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="50204-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50204-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="50204-124">Schema Name</span></span>  <br/> |<span data-ttu-id="50204-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="50204-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="50204-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="50204-126">Validation File</span></span>  <br/> |<span data-ttu-id="50204-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="50204-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50204-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="50204-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="50204-129">False</span><span class="sxs-lookup"><span data-stu-id="50204-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50204-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="50204-130">See also</span></span>



[<span data-ttu-id="50204-131">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="50204-131">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="50204-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="50204-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="50204-133">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="50204-133">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

