---
title: UpdatedItemIds
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9199aeb2-abdf-40c5-8743-40b61853c951
description: L’élément UpdatedItemIds spécifie les identificateurs des éléments de rappel mis à jour.
ms.openlocfilehash: b95ebb20823706e68b1fd66dc64f756808bb7375
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838859"
---
# <a name="updateditemids"></a><span data-ttu-id="9c035-103">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="9c035-103">UpdatedItemIds</span></span>

<span data-ttu-id="9c035-104">L’élément **UpdatedItemIds** spécifie les identificateurs des éléments de rappel mis à jour.</span><span class="sxs-lookup"><span data-stu-id="9c035-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="9c035-105">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="9c035-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c035-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9c035-106">Attributes and elements</span></span>

<span data-ttu-id="9c035-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9c035-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c035-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9c035-108">Attributes</span></span>

<span data-ttu-id="9c035-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9c035-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c035-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9c035-110">Child elements</span></span>

[<span data-ttu-id="9c035-111">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="9c035-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="9c035-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9c035-112">Parent elements</span></span>

[<span data-ttu-id="9c035-113">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="9c035-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="9c035-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="9c035-114">Remarks</span></span>

<span data-ttu-id="9c035-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9c035-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9c035-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c035-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="9c035-117">Si l’opération [PerformReminderAction](performreminderaction-operation.md) a échoué ou aucune modification effectuée sur le serveur, l’élément **UpdatedItemIds** est renvoyée sous forme de valeur vide.</span><span class="sxs-lookup"><span data-stu-id="9c035-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9c035-118">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9c035-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c035-119">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9c035-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9c035-120">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9c035-120">Schema Name</span></span>  <br/> |<span data-ttu-id="9c035-121">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9c035-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9c035-122">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9c035-122">Validation File</span></span>  <br/> |<span data-ttu-id="9c035-123">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9c035-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c035-124">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9c035-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c035-125">True</span><span class="sxs-lookup"><span data-stu-id="9c035-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c035-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9c035-126">See also</span></span>



[<span data-ttu-id="9c035-127">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="9c035-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="9c035-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9c035-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

