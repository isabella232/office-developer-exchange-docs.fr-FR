---
title: UpdateItemInRecoverableItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96259756-322e-4c24-ac76-0cd9c32e0d6d
description: L’élément UpdateItemInRecoverableItemsResponseMessage spécifie la réponse à une demande UpdateItemInRecoverableItems.
ms.openlocfilehash: 021631f5c30eebbf4d7ae0aad35a85b99a23925f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466534"
---
# <a name="updateiteminrecoverableitemsresponsemessage"></a><span data-ttu-id="d8dca-103">UpdateItemInRecoverableItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d8dca-103">UpdateItemInRecoverableItemsResponseMessage</span></span>

<span data-ttu-id="d8dca-104">L’élément **UpdateItemInRecoverableItemsResponseMessage** spécifie la réponse à une demande **UpdateItemInRecoverableItems** .</span><span class="sxs-lookup"><span data-stu-id="d8dca-104">The **UpdateItemInRecoverableItemsResponseMessage** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKet/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponseMessage>
```

 <span data-ttu-id="d8dca-105">**UpdateItemInRecoverableItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d8dca-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8dca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d8dca-106">Attributes and elements</span></span>

<span data-ttu-id="d8dca-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d8dca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8dca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d8dca-108">Attributes</span></span>

<span data-ttu-id="d8dca-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d8dca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8dca-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d8dca-110">Child elements</span></span>

<span data-ttu-id="d8dca-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [Éléments](items.md)  |  [Pièces jointes](attachments-ex15websvcsotherref.md)  |  [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="d8dca-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8dca-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d8dca-112">Parent elements</span></span>

<span data-ttu-id="d8dca-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d8dca-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8dca-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="d8dca-114">Remarks</span></span>

<span data-ttu-id="d8dca-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8dca-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8dca-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8dca-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8dca-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d8dca-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8dca-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d8dca-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="d8dca-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d8dca-119">Schema name</span></span>  <br/> |<span data-ttu-id="d8dca-120">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="d8dca-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="d8dca-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d8dca-121">Validation file</span></span>  <br/> |<span data-ttu-id="d8dca-122">Message. xsd</span><span class="sxs-lookup"><span data-stu-id="d8dca-122">Message.xsd</span></span>  <br/> |
|<span data-ttu-id="d8dca-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d8dca-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d8dca-124">false</span><span class="sxs-lookup"><span data-stu-id="d8dca-124">false</span></span>  <br/> |
   

