---
title: UpdateItemInRecoverableItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2f61b038-eba0-40fc-8af2-c3db5cc5a420
description: L’élément UpdateItemInRecoverableItemsResponse spécifie la réponse à une demande de UpdateItemInRecoverableItems.
ms.openlocfilehash: 2cb9bcb2752599a546c1391d6ea306735b3b0c78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838890"
---
# <a name="updateiteminrecoverableitemsresponse"></a><span data-ttu-id="b69f5-103">UpdateItemInRecoverableItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b69f5-103">UpdateItemInRecoverableItemsResponse</span></span>

<span data-ttu-id="b69f5-104">L’élément **UpdateItemInRecoverableItemsResponse** spécifie la réponse à une demande de **UpdateItemInRecoverableItems** .</span><span class="sxs-lookup"><span data-stu-id="b69f5-104">The **UpdateItemInRecoverableItemsResponse** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponse>
```

 <span data-ttu-id="b69f5-105">**UpdateItemInRecoverableItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b69f5-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b69f5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b69f5-106">Attributes and elements</span></span>

<span data-ttu-id="b69f5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b69f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b69f5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b69f5-108">Attributes</span></span>

<span data-ttu-id="b69f5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b69f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b69f5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b69f5-110">Child elements</span></span>

<span data-ttu-id="b69f5-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [éléments](items.md) | [pièces jointes](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="b69f5-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b69f5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b69f5-112">Parent elements</span></span>

<span data-ttu-id="b69f5-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b69f5-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b69f5-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="b69f5-114">Remarks</span></span>

<span data-ttu-id="b69f5-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b69f5-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b69f5-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b69f5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b69f5-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b69f5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b69f5-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b69f5-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b69f5-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b69f5-119">Schema name</span></span>  <br/> |<span data-ttu-id="b69f5-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b69f5-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b69f5-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b69f5-121">Validation file</span></span>  <br/> |<span data-ttu-id="b69f5-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b69f5-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b69f5-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b69f5-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b69f5-124">false</span><span class="sxs-lookup"><span data-stu-id="b69f5-124">false</span></span>  <br/> |
   

