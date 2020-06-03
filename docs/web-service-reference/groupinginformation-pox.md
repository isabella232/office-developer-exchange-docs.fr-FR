---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: L’élément GroupingInformation contient une valeur qui est utilisée pour regrouper la boîte aux lettres de l’utilisateur afin de préserver l’affinité lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres.
ms.openlocfilehash: 7cab5d68f7dd5ec1f6caded5b9da6cfee03f3a67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530077"
---
# <a name="groupinginformation-pox"></a><span data-ttu-id="75274-103">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="75274-103">GroupingInformation (POX)</span></span>

<span data-ttu-id="75274-104">L’élément **GroupingInformation** contient une valeur qui est utilisée pour regrouper la boîte aux lettres de l’utilisateur afin de [préserver l’affinité](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="75274-104">The **GroupingInformation** element contains a value that is used to group the user's mailbox to [maintain affinity](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) when subscribing to notifications across multiple mailboxes.</span></span> 
  
[<span data-ttu-id="75274-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="75274-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="75274-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="75274-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="75274-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="75274-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="75274-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="75274-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="75274-109">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="75274-109">GroupingInformation (POX)</span></span>](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="75274-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="75274-110">Attributes and elements</span></span>

<span data-ttu-id="75274-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="75274-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75274-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="75274-112">Attributes</span></span>

<span data-ttu-id="75274-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="75274-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75274-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="75274-114">Child elements</span></span>

<span data-ttu-id="75274-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="75274-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75274-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="75274-116">Parent elements</span></span>

|<span data-ttu-id="75274-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="75274-117">**Element**</span></span>|<span data-ttu-id="75274-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="75274-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75274-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="75274-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="75274-120">Contient les spécifications relatives à la connexion d’un client au serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="75274-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75274-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="75274-121">Text value</span></span>

<span data-ttu-id="75274-122">La valeur de texte est comparée à la valeur de l’élément **GroupingInformation** pour d’autres boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="75274-122">The text value is compared to the value of the **GroupingInformation** element for other mailboxes.</span></span> <span data-ttu-id="75274-123">Les boîtes aux lettres qui ont la même valeur et utilisent le même point de terminaison des services Web Exchange (EWS) peuvent être regroupées pour maintenir l’affinité.</span><span class="sxs-lookup"><span data-stu-id="75274-123">Mailboxes that have the same value and use the same Exchange Web Services (EWS) endpoint can be grouped together to maintain affinity.</span></span> <span data-ttu-id="75274-124">Pour plus d’informations, consultez [la rubrique maintenir l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="75274-124">For more details, see [Maintain affinity between a group of subscriptions and the Mailbox server in Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75274-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="75274-125">Remarks</span></span>

<span data-ttu-id="75274-126">L’élément **GroupingInformation** s’applique uniquement aux éléments de **protocole** qui ont un élément enfant [type (POX)](type-pox.md) avec la valeur « Expr ».</span><span class="sxs-lookup"><span data-stu-id="75274-126">The **GroupingInformation** element is only applicable to **Protocol** elements that have a [Type (POX)](type-pox.md) child element with a value of "EXPR".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="75274-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="75274-127">See also</span></span>

- [<span data-ttu-id="75274-128">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="75274-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
- [<span data-ttu-id="75274-129">Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange</span><span class="sxs-lookup"><span data-stu-id="75274-129">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

