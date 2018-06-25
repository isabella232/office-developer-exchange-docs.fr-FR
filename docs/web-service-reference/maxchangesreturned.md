---
title: MaxChangesReturned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: L’élément MaxChangesReturned décrit le nombre maximal de modifications pouvant être renvoyés dans une réponse de la synchronisation.
ms.openlocfilehash: c3719b12b7e3e2f83a9454c7b68432b375d78614
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828395"
---
# <a name="maxchangesreturned"></a><span data-ttu-id="9533f-103">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="9533f-103">MaxChangesReturned</span></span>

<span data-ttu-id="9533f-104">L’élément **MaxChangesReturned** décrit le nombre maximal de modifications pouvant être renvoyés dans une réponse de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="9533f-104">The **MaxChangesReturned** element describes the maximum number of changes that can be returned in a synchronization response.</span></span> 
  
[<span data-ttu-id="9533f-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9533f-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="9533f-106">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="9533f-106">MaxChangesReturned</span></span>](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 <span data-ttu-id="9533f-107">**int**</span><span class="sxs-lookup"><span data-stu-id="9533f-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9533f-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9533f-108">Attributes and elements</span></span>

<span data-ttu-id="9533f-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9533f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9533f-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9533f-110">Attributes</span></span>

<span data-ttu-id="9533f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9533f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9533f-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9533f-112">Child elements</span></span>

<span data-ttu-id="9533f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9533f-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9533f-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9533f-114">Parent elements</span></span>

|<span data-ttu-id="9533f-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9533f-115">**Element**</span></span>|<span data-ttu-id="9533f-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="9533f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9533f-117">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9533f-117">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="9533f-118">Définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="9533f-118">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9533f-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9533f-119">Text value</span></span>

<span data-ttu-id="9533f-120">La valeur de texte représente un entier qui décrit le nombre maximal d’éléments qui sont retournés dans un appel de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="9533f-120">The text value represents an integer that describes the maximum number of items that are returned in a single synchronization call.</span></span> <span data-ttu-id="9533f-121">La valeur doit être comprise entre 1 et 512, inclus.</span><span class="sxs-lookup"><span data-stu-id="9533f-121">The value must be between 1 and 512, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9533f-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="9533f-122">Remarks</span></span>

<span data-ttu-id="9533f-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9533f-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9533f-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9533f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9533f-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9533f-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9533f-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9533f-126">Schema name</span></span>  <br/> |<span data-ttu-id="9533f-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9533f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="9533f-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9533f-128">Validation file</span></span>  <br/> |<span data-ttu-id="9533f-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9533f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9533f-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9533f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="9533f-131">False</span><span class="sxs-lookup"><span data-stu-id="9533f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9533f-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9533f-132">See also</span></span>



[<span data-ttu-id="9533f-133">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9533f-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="9533f-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9533f-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

