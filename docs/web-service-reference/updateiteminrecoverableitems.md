---
title: UpdateItemInRecoverableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c49816b1-dbb5-4716-86c7-30790e86f30e
description: L’élément UpdateItemInRecoverableItems spécifie une requête pour mettre à jour un élément d’éléments récupérables.
ms.openlocfilehash: 768de4bb8abe4780ab520405bae3149b8f17637c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838885"
---
# <a name="updateiteminrecoverableitems"></a><span data-ttu-id="93186-103">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="93186-103">UpdateItemInRecoverableItems</span></span>

<span data-ttu-id="93186-104">L’élément **UpdateItemInRecoverableItems** spécifie une requête pour mettre à jour un élément d’éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="93186-104">The **UpdateItemInRecoverableItems** element specifies a request to update an item in recoverable items.</span></span> 
  
```XML
<UpdateItemInRecoverableItems>
   <ItemId/>
   <Updates/>
   <Attachments/>
   <MakeItemImmutable/>
</UpdateItemInRecoverableItems>
```

 <span data-ttu-id="93186-105">**UpdateItemInRecoverableItemsType**</span><span class="sxs-lookup"><span data-stu-id="93186-105">**UpdateItemInRecoverableItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93186-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="93186-106">Attributes and elements</span></span>

<span data-ttu-id="93186-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="93186-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93186-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="93186-108">Attributes</span></span>

<span data-ttu-id="93186-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="93186-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93186-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="93186-110">Child elements</span></span>

<span data-ttu-id="93186-111">[ItemId](itemid.md) | [mises à jour (élément)](updates-item.md) | [pièces jointes](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span><span class="sxs-lookup"><span data-stu-id="93186-111">[ItemId](itemid.md) | [Updates (Item)](updates-item.md) | [Attachments](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93186-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="93186-112">Parent elements</span></span>

<span data-ttu-id="93186-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="93186-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93186-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="93186-114">Remarks</span></span>

<span data-ttu-id="93186-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="93186-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93186-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="93186-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93186-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="93186-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93186-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="93186-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93186-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="93186-119">Schema name</span></span>  <br/> |<span data-ttu-id="93186-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="93186-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93186-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="93186-121">Validation file</span></span>  <br/> |<span data-ttu-id="93186-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="93186-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93186-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="93186-123">Can be empty</span></span>  <br/> |<span data-ttu-id="93186-124">false</span><span class="sxs-lookup"><span data-stu-id="93186-124">false</span></span>  <br/> |
   

