---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: L’élément GlobalHasIrm spécifie si au moins un message de la conversation et de tous les dossiers est un message protégé par IRM.
ms.openlocfilehash: 10b99c9a6421a89a549b69e918087f3e542ffa09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459468"
---
# <a name="globalhasirm"></a><span data-ttu-id="01273-103">GlobalHasIrm</span><span class="sxs-lookup"><span data-stu-id="01273-103">GlobalHasIrm</span></span>

<span data-ttu-id="01273-104">L’élément **GlobalHasIrm** spécifie si au moins un message de la conversation et de tous les dossiers est un message protégé par IRM.</span><span class="sxs-lookup"><span data-stu-id="01273-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="01273-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="01273-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01273-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="01273-106">Attributes and elements</span></span>

<span data-ttu-id="01273-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="01273-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01273-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="01273-108">Attributes</span></span>

<span data-ttu-id="01273-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="01273-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01273-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="01273-110">Child elements</span></span>

<span data-ttu-id="01273-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="01273-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01273-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="01273-112">Parent elements</span></span>

[<span data-ttu-id="01273-113">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="01273-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="01273-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="01273-114">Text value</span></span>

<span data-ttu-id="01273-115">La valeur de texte de l’élément **GlobalHasIrm** est **true** si au moins un message dans la conversation et tous les dossiers est un message protégé par IRM.</span><span class="sxs-lookup"><span data-stu-id="01273-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="01273-116">Sinon, la valeur est **false**.</span><span class="sxs-lookup"><span data-stu-id="01273-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01273-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="01273-117">Remarks</span></span>

<span data-ttu-id="01273-118">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="01273-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="01273-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="01273-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01273-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="01273-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01273-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="01273-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01273-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="01273-122">Schema Name</span></span>  <br/> |<span data-ttu-id="01273-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="01273-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="01273-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="01273-124">Validation File</span></span>  <br/> |<span data-ttu-id="01273-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01273-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01273-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="01273-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="01273-127">True</span><span class="sxs-lookup"><span data-stu-id="01273-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01273-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="01273-128">See also</span></span>



[<span data-ttu-id="01273-129">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="01273-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="01273-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="01273-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

