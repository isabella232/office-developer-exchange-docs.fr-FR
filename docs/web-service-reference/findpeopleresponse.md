---
title: FindPeopleResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: L’élément FindPeopleResponse spécifie la réponse à une demande FindPeople.
ms.openlocfilehash: b969ac3f7bc2bbd3fc77bf753a15696c3b6d8216
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466401"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="90e0a-103">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="90e0a-103">FindPeopleResponse</span></span>

<span data-ttu-id="90e0a-104">L’élément **FindPeopleResponse** spécifie la réponse à une demande **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="90e0a-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponse ResponseClass=" Success | Warning | Error ">
    <People/>
    <TotalNumberOfPeopleInView/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindPeopleResponse>
```

 <span data-ttu-id="90e0a-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="90e0a-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90e0a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="90e0a-106">Attributes and elements</span></span>

<span data-ttu-id="90e0a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="90e0a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90e0a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="90e0a-108">Attributes</span></span>

|<span data-ttu-id="90e0a-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="90e0a-109">**Attribute**</span></span>|<span data-ttu-id="90e0a-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="90e0a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90e0a-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="90e0a-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="90e0a-112">Spécifie la classe Response.</span><span class="sxs-lookup"><span data-stu-id="90e0a-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="90e0a-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="90e0a-113">ResponseClass</span></span>

|<span data-ttu-id="90e0a-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="90e0a-114">**Value**</span></span>|<span data-ttu-id="90e0a-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="90e0a-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90e0a-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="90e0a-116">Success</span></span>  <br/> |<span data-ttu-id="90e0a-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="90e0a-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="90e0a-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="90e0a-118">Warning</span></span>  <br/> |<span data-ttu-id="90e0a-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="90e0a-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="90e0a-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="90e0a-120">Error</span></span>  <br/> |<span data-ttu-id="90e0a-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="90e0a-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="90e0a-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="90e0a-122">Child elements</span></span>

|<span data-ttu-id="90e0a-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="90e0a-123">**Element**</span></span>|<span data-ttu-id="90e0a-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="90e0a-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90e0a-125">Contacts</span><span class="sxs-lookup"><span data-stu-id="90e0a-125">People</span></span>](people.md) <br/> |<span data-ttu-id="90e0a-126">Spécifie un tableau de données Persona renvoyées comme résultat d’une demande **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="90e0a-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="90e0a-127">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="90e0a-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="90e0a-128">Indique le nombre total de personnes qui sont stockées sur un serveur et qui sont renvoyées par une demande **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="90e0a-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="90e0a-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="90e0a-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="90e0a-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="90e0a-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="90e0a-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="90e0a-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="90e0a-132">Fournit des informations sur l’état de la demande.</span><span class="sxs-lookup"><span data-stu-id="90e0a-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="90e0a-133">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="90e0a-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="90e0a-134">Actuellement inutilisé et réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="90e0a-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="90e0a-135">MessageXml</span><span class="sxs-lookup"><span data-stu-id="90e0a-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="90e0a-136">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="90e0a-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90e0a-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="90e0a-137">Parent elements</span></span>

|<span data-ttu-id="90e0a-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="90e0a-138">**Element**</span></span>|<span data-ttu-id="90e0a-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="90e0a-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90e0a-140">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="90e0a-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="90e0a-141">Spécifie un tableau de messages de réponse.</span><span class="sxs-lookup"><span data-stu-id="90e0a-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90e0a-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="90e0a-142">Remarks</span></span>

<span data-ttu-id="90e0a-143">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="90e0a-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="90e0a-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="90e0a-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90e0a-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="90e0a-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90e0a-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="90e0a-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90e0a-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="90e0a-147">Schema Name</span></span>  <br/> |<span data-ttu-id="90e0a-148">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="90e0a-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="90e0a-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="90e0a-149">Validation File</span></span>  <br/> |<span data-ttu-id="90e0a-150">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="90e0a-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90e0a-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="90e0a-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="90e0a-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="90e0a-152">See also</span></span>



- [<span data-ttu-id="90e0a-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="90e0a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

