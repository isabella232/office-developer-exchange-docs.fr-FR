---
title: InstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: L’élément InstallAppResponse spécifie la réponse à une demande de InstallApp.
ms.openlocfilehash: 8e8da720b3a38e979b3d83810bb798350822146c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827942"
---
# <a name="installappresponse"></a><span data-ttu-id="91199-103">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="91199-103">InstallAppResponse</span></span>

<span data-ttu-id="91199-104">L’élément **InstallAppResponse** spécifie la réponse à une demande de **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="91199-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="91199-105">**InstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="91199-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91199-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="91199-106">Attributes and elements</span></span>

<span data-ttu-id="91199-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="91199-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91199-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="91199-108">Attributes</span></span>

|<span data-ttu-id="91199-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="91199-109">**Attribute**</span></span>|<span data-ttu-id="91199-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="91199-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91199-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="91199-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="91199-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="91199-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="91199-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="91199-113">ResponseClass</span></span>

|<span data-ttu-id="91199-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="91199-114">**Value**</span></span>|<span data-ttu-id="91199-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="91199-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91199-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="91199-116">Success</span></span>  <br/> |<span data-ttu-id="91199-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="91199-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="91199-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="91199-118">Warning</span></span>  <br/> |<span data-ttu-id="91199-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="91199-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="91199-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="91199-120">Error</span></span>  <br/> |<span data-ttu-id="91199-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="91199-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="91199-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="91199-122">Child elements</span></span>

|<span data-ttu-id="91199-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91199-123">**Element**</span></span>|<span data-ttu-id="91199-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="91199-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91199-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="91199-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="91199-126">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="91199-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="91199-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="91199-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="91199-128">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="91199-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="91199-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="91199-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="91199-130">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="91199-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="91199-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="91199-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="91199-132">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="91199-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="91199-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="91199-133">Parent elements</span></span>

|<span data-ttu-id="91199-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91199-134">**Element**</span></span>|<span data-ttu-id="91199-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="91199-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91199-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="91199-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="91199-137">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="91199-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91199-138">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="91199-138">Text value</span></span>

<span data-ttu-id="91199-139">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91199-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91199-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="91199-140">Remarks</span></span>

<span data-ttu-id="91199-141">L’élément **GetAppManifestsResponseMessage** n’est applicable pour les clients qui ciblent Exchange Online et les versions de Microsoft Exchange Server commençant par Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="91199-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="91199-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="91199-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91199-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="91199-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="91199-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="91199-144">Schema Name</span></span>  <br/> |<span data-ttu-id="91199-145">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="91199-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="91199-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="91199-146">Validation File</span></span>  <br/> |<span data-ttu-id="91199-147">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="91199-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="91199-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="91199-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="91199-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="91199-149">See also</span></span>



- [<span data-ttu-id="91199-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="91199-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

