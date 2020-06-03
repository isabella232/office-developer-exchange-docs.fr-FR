---
title: UpdateItemInRecoverableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c49816b1-dbb5-4716-86c7-30790e86f30e
description: L’élément UpdateItemInRecoverableItems spécifie une demande de mise à jour d’un élément dans les éléments récupérables.
ms.openlocfilehash: f3dae55097c613b84a80795185baad559e312b90
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459783"
---
# <a name="updateiteminrecoverableitems"></a><span data-ttu-id="de9e6-103">UpdateItemInRecoverableItems</span><span class="sxs-lookup"><span data-stu-id="de9e6-103">UpdateItemInRecoverableItems</span></span>

<span data-ttu-id="de9e6-104">L’élément **UpdateItemInRecoverableItems** spécifie une demande de mise à jour d’un élément dans les éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="de9e6-104">The **UpdateItemInRecoverableItems** element specifies a request to update an item in recoverable items.</span></span> 
  
```XML
<UpdateItemInRecoverableItems>
   <ItemId/>
   <Updates/>
   <Attachments/>
   <MakeItemImmutable/>
</UpdateItemInRecoverableItems>
```

 <span data-ttu-id="de9e6-105">**UpdateItemInRecoverableItemsType**</span><span class="sxs-lookup"><span data-stu-id="de9e6-105">**UpdateItemInRecoverableItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de9e6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de9e6-106">Attributes and elements</span></span>

<span data-ttu-id="de9e6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de9e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de9e6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="de9e6-108">Attributes</span></span>

<span data-ttu-id="de9e6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="de9e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de9e6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de9e6-110">Child elements</span></span>

<span data-ttu-id="de9e6-111">[ItemId](itemid.md)  |  [Mises à jour (élément)](updates-item.md)  |  [Pièces jointes](attachments-ex15websvcsotherref.md)  |  [MakeItemImmutable](makeitemimmutable.md)</span><span class="sxs-lookup"><span data-stu-id="de9e6-111">[ItemId](itemid.md) | [Updates (Item)](updates-item.md) | [Attachments](attachments-ex15websvcsotherref.md) | [MakeItemImmutable](makeitemimmutable.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de9e6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de9e6-112">Parent elements</span></span>

<span data-ttu-id="de9e6-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="de9e6-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de9e6-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="de9e6-114">Remarks</span></span>

<span data-ttu-id="de9e6-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="de9e6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="de9e6-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="de9e6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de9e6-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de9e6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de9e6-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de9e6-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de9e6-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de9e6-119">Schema name</span></span>  <br/> |<span data-ttu-id="de9e6-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="de9e6-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="de9e6-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de9e6-121">Validation file</span></span>  <br/> |<span data-ttu-id="de9e6-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="de9e6-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de9e6-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de9e6-123">Can be empty</span></span>  <br/> |<span data-ttu-id="de9e6-124">false</span><span class="sxs-lookup"><span data-stu-id="de9e6-124">false</span></span>  <br/> |
   

