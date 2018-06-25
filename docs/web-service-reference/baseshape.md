---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: L’élément BaseShape identifie le jeu de propriétés à retourner dans une réponse de l’élément ou le dossier.
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755381"
---
# <a name="baseshape"></a><span data-ttu-id="7a98e-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="7a98e-103">BaseShape</span></span>

<span data-ttu-id="7a98e-104">L’élément **BaseShape** identifie le jeu de propriétés à retourner dans une réponse de l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="7a98e-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="7a98e-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="7a98e-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a98e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a98e-106">Attributes and elements</span></span>

<span data-ttu-id="7a98e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a98e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a98e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a98e-108">Attributes</span></span>

<span data-ttu-id="7a98e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a98e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a98e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a98e-110">Child elements</span></span>

<span data-ttu-id="7a98e-111">Aucun</span><span class="sxs-lookup"><span data-stu-id="7a98e-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a98e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a98e-112">Parent elements</span></span>

|<span data-ttu-id="7a98e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a98e-113">**Element**</span></span>|<span data-ttu-id="7a98e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a98e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a98e-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="7a98e-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="7a98e-116">Identifie les propriétés du dossier à inclure dans la réponse GetFolder, FindFolder ou SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="7a98e-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="7a98e-117">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7a98e-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="7a98e-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="7a98e-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="7a98e-119">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="7a98e-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="7a98e-120">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="7a98e-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a98e-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7a98e-121">Text value</span></span>

<span data-ttu-id="7a98e-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="7a98e-122">A text value is required.</span></span> <span data-ttu-id="7a98e-123">Le tableau suivant répertorie les valeurs possibles de texte.</span><span class="sxs-lookup"><span data-stu-id="7a98e-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="7a98e-124">**Valeurs de texte pour l’élément BaseShape**</span><span class="sxs-lookup"><span data-stu-id="7a98e-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="7a98e-125">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7a98e-125">**Value**</span></span>|<span data-ttu-id="7a98e-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a98e-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a98e-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="7a98e-127">IdOnly</span></span>  <br/> |<span data-ttu-id="7a98e-128">Renvoie uniquement l’élément ou le dossier ID de.</span><span class="sxs-lookup"><span data-stu-id="7a98e-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="7a98e-129">Default (Défaut)</span><span class="sxs-lookup"><span data-stu-id="7a98e-129">Default</span></span>  <br/> |<span data-ttu-id="7a98e-130">Renvoie un ensemble de propriétés qui sont définies par défaut pour l’élément ou d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="7a98e-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="7a98e-131">AllProperties</span><span class="sxs-lookup"><span data-stu-id="7a98e-131">AllProperties</span></span>  <br/> |<span data-ttu-id="7a98e-132">Retourne toutes les propriétés utilisées par la couche de la logique du système Exchange pour créer un dossier.</span><span class="sxs-lookup"><span data-stu-id="7a98e-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="7a98e-133">Le tableau suivant répertorie les propriétés par défaut qui sont retournées pour une demande FindFolder.</span><span class="sxs-lookup"><span data-stu-id="7a98e-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="7a98e-134">Tous les sous-dossiers d’un dossier donné sont retournés dans l’ordre par nom.</span><span class="sxs-lookup"><span data-stu-id="7a98e-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="7a98e-135">**Propriétés par défaut**</span><span class="sxs-lookup"><span data-stu-id="7a98e-135">**Default properties**</span></span>

|<span data-ttu-id="7a98e-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="7a98e-136">**Folder**</span></span>|<span data-ttu-id="7a98e-137">**Propriétés par défaut**</span><span class="sxs-lookup"><span data-stu-id="7a98e-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a98e-138">Inbox</span><span class="sxs-lookup"><span data-stu-id="7a98e-138">Inbox</span></span>  <br/> |<span data-ttu-id="7a98e-139">FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-140">Contacts</span><span class="sxs-lookup"><span data-stu-id="7a98e-140">Contacts</span></span>  <br/> |<span data-ttu-id="7a98e-141">FolderId, nom complet, le nombre total, count sous-dossier</span><span class="sxs-lookup"><span data-stu-id="7a98e-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-142">Calendrier</span><span class="sxs-lookup"><span data-stu-id="7a98e-142">Calendar</span></span>  <br/> |<span data-ttu-id="7a98e-143">FolderId, nom d’affichage, le nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-144">Brouillons</span><span class="sxs-lookup"><span data-stu-id="7a98e-144">Drafts</span></span>  <br/> |<span data-ttu-id="7a98e-145">FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-146">Éléments supprimés</span><span class="sxs-lookup"><span data-stu-id="7a98e-146">Deleted items</span></span>  <br/> |<span data-ttu-id="7a98e-147">FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-148">Autres dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-148">Other folders</span></span>  <br/> |<span data-ttu-id="7a98e-149">FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-150">La boîte d’envoi</span><span class="sxs-lookup"><span data-stu-id="7a98e-150">Outbox</span></span>  <br/> |<span data-ttu-id="7a98e-151">FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-152">Tâches</span><span class="sxs-lookup"><span data-stu-id="7a98e-152">Tasks</span></span>  <br/> |<span data-ttu-id="7a98e-153">FolderId, nom d’affichage, en retard count, nombre total, le nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="7a98e-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="7a98e-154">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a98e-154">Notes</span></span>  <br/> |<span data-ttu-id="7a98e-155">FolderId, nom complet, le nombre total, count sous-dossier</span><span class="sxs-lookup"><span data-stu-id="7a98e-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a98e-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a98e-156">Remarks</span></span>

<span data-ttu-id="7a98e-157">Pour renvoyer les propriétés en plus de celles identifié par l’élément [BaseShape](baseshape.md) , utilisez l’élément [AdditionalProperties](additionalproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="7a98e-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="7a98e-158">Exemple</span><span class="sxs-lookup"><span data-stu-id="7a98e-158">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="7a98e-159">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7a98e-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a98e-160">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7a98e-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a98e-161">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7a98e-161">Schema Name</span></span>  <br/> |<span data-ttu-id="7a98e-162">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7a98e-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a98e-163">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7a98e-163">Validation File</span></span>  <br/> |<span data-ttu-id="7a98e-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a98e-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a98e-165">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7a98e-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a98e-166">False</span><span class="sxs-lookup"><span data-stu-id="7a98e-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a98e-167">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a98e-167">See also</span></span>

- [<span data-ttu-id="7a98e-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="7a98e-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="7a98e-169">ItemShape</span><span class="sxs-lookup"><span data-stu-id="7a98e-169">ItemShape</span></span>](itemshape.md)

