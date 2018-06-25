---
title: GetMailTipsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTipsResponse
api_type:
- schema
ms.assetid: fe270e34-566e-4f9e-9e73-fbf38e06436d
description: L’élément GetMailTipsResponse représente le message de réponse d’une opération de GetMailTips.
ms.openlocfilehash: e7a18e8818761af931d32b26aeaf58a2853fa684
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756671"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="28544-103">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="28544-103">GetMailTipsResponse</span></span>

<span data-ttu-id="28544-104">L’élément **GetMailTipsResponse** représente le message de réponse d’une [opération GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="28544-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="28544-105">**GetMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="28544-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28544-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28544-106">Attributes and elements</span></span>

<span data-ttu-id="28544-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28544-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28544-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="28544-108">Attributes</span></span>

<span data-ttu-id="28544-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28544-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28544-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28544-110">Child elements</span></span>

|<span data-ttu-id="28544-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28544-111">**Element**</span></span>|<span data-ttu-id="28544-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="28544-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28544-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="28544-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="28544-114">Représente une liste des messages de réponse de conseils.</span><span class="sxs-lookup"><span data-stu-id="28544-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28544-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28544-115">Parent elements</span></span>

<span data-ttu-id="28544-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28544-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="28544-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="28544-117">Text value</span></span>

<span data-ttu-id="28544-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28544-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28544-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="28544-119">Remarks</span></span>

<span data-ttu-id="28544-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="28544-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28544-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28544-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28544-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28544-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28544-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28544-123">Schema Name</span></span>  <br/> |<span data-ttu-id="28544-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="28544-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28544-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28544-125">Validation File</span></span>  <br/> |<span data-ttu-id="28544-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="28544-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28544-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28544-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="28544-128">False</span><span class="sxs-lookup"><span data-stu-id="28544-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28544-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28544-129">See also</span></span>



[<span data-ttu-id="28544-130">Opération GetMailTips</span><span class="sxs-lookup"><span data-stu-id="28544-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="28544-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="28544-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

