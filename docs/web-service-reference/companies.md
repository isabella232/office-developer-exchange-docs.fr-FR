---
title: Companies
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Companies
api_type:
- schema
ms.assetid: 5d9ea76f-e14d-4424-8842-0c3cc3305119
description: L’élément sociétés représente la collection des sociétés qui sont associés à un contact ou une tâche.
ms.openlocfilehash: 5b8ac20d4a02017881f941d12380fe29078f51cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755516"
---
# <a name="companies"></a><span data-ttu-id="19565-103">Companies</span><span class="sxs-lookup"><span data-stu-id="19565-103">Companies</span></span>

<span data-ttu-id="19565-104">L’élément **sociétés** représente la collection des sociétés qui sont associés à un contact ou une tâche.</span><span class="sxs-lookup"><span data-stu-id="19565-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="19565-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="19565-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19565-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="19565-106">Attributes and elements</span></span>

<span data-ttu-id="19565-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="19565-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19565-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="19565-108">Attributes</span></span>

<span data-ttu-id="19565-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="19565-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19565-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="19565-110">Child elements</span></span>

|<span data-ttu-id="19565-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="19565-111">**Element**</span></span>|<span data-ttu-id="19565-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="19565-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19565-113">String</span><span class="sxs-lookup"><span data-stu-id="19565-113">String</span></span>](string.md) <br/> |<span data-ttu-id="19565-114">Représente le nom d’une société.</span><span class="sxs-lookup"><span data-stu-id="19565-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19565-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="19565-115">Parent elements</span></span>

|<span data-ttu-id="19565-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="19565-116">**Element**</span></span>|<span data-ttu-id="19565-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="19565-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19565-118">Contact</span><span class="sxs-lookup"><span data-stu-id="19565-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="19565-119">Représente un contact dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="19565-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="19565-120">Tâche</span><span class="sxs-lookup"><span data-stu-id="19565-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="19565-121">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="19565-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="19565-122">Note</span><span class="sxs-lookup"><span data-stu-id="19565-122">Remarks</span></span>

<span data-ttu-id="19565-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="19565-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19565-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="19565-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19565-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="19565-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="19565-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="19565-126">Schema name</span></span>  <br/> |<span data-ttu-id="19565-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="19565-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="19565-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="19565-128">Validation file</span></span>  <br/> |<span data-ttu-id="19565-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="19565-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="19565-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="19565-130">Can be empty</span></span>  <br/> |<span data-ttu-id="19565-131">False</span><span class="sxs-lookup"><span data-stu-id="19565-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19565-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="19565-132">See also</span></span>



- [<span data-ttu-id="19565-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="19565-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

