---
title: FindPeopleResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: L’élément FindPeopleResponse spécifie la réponse à une demande de FindPeople.
ms.openlocfilehash: 4f2c2f6069a515d5153ea488b35182d8b35f029f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756417"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="c6039-103">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="c6039-103">FindPeopleResponse</span></span>

<span data-ttu-id="c6039-104">L’élément **FindPeopleResponse** spécifie la réponse à une demande de **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="c6039-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
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

 <span data-ttu-id="c6039-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c6039-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6039-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c6039-106">Attributes and elements</span></span>

<span data-ttu-id="c6039-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c6039-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6039-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c6039-108">Attributes</span></span>

|<span data-ttu-id="c6039-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c6039-109">**Attribute**</span></span>|<span data-ttu-id="c6039-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6039-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c6039-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c6039-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="c6039-112">Spécifie la classe de la réponse.</span><span class="sxs-lookup"><span data-stu-id="c6039-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="c6039-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c6039-113">ResponseClass</span></span>

|<span data-ttu-id="c6039-114">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="c6039-114">**Value**</span></span>|<span data-ttu-id="c6039-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6039-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c6039-116">Opération réussie</span><span class="sxs-lookup"><span data-stu-id="c6039-116">Success</span></span>  <br/> |<span data-ttu-id="c6039-117">Indique la réussite.</span><span class="sxs-lookup"><span data-stu-id="c6039-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="c6039-118">Avertissement</span><span class="sxs-lookup"><span data-stu-id="c6039-118">Warning</span></span>  <br/> |<span data-ttu-id="c6039-119">Indique un avertissement.</span><span class="sxs-lookup"><span data-stu-id="c6039-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="c6039-120">Erreur</span><span class="sxs-lookup"><span data-stu-id="c6039-120">Error</span></span>  <br/> |<span data-ttu-id="c6039-121">Indique une erreur.</span><span class="sxs-lookup"><span data-stu-id="c6039-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c6039-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c6039-122">Child elements</span></span>

|<span data-ttu-id="c6039-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6039-123">**Element**</span></span>|<span data-ttu-id="c6039-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6039-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6039-125">Personnes</span><span class="sxs-lookup"><span data-stu-id="c6039-125">People</span></span>](people.md) <br/> |<span data-ttu-id="c6039-126">Spécifie un tableau de données personnage renvoyées à la suite d’une demande **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="c6039-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="c6039-127">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="c6039-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="c6039-128">Spécifie le nombre total de personnages stockés sur un serveur qui sont renvoyées par une requête **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="c6039-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="c6039-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="c6039-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c6039-130">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="c6039-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c6039-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c6039-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c6039-132">Fournit des informations d’état sur la demande.</span><span class="sxs-lookup"><span data-stu-id="c6039-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="c6039-133">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c6039-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c6039-134">Actuellement inutilisée et réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="c6039-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="c6039-135">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c6039-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c6039-136">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="c6039-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6039-137">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c6039-137">Parent elements</span></span>

|<span data-ttu-id="c6039-138">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6039-138">**Element**</span></span>|<span data-ttu-id="c6039-139">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6039-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6039-140">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c6039-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c6039-141">Spécifie un tableau de messages de réponse.</span><span class="sxs-lookup"><span data-stu-id="c6039-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c6039-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="c6039-142">Remarks</span></span>

<span data-ttu-id="c6039-143">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c6039-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c6039-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c6039-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6039-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c6039-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6039-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c6039-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c6039-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c6039-147">Schema Name</span></span>  <br/> |<span data-ttu-id="c6039-148">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="c6039-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="c6039-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c6039-149">Validation File</span></span>  <br/> |<span data-ttu-id="c6039-150">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c6039-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6039-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c6039-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c6039-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c6039-152">See also</span></span>



- [<span data-ttu-id="c6039-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c6039-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

