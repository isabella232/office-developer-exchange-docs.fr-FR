---
title: GetCallInfo (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 2758904d-ffb0-46ee-a134-e6394276996c
description: L’élément GetCallInfo définit une demande pour obtenir des informations relatives à un appel.
ms.openlocfilehash: 749a47abf4dd9ac70c6b29968f36c93988a1d6fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756531"
---
# <a name="getcallinfo-um-web-service"></a><span data-ttu-id="4d3f1-103">GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d3f1-103">GetCallInfo (UM web service)</span></span>

<span data-ttu-id="4d3f1-104">L’élément **GetCallInfo** définit une demande pour obtenir des informations relatives à un appel.</span><span class="sxs-lookup"><span data-stu-id="4d3f1-104">The **GetCallInfo** element defines a request to get information about a call.</span></span> 
  
[<span data-ttu-id="4d3f1-105">GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d3f1-105">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
```xml
<GetCallInfo>
  <CallId/>
</GetCallInfo>
```

 <span data-ttu-id="4d3f1-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="4d3f1-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d3f1-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d3f1-107">Attributes and elements</span></span>

<span data-ttu-id="4d3f1-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d3f1-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d3f1-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d3f1-109">Attributes</span></span>

<span data-ttu-id="4d3f1-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d3f1-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d3f1-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d3f1-111">Child elements</span></span>

|<span data-ttu-id="4d3f1-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d3f1-112">**Element**</span></span>|<span data-ttu-id="4d3f1-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d3f1-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d3f1-114">ID d’appel (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d3f1-114">CallId (UM web service)</span></span>](callid-um-web-service.md) <br/> |<span data-ttu-id="4d3f1-115">Contient l’identificateur de l’appel sur laquelle obtenir plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="4d3f1-115">Contains the identifier of the call about which to get information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d3f1-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d3f1-116">Parent elements</span></span>

<span data-ttu-id="4d3f1-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d3f1-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4d3f1-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4d3f1-118">Text value</span></span>

<span data-ttu-id="4d3f1-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d3f1-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d3f1-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d3f1-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d3f1-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d3f1-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d3f1-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d3f1-122">Schema Name</span></span>  <br/> |<span data-ttu-id="4d3f1-123">Messages</span><span class="sxs-lookup"><span data-stu-id="4d3f1-123">Messages</span></span>  <br/> |
|<span data-ttu-id="4d3f1-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d3f1-124">Validation File</span></span>  <br/> |<span data-ttu-id="4d3f1-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d3f1-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d3f1-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d3f1-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d3f1-127">False</span><span class="sxs-lookup"><span data-stu-id="4d3f1-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d3f1-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4d3f1-128">See also</span></span>



[<span data-ttu-id="4d3f1-129">Opération GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d3f1-129">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)

