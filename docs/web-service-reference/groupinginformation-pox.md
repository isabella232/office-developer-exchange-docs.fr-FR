---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: L’élément GroupingInformation contient une valeur qui est utilisée pour la boîte aux lettres de l’utilisateur pour maintenir l’affinité lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres de groupe.
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827781"
---
# <a name="groupinginformation-pox"></a><span data-ttu-id="f1da8-103">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="f1da8-103">GroupingInformation (POX)</span></span>

<span data-ttu-id="f1da8-104">L’élément **GroupingInformation** contient une valeur qui est utilisée pour regrouper les boîtes aux lettres de l’utilisateur à [mettre à jour l’affinité](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) lors de l’abonnement aux notifications entre plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1da8-104">The **GroupingInformation** element contains a value that is used to group the user's mailbox to [maintain affinity](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) when subscribing to notifications across multiple mailboxes.</span></span> 
  
[<span data-ttu-id="f1da8-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="f1da8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f1da8-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="f1da8-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f1da8-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="f1da8-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f1da8-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="f1da8-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f1da8-109">GroupingInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="f1da8-109">GroupingInformation (POX)</span></span>](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f1da8-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1da8-110">Attributes and elements</span></span>

<span data-ttu-id="f1da8-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1da8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1da8-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1da8-112">Attributes</span></span>

<span data-ttu-id="f1da8-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f1da8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1da8-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1da8-114">Child elements</span></span>

<span data-ttu-id="f1da8-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f1da8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1da8-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1da8-116">Parent elements</span></span>

|<span data-ttu-id="f1da8-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1da8-117">**Element**</span></span>|<span data-ttu-id="f1da8-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1da8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1da8-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="f1da8-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f1da8-120">Contient les spécifications pour la connexion d’un client sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1da8-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1da8-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f1da8-121">Text value</span></span>

<span data-ttu-id="f1da8-122">La valeur de texte est comparée à la valeur de l’élément **GroupingInformation** pour d’autres boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1da8-122">The text value is compared to the value of the **GroupingInformation** element for other mailboxes.</span></span> <span data-ttu-id="f1da8-123">Boîtes aux lettres qui ont la même valeur et utilisent le même point de terminaison Exchange Web Services (EWS) peuvent être regroupés pour maintenir l’affinité.</span><span class="sxs-lookup"><span data-stu-id="f1da8-123">Mailboxes that have the same value and use the same Exchange Web Services (EWS) endpoint can be grouped together to maintain affinity.</span></span> <span data-ttu-id="f1da8-124">Pour plus d’informations, voir [mettre à jour l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f1da8-124">For more details, see [Maintain affinity between a group of subscriptions and the Mailbox server in Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1da8-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="f1da8-125">Remarks</span></span>

<span data-ttu-id="f1da8-126">L’élément **GroupingInformation** est uniquement applicable à des éléments de **protocole** qui ont un élément enfant de [Type (POX)](type-pox.md) avec la valeur « EXPR ».</span><span class="sxs-lookup"><span data-stu-id="f1da8-126">The **GroupingInformation** element is only applicable to **Protocol** elements that have a [Type (POX)](type-pox.md) child element with a value of "EXPR".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f1da8-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1da8-127">See also</span></span>

- [<span data-ttu-id="f1da8-128">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="f1da8-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
- [<span data-ttu-id="f1da8-129">Conserve les affinités entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f1da8-129">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

