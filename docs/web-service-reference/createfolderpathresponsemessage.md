---
title: CreateFolderPathResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: L’élément CreateFolderPathResponseMessage spécifie le message de réponse pour une demande CreateFolderPath.
ms.openlocfilehash: 3c0c4e98b568a6398dcd0e71a6e6931a3f47e3da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458886"
---
# <a name="createfolderpathresponsemessage"></a><span data-ttu-id="e1c03-103">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e1c03-103">CreateFolderPathResponseMessage</span></span>

<span data-ttu-id="e1c03-104">L’élément **CreateFolderPathResponseMessage** spécifie le message de réponse pour une demande **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="e1c03-104">The **CreateFolderPathResponseMessage** element specifies the response message for a **CreateFolderPath** request.</span></span> 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 <span data-ttu-id="e1c03-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e1c03-105">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1c03-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e1c03-106">Attributes and elements</span></span>

<span data-ttu-id="e1c03-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e1c03-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1c03-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e1c03-108">Attributes</span></span>

|<span data-ttu-id="e1c03-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="e1c03-109">**Attribute**</span></span>|<span data-ttu-id="e1c03-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1c03-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1c03-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e1c03-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e1c03-112">Indique la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="e1c03-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e1c03-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e1c03-113">ResponseClass</span></span>

|<span data-ttu-id="e1c03-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e1c03-114">**Value**</span></span>|<span data-ttu-id="e1c03-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1c03-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1c03-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="e1c03-116">Success</span></span>  <br/> |<span data-ttu-id="e1c03-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="e1c03-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e1c03-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="e1c03-118">Warning</span></span>  <br/> |<span data-ttu-id="e1c03-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="e1c03-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e1c03-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="e1c03-120">Error</span></span>  <br/> |<span data-ttu-id="e1c03-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="e1c03-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e1c03-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e1c03-122">Child elements</span></span>

|<span data-ttu-id="e1c03-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1c03-123">**Element**</span></span>|<span data-ttu-id="e1c03-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1c03-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1c03-125">Dossiers</span><span class="sxs-lookup"><span data-stu-id="e1c03-125">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e1c03-126">Contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="e1c03-126">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
|[<span data-ttu-id="e1c03-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e1c03-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e1c03-128">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="e1c03-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e1c03-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="e1c03-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e1c03-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="e1c03-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e1c03-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e1c03-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e1c03-132">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="e1c03-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e1c03-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1c03-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e1c03-134">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="e1c03-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1c03-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e1c03-135">Parent elements</span></span>

|<span data-ttu-id="e1c03-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1c03-136">**Element**</span></span>|<span data-ttu-id="e1c03-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1c03-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1c03-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e1c03-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e1c03-139">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1c03-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1c03-140">Remarques</span><span class="sxs-lookup"><span data-stu-id="e1c03-140">Remarks</span></span>

<span data-ttu-id="e1c03-141">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e1c03-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e1c03-142">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1c03-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1c03-143">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e1c03-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1c03-144">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e1c03-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e1c03-145">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e1c03-145">Schema Name</span></span>  <br/> |<span data-ttu-id="e1c03-146">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="e1c03-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="e1c03-147">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e1c03-147">Validation File</span></span>  <br/> |<span data-ttu-id="e1c03-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e1c03-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1c03-149">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e1c03-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e1c03-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e1c03-150">See also</span></span>

- [<span data-ttu-id="e1c03-151">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e1c03-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

