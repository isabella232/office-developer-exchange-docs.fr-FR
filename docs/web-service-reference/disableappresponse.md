---
title: DisableAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: L’élément DisableAppResponse spécifie la réponse à une demande DisableApp.
ms.openlocfilehash: cc28abf644247339e1226cd0e13824cc5f5669be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455645"
---
# <a name="disableappresponse"></a><span data-ttu-id="c342d-103">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="c342d-103">DisableAppResponse</span></span>

<span data-ttu-id="c342d-104">L’élément **DisableAppResponse** spécifie la réponse à une demande **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="c342d-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="c342d-105">**DisableAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="c342d-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c342d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c342d-106">Attributes and elements</span></span>

<span data-ttu-id="c342d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c342d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c342d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c342d-108">Attributes</span></span>

<span data-ttu-id="c342d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c342d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c342d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c342d-110">Child elements</span></span>

|<span data-ttu-id="c342d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c342d-111">**Element**</span></span>|<span data-ttu-id="c342d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c342d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c342d-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="c342d-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c342d-114">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="c342d-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c342d-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c342d-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c342d-116">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="c342d-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="c342d-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c342d-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c342d-118">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="c342d-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="c342d-119">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c342d-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c342d-120">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="c342d-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c342d-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c342d-121">Parent elements</span></span>

<span data-ttu-id="c342d-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c342d-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c342d-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="c342d-123">Remarks</span></span>

<span data-ttu-id="c342d-124">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c342d-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c342d-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c342d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c342d-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c342d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c342d-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c342d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c342d-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c342d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c342d-129">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="c342d-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="c342d-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c342d-130">Validation File</span></span>  <br/> |<span data-ttu-id="c342d-131">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c342d-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c342d-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c342d-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c342d-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c342d-133">See also</span></span>

- [<span data-ttu-id="c342d-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c342d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

