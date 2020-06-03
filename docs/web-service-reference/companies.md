---
title: Sociétés
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
description: L’élément Companies représente la collection de sociétés associées à un contact ou une tâche.
ms.openlocfilehash: eda2b92f3ca874aeeceef6a0935a49a98af0ec39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461449"
---
# <a name="companies"></a><span data-ttu-id="cf408-103">Sociétés</span><span class="sxs-lookup"><span data-stu-id="cf408-103">Companies</span></span>

<span data-ttu-id="cf408-104">L’élément **Companies** représente la collection de sociétés associées à un contact ou une tâche.</span><span class="sxs-lookup"><span data-stu-id="cf408-104">The **Companies** element represents the collection of companies that are associated with a contact or task.</span></span> 
  
```xml
<Companies>
   <String/>
</Companies>
```

 <span data-ttu-id="cf408-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="cf408-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf408-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cf408-106">Attributes and elements</span></span>

<span data-ttu-id="cf408-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cf408-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf408-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cf408-108">Attributes</span></span>

<span data-ttu-id="cf408-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cf408-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf408-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cf408-110">Child elements</span></span>

|<span data-ttu-id="cf408-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf408-111">**Element**</span></span>|<span data-ttu-id="cf408-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf408-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf408-113">String</span><span class="sxs-lookup"><span data-stu-id="cf408-113">String</span></span>](string.md) <br/> |<span data-ttu-id="cf408-114">Représente le nom d’une société.</span><span class="sxs-lookup"><span data-stu-id="cf408-114">Represents the name of a company.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf408-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cf408-115">Parent elements</span></span>

|<span data-ttu-id="cf408-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf408-116">**Element**</span></span>|<span data-ttu-id="cf408-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf408-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf408-118">Contact</span><span class="sxs-lookup"><span data-stu-id="cf408-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="cf408-119">Représente un contact dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf408-119">Represents a contact in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="cf408-120">Tâche</span><span class="sxs-lookup"><span data-stu-id="cf408-120">Task</span></span>](task.md) <br/> |<span data-ttu-id="cf408-121">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf408-121">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf408-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="cf408-122">Remarks</span></span>

<span data-ttu-id="cf408-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cf408-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf408-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cf408-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf408-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cf408-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf408-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cf408-126">Schema name</span></span>  <br/> |<span data-ttu-id="cf408-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cf408-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf408-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cf408-128">Validation file</span></span>  <br/> |<span data-ttu-id="cf408-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf408-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf408-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cf408-130">Can be empty</span></span>  <br/> |<span data-ttu-id="cf408-131">False</span><span class="sxs-lookup"><span data-stu-id="cf408-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf408-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf408-132">See also</span></span>



- [<span data-ttu-id="cf408-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cf408-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

