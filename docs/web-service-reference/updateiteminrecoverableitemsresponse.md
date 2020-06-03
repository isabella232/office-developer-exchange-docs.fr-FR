---
title: UpdateItemInRecoverableItemsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2f61b038-eba0-40fc-8af2-c3db5cc5a420
description: L’élément UpdateItemInRecoverableItemsResponse spécifie la réponse à une demande UpdateItemInRecoverableItems.
ms.openlocfilehash: 02e030774949e895bc89579cb9364d08c7844ce3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466555"
---
# <a name="updateiteminrecoverableitemsresponse"></a><span data-ttu-id="b7d44-103">UpdateItemInRecoverableItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b7d44-103">UpdateItemInRecoverableItemsResponse</span></span>

<span data-ttu-id="b7d44-104">L’élément **UpdateItemInRecoverableItemsResponse** spécifie la réponse à une demande **UpdateItemInRecoverableItems** .</span><span class="sxs-lookup"><span data-stu-id="b7d44-104">The **UpdateItemInRecoverableItemsResponse** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
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

 <span data-ttu-id="b7d44-105">**UpdateItemInRecoverableItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b7d44-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7d44-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b7d44-106">Attributes and elements</span></span>

<span data-ttu-id="b7d44-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b7d44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7d44-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b7d44-108">Attributes</span></span>

<span data-ttu-id="b7d44-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b7d44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7d44-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b7d44-110">Child elements</span></span>

<span data-ttu-id="b7d44-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [Éléments](items.md)  |  [Pièces jointes](attachments-ex15websvcsotherref.md)  |  [ConflictResults](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="b7d44-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7d44-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b7d44-112">Parent elements</span></span>

<span data-ttu-id="b7d44-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7d44-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b7d44-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="b7d44-114">Remarks</span></span>

<span data-ttu-id="b7d44-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b7d44-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b7d44-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7d44-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7d44-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b7d44-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7d44-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b7d44-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b7d44-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b7d44-119">Schema name</span></span>  <br/> |<span data-ttu-id="b7d44-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b7d44-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b7d44-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b7d44-121">Validation file</span></span>  <br/> |<span data-ttu-id="b7d44-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b7d44-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7d44-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b7d44-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b7d44-124">false</span><span class="sxs-lookup"><span data-stu-id="b7d44-124">false</span></span>  <br/> |
   

