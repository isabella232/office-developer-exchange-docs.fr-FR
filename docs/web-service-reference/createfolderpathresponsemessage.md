---
title: CreateFolderPathResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: L’élément CreateFolderPathResponseMessage Spécifie le message de réponse pour une demande CreateFolderPath.
ms.openlocfilehash: f8f85cc246bb5d5ecd5cb745267d9d373286cf7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755704"
---
# <a name="createfolderpathresponsemessage"></a><span data-ttu-id="964ce-103">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="964ce-103">CreateFolderPathResponseMessage</span></span>

<span data-ttu-id="964ce-104">L’élément **CreateFolderPathResponseMessage** Spécifie le message de réponse pour une demande **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="964ce-104">The **CreateFolderPathResponseMessage** element specifies the response message for a **CreateFolderPath** request.</span></span> 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 <span data-ttu-id="964ce-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="964ce-105">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="964ce-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="964ce-106">Attributes and elements</span></span>

<span data-ttu-id="964ce-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="964ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="964ce-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="964ce-108">Attributes</span></span>

|<span data-ttu-id="964ce-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="964ce-109">**Attribute**</span></span>|<span data-ttu-id="964ce-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="964ce-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="964ce-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="964ce-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="964ce-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="964ce-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="964ce-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="964ce-113">ResponseClass</span></span>

|<span data-ttu-id="964ce-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="964ce-114">**Value**</span></span>|<span data-ttu-id="964ce-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="964ce-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="964ce-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="964ce-116">Success</span></span>  <br/> |<span data-ttu-id="964ce-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="964ce-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="964ce-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="964ce-118">Warning</span></span>  <br/> |<span data-ttu-id="964ce-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="964ce-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="964ce-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="964ce-120">Error</span></span>  <br/> |<span data-ttu-id="964ce-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="964ce-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="964ce-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="964ce-122">Child elements</span></span>

|<span data-ttu-id="964ce-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="964ce-123">**Element**</span></span>|<span data-ttu-id="964ce-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="964ce-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="964ce-125">Dossiers</span><span class="sxs-lookup"><span data-stu-id="964ce-125">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="964ce-126">Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="964ce-126">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
|[<span data-ttu-id="964ce-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="964ce-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="964ce-128">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="964ce-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="964ce-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="964ce-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="964ce-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="964ce-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="964ce-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="964ce-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="964ce-132">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="964ce-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="964ce-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="964ce-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="964ce-134">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="964ce-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="964ce-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="964ce-135">Parent elements</span></span>

|<span data-ttu-id="964ce-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="964ce-136">**Element**</span></span>|<span data-ttu-id="964ce-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="964ce-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="964ce-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="964ce-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="964ce-139">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="964ce-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="964ce-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="964ce-140">Remarks</span></span>

<span data-ttu-id="964ce-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="964ce-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="964ce-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="964ce-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="964ce-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="964ce-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="964ce-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="964ce-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="964ce-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="964ce-145">Schema Name</span></span>  <br/> |<span data-ttu-id="964ce-146">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="964ce-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="964ce-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="964ce-147">Validation File</span></span>  <br/> |<span data-ttu-id="964ce-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="964ce-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="964ce-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="964ce-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="964ce-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="964ce-150">See also</span></span>

- [<span data-ttu-id="964ce-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="964ce-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

