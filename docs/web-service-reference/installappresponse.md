---
title: InstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: L’élément InstallAppResponse spécifie la réponse à une demande InstallApp.
ms.openlocfilehash: 0f7690e2df7e71c4e478dec191671af24f96294b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465666"
---
# <a name="installappresponse"></a><span data-ttu-id="f7bfa-103">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="f7bfa-103">InstallAppResponse</span></span>

<span data-ttu-id="f7bfa-104">L’élément **InstallAppResponse** spécifie la réponse à une demande **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="f7bfa-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="f7bfa-105">**InstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7bfa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7bfa-106">Attributes and elements</span></span>

<span data-ttu-id="f7bfa-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7bfa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7bfa-108">Attributes</span></span>

|<span data-ttu-id="f7bfa-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-109">**Attribute**</span></span>|<span data-ttu-id="f7bfa-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f7bfa-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f7bfa-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="f7bfa-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="f7bfa-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f7bfa-113">ResponseClass</span></span>

|<span data-ttu-id="f7bfa-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-114">**Value**</span></span>|<span data-ttu-id="f7bfa-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f7bfa-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="f7bfa-116">Success</span></span>  <br/> |<span data-ttu-id="f7bfa-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="f7bfa-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="f7bfa-118">Warning</span></span>  <br/> |<span data-ttu-id="f7bfa-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="f7bfa-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="f7bfa-120">Error</span></span>  <br/> |<span data-ttu-id="f7bfa-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f7bfa-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7bfa-122">Child elements</span></span>

|<span data-ttu-id="f7bfa-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-123">**Element**</span></span>|<span data-ttu-id="f7bfa-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7bfa-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f7bfa-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f7bfa-126">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="f7bfa-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="f7bfa-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f7bfa-128">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f7bfa-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f7bfa-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f7bfa-130">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f7bfa-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f7bfa-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f7bfa-132">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7bfa-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7bfa-133">Parent elements</span></span>

|<span data-ttu-id="f7bfa-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-134">**Element**</span></span>|<span data-ttu-id="f7bfa-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7bfa-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7bfa-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f7bfa-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f7bfa-137">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7bfa-138">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f7bfa-138">Text value</span></span>

<span data-ttu-id="f7bfa-139">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7bfa-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7bfa-140">Remarks</span></span>

<span data-ttu-id="f7bfa-141">L’élément **GetAppManifestsResponseMessage** est applicable pour les clients qui ciblent Exchange Online et les versions de Microsoft Exchange Server à partir d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="f7bfa-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f7bfa-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7bfa-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7bfa-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7bfa-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f7bfa-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7bfa-144">Schema Name</span></span>  <br/> |<span data-ttu-id="f7bfa-145">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="f7bfa-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="f7bfa-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7bfa-146">Validation File</span></span>  <br/> |<span data-ttu-id="f7bfa-147">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f7bfa-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7bfa-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7bfa-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f7bfa-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7bfa-149">See also</span></span>



- [<span data-ttu-id="f7bfa-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f7bfa-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

