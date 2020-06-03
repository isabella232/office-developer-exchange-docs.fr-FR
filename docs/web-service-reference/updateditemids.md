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
ms.openlocfilehash: 4a87bf50f90e80c0c887ee3a66b9f201ea1c8440
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465035"
---
# <a name="updateditemids"></a><span data-ttu-id="4fe99-103">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="4fe99-103">UpdatedItemIds</span></span>

<span data-ttu-id="4fe99-104">L’élément **UpdatedItemIds** spécifie les identificateurs des éléments de rappel mis à jour.</span><span class="sxs-lookup"><span data-stu-id="4fe99-104">The **UpdatedItemIds** element specifies the identifiers of updated reminder items.</span></span> 
  
```XML
<UpdatedItemIds>
   <ItemId></ItemId>
</UpdatedItemIds>

```

 <span data-ttu-id="4fe99-105">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="4fe99-105">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fe99-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4fe99-106">Attributes and elements</span></span>

<span data-ttu-id="4fe99-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4fe99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fe99-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4fe99-108">Attributes</span></span>

<span data-ttu-id="4fe99-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4fe99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fe99-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4fe99-110">Child elements</span></span>

[<span data-ttu-id="4fe99-111">ItemId</span><span class="sxs-lookup"><span data-stu-id="4fe99-111">ItemId</span></span>](itemid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="4fe99-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4fe99-112">Parent elements</span></span>

[<span data-ttu-id="4fe99-113">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="4fe99-113">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="4fe99-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="4fe99-114">Remarks</span></span>

<span data-ttu-id="4fe99-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4fe99-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4fe99-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fe99-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="4fe99-117">Si l’opération [PerformReminderAction](performreminderaction-operation.md) ne s’est pas terminée correctement ou qu’aucune modification n’a été apportée sur le serveur, l’élément **UpdatedItemIds** est renvoyé sous la forme d’une valeur vide.</span><span class="sxs-lookup"><span data-stu-id="4fe99-117">If the [PerformReminderAction](performreminderaction-operation.md) operation did not complete successfully, or no changes were made on the server, the **UpdatedItemIds** element is returned as an empty value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4fe99-118">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4fe99-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fe99-119">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4fe99-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4fe99-120">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4fe99-120">Schema Name</span></span>  <br/> |<span data-ttu-id="4fe99-121">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4fe99-121">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4fe99-122">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4fe99-122">Validation File</span></span>  <br/> |<span data-ttu-id="4fe99-123">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4fe99-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4fe99-124">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4fe99-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fe99-125">True</span><span class="sxs-lookup"><span data-stu-id="4fe99-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fe99-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4fe99-126">See also</span></span>



[<span data-ttu-id="4fe99-127">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="4fe99-127">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)


- [<span data-ttu-id="4fe99-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4fe99-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

