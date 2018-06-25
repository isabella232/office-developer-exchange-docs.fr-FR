---
title: DisableAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: L’élément DisableAppResponse spécifie la réponse à une demande de DisableApp.
ms.openlocfilehash: 740801fa4b60e217f0b9148bcfcc5b206e96bf31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755949"
---
# <a name="disableappresponse"></a><span data-ttu-id="1d362-103">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="1d362-103">DisableAppResponse</span></span>

<span data-ttu-id="1d362-104">L’élément **DisableAppResponse** spécifie la réponse à une demande de **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="1d362-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="1d362-105">**DisableAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="1d362-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d362-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1d362-106">Attributes and elements</span></span>

<span data-ttu-id="1d362-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1d362-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d362-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1d362-108">Attributes</span></span>

<span data-ttu-id="1d362-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d362-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d362-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1d362-110">Child elements</span></span>

|<span data-ttu-id="1d362-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d362-111">**Element**</span></span>|<span data-ttu-id="1d362-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d362-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d362-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="1d362-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1d362-114">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="1d362-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1d362-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1d362-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1d362-116">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="1d362-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="1d362-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1d362-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1d362-118">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="1d362-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="1d362-119">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1d362-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1d362-120">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="1d362-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d362-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1d362-121">Parent elements</span></span>

<span data-ttu-id="1d362-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d362-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1d362-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="1d362-123">Remarks</span></span>

<span data-ttu-id="1d362-124">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1d362-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1d362-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d362-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d362-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1d362-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d362-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1d362-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1d362-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1d362-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1d362-129">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="1d362-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="1d362-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1d362-130">Validation File</span></span>  <br/> |<span data-ttu-id="1d362-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1d362-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d362-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1d362-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1d362-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d362-133">See also</span></span>

- [<span data-ttu-id="1d362-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1d362-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

