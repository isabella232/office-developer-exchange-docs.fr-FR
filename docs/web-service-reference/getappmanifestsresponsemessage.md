---
title: GetAppManifestsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 815908f1-4223-42d8-92dc-f8bdfc6b5df8
description: L’élément GetAppManifestsResponseMessage spécifie le message de réponse pour une demande GetAppManifests.
ms.openlocfilehash: 26a521d8647a010fe956596eaf63d4df4756edb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459531"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="71df2-103">GetAppManifestsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="71df2-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="71df2-104">L’élément **GetAppManifestsResponseMessage** spécifie le message de réponse pour une demande **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="71df2-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="71df2-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="71df2-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71df2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="71df2-106">Attributes and elements</span></span>

<span data-ttu-id="71df2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="71df2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71df2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="71df2-108">Attributes</span></span>

|<span data-ttu-id="71df2-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="71df2-109">**Attribute**</span></span>|<span data-ttu-id="71df2-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="71df2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71df2-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="71df2-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="71df2-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="71df2-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="71df2-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="71df2-113">ResponseClass</span></span>

|<span data-ttu-id="71df2-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="71df2-114">**Value**</span></span>|<span data-ttu-id="71df2-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="71df2-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71df2-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="71df2-116">Success</span></span>  <br/> |<span data-ttu-id="71df2-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="71df2-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="71df2-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="71df2-118">Warning</span></span>  <br/> |<span data-ttu-id="71df2-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="71df2-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="71df2-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="71df2-120">Error</span></span>  <br/> |<span data-ttu-id="71df2-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="71df2-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71df2-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="71df2-122">Child elements</span></span>

|<span data-ttu-id="71df2-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71df2-123">**Element**</span></span>|<span data-ttu-id="71df2-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="71df2-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71df2-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="71df2-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="71df2-126">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="71df2-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="71df2-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="71df2-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="71df2-128">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="71df2-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="71df2-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="71df2-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="71df2-130">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="71df2-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="71df2-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="71df2-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="71df2-132">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="71df2-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71df2-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="71df2-133">Parent elements</span></span>

|<span data-ttu-id="71df2-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71df2-134">**Element**</span></span>|<span data-ttu-id="71df2-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="71df2-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71df2-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="71df2-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="71df2-137">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="71df2-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71df2-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="71df2-138">Remarks</span></span>

<span data-ttu-id="71df2-139">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="71df2-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="71df2-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="71df2-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71df2-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="71df2-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71df2-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="71df2-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="71df2-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="71df2-143">Schema Name</span></span>  <br/> |<span data-ttu-id="71df2-144">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="71df2-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="71df2-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="71df2-145">Validation File</span></span>  <br/> |<span data-ttu-id="71df2-146">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="71df2-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71df2-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="71df2-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="71df2-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71df2-148">See also</span></span>



- [<span data-ttu-id="71df2-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="71df2-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

