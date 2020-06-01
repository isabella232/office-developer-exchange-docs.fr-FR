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
description: L’élément GetMailTipsResponse représente le message de réponse pour une opération GetMailTips.
ms.openlocfilehash: 2c0dcfe4e2deddcf9a6f4bb9d68d59115c171796
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458606"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="b3668-103">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="b3668-103">GetMailTipsResponse</span></span>

<span data-ttu-id="b3668-104">L’élément **GetMailTipsResponse** représente le message de réponse pour une [opération GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b3668-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="b3668-105">**GetMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b3668-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3668-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b3668-106">Attributes and elements</span></span>

<span data-ttu-id="b3668-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b3668-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3668-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b3668-108">Attributes</span></span>

<span data-ttu-id="b3668-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b3668-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3668-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b3668-110">Child elements</span></span>

|<span data-ttu-id="b3668-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3668-111">**Element**</span></span>|<span data-ttu-id="b3668-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3668-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3668-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="b3668-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="b3668-114">Représente une liste de messages de réponse à des conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="b3668-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3668-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b3668-115">Parent elements</span></span>

<span data-ttu-id="b3668-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3668-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b3668-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b3668-117">Text value</span></span>

<span data-ttu-id="b3668-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3668-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b3668-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="b3668-119">Remarks</span></span>

<span data-ttu-id="b3668-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3668-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3668-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b3668-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3668-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b3668-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b3668-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b3668-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b3668-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b3668-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b3668-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b3668-125">Validation File</span></span>  <br/> |<span data-ttu-id="b3668-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b3668-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b3668-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b3668-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3668-128">False</span><span class="sxs-lookup"><span data-stu-id="b3668-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3668-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3668-129">See also</span></span>



[<span data-ttu-id="b3668-130">Opération GetMailTips</span><span class="sxs-lookup"><span data-stu-id="b3668-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="b3668-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b3668-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

