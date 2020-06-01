---
title: Domaine (suivi des messages)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 4e8e9efa-8885-4ca5-bf90-424e63768dc3
description: L’élément Domain représente le domaine à rechercher.
ms.openlocfilehash: 77da9028766881b9bc633e1b3318cd4d70c6b72f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457024"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="5f85c-103">Domaine (suivi des messages)</span><span class="sxs-lookup"><span data-stu-id="5f85c-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="5f85c-104">L’élément **Domain** représente le domaine à rechercher.</span><span class="sxs-lookup"><span data-stu-id="5f85c-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="5f85c-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="5f85c-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f85c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5f85c-106">Attributes and elements</span></span>

<span data-ttu-id="5f85c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5f85c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f85c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5f85c-108">Attributes</span></span>

<span data-ttu-id="5f85c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5f85c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f85c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5f85c-110">Child elements</span></span>

<span data-ttu-id="5f85c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5f85c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f85c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5f85c-112">Parent elements</span></span>

|<span data-ttu-id="5f85c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5f85c-113">**Element**</span></span>|<span data-ttu-id="5f85c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5f85c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f85c-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="5f85c-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="5f85c-116">Contient des critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="5f85c-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f85c-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5f85c-117">Text value</span></span>

<span data-ttu-id="5f85c-118">Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="5f85c-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f85c-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="5f85c-119">Remarks</span></span>

<span data-ttu-id="5f85c-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f85c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f85c-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5f85c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f85c-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5f85c-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5f85c-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5f85c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5f85c-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5f85c-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5f85c-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5f85c-125">Validation File</span></span>  <br/> |<span data-ttu-id="5f85c-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5f85c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5f85c-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5f85c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f85c-128">False</span><span class="sxs-lookup"><span data-stu-id="5f85c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f85c-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5f85c-129">See also</span></span>

- [<span data-ttu-id="5f85c-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5f85c-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

