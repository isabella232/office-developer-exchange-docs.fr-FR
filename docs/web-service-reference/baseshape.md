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
description: L’élément BaseShape identifie le jeu de propriétés à renvoyer dans une réponse d’élément ou de dossier.
ms.openlocfilehash: 9b3f00ff94fbfe6ad6373b16ad95eb9136f81c64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464489"
---
# <a name="baseshape"></a><span data-ttu-id="55b30-103">BaseShape</span><span class="sxs-lookup"><span data-stu-id="55b30-103">BaseShape</span></span>

<span data-ttu-id="55b30-104">L’élément **BaseShape** identifie le jeu de propriétés à renvoyer dans une réponse d’élément ou de dossier.</span><span class="sxs-lookup"><span data-stu-id="55b30-104">The **BaseShape** element identifies the set of properties to return in an item or folder response.</span></span> 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 <span data-ttu-id="55b30-105">**DefaultShapeNamesType**</span><span class="sxs-lookup"><span data-stu-id="55b30-105">**DefaultShapeNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55b30-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55b30-106">Attributes and elements</span></span>

<span data-ttu-id="55b30-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55b30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55b30-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="55b30-108">Attributes</span></span>

<span data-ttu-id="55b30-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="55b30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55b30-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55b30-110">Child elements</span></span>

<span data-ttu-id="55b30-111">Aucun</span><span class="sxs-lookup"><span data-stu-id="55b30-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55b30-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55b30-112">Parent elements</span></span>

|<span data-ttu-id="55b30-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55b30-113">**Element**</span></span>|<span data-ttu-id="55b30-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="55b30-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55b30-115">FolderShape</span><span class="sxs-lookup"><span data-stu-id="55b30-115">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="55b30-116">Identifie les propriétés de dossier à inclure dans la réponse GetFolder, FindFolder ou Opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="55b30-116">Identifies the folder properties to include in the GetFolder, FindFolder, or SyncFolderHierarchy response.</span></span><br/><br/><span data-ttu-id="55b30-117">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="55b30-117">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="55b30-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="55b30-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="55b30-119">Identifie les propriétés d’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="55b30-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span><br/><br/><span data-ttu-id="55b30-120">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="55b30-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55b30-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="55b30-121">Text value</span></span>

<span data-ttu-id="55b30-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="55b30-122">A text value is required.</span></span> <span data-ttu-id="55b30-123">Le tableau suivant répertorie les valeurs de texte possibles.</span><span class="sxs-lookup"><span data-stu-id="55b30-123">The following table lists the possible text values.</span></span>
  
<span data-ttu-id="55b30-124">**Valeurs de texte pour l’élément BaseShape**</span><span class="sxs-lookup"><span data-stu-id="55b30-124">**Text values for the BaseShape element**</span></span>

|<span data-ttu-id="55b30-125">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="55b30-125">**Value**</span></span>|<span data-ttu-id="55b30-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="55b30-126">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55b30-127">IdOnly</span><span class="sxs-lookup"><span data-stu-id="55b30-127">IdOnly</span></span>  <br/> |<span data-ttu-id="55b30-128">Renvoie uniquement l’ID d’élément ou de dossier.</span><span class="sxs-lookup"><span data-stu-id="55b30-128">Returns only the item or folder ID.</span></span>  <br/> |
|<span data-ttu-id="55b30-129">Par défaut</span><span class="sxs-lookup"><span data-stu-id="55b30-129">Default</span></span>  <br/> |<span data-ttu-id="55b30-130">Renvoie un ensemble de propriétés qui sont définies comme valeur par défaut pour l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="55b30-130">Returns a set of properties that are defined as the default for the item or folder.</span></span>  <br/> |
|<span data-ttu-id="55b30-131">AllProperties</span><span class="sxs-lookup"><span data-stu-id="55b30-131">AllProperties</span></span>  <br/> |<span data-ttu-id="55b30-132">Renvoie toutes les propriétés utilisées par la couche de logique métier Exchange pour créer un dossier.</span><span class="sxs-lookup"><span data-stu-id="55b30-132">Returns all the properties used by the Exchange Business Logic layer to construct a folder.</span></span>  <br/> |
   
<span data-ttu-id="55b30-133">Le tableau suivant répertorie les propriétés par défaut qui sont renvoyées pour une demande FindFolder.</span><span class="sxs-lookup"><span data-stu-id="55b30-133">The following table lists the default properties that are returned for a FindFolder request.</span></span> <span data-ttu-id="55b30-134">Tous les sous-dossiers d’un dossier donné sont renvoyés par nom.</span><span class="sxs-lookup"><span data-stu-id="55b30-134">All subfolders of a given folder are returned in order by name.</span></span>
  
<span data-ttu-id="55b30-135">**Propriétés par défaut**</span><span class="sxs-lookup"><span data-stu-id="55b30-135">**Default properties**</span></span>

|<span data-ttu-id="55b30-136">**Folder**</span><span class="sxs-lookup"><span data-stu-id="55b30-136">**Folder**</span></span>|<span data-ttu-id="55b30-137">**Propriétés par défaut**</span><span class="sxs-lookup"><span data-stu-id="55b30-137">**Default Properties**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55b30-138">Boîte de réception</span><span class="sxs-lookup"><span data-stu-id="55b30-138">Inbox</span></span>  <br/> |<span data-ttu-id="55b30-139">FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-139">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-140">Contacts</span><span class="sxs-lookup"><span data-stu-id="55b30-140">Contacts</span></span>  <br/> |<span data-ttu-id="55b30-141">FolderId, nom complet, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-141">FolderId, display name, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-142">Calendrier</span><span class="sxs-lookup"><span data-stu-id="55b30-142">Calendar</span></span>  <br/> |<span data-ttu-id="55b30-143">FolderId, nom d’affichage, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-143">FolderId, display name, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-144">Brouillons</span><span class="sxs-lookup"><span data-stu-id="55b30-144">Drafts</span></span>  <br/> |<span data-ttu-id="55b30-145">FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-145">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-146">Éléments supprimés</span><span class="sxs-lookup"><span data-stu-id="55b30-146">Deleted items</span></span>  <br/> |<span data-ttu-id="55b30-147">FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-147">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-148">Autres dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-148">Other folders</span></span>  <br/> |<span data-ttu-id="55b30-149">FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-149">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-150">Boîte d'envoi</span><span class="sxs-lookup"><span data-stu-id="55b30-150">Outbox</span></span>  <br/> |<span data-ttu-id="55b30-151">FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-151">FolderId, display name, unread count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-152">Tâches</span><span class="sxs-lookup"><span data-stu-id="55b30-152">Tasks</span></span>  <br/> |<span data-ttu-id="55b30-153">FolderId, nom complet, nombre de retard, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-153">FolderId, display name, past due count, total count, subfolder count</span></span>  <br/> |
|<span data-ttu-id="55b30-154">Notes</span><span class="sxs-lookup"><span data-stu-id="55b30-154">Notes</span></span>  <br/> |<span data-ttu-id="55b30-155">FolderId, nom complet, nombre total, nombre de sous-dossiers</span><span class="sxs-lookup"><span data-stu-id="55b30-155">FolderId, display name, total count, subfolder count</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55b30-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="55b30-156">Remarks</span></span>

<span data-ttu-id="55b30-157">Pour renvoyer des propriétés en plus de celles identifiées par l’élément [BaseShape](baseshape.md) , utilisez l’élément [AdditionalProperties](additionalproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="55b30-157">To return properties in addition to those identified by the [BaseShape](baseshape.md) element, use the [AdditionalProperties](additionalproperties.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="55b30-158">Exemple</span><span class="sxs-lookup"><span data-stu-id="55b30-158">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="55b30-159">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55b30-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55b30-160">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55b30-160">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55b30-161">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55b30-161">Schema Name</span></span>  <br/> |<span data-ttu-id="55b30-162">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="55b30-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="55b30-163">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55b30-163">Validation File</span></span>  <br/> |<span data-ttu-id="55b30-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55b30-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55b30-165">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55b30-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="55b30-166">False</span><span class="sxs-lookup"><span data-stu-id="55b30-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55b30-167">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55b30-167">See also</span></span>

- [<span data-ttu-id="55b30-168">FolderShape</span><span class="sxs-lookup"><span data-stu-id="55b30-168">FolderShape</span></span>](foldershape.md)
- [<span data-ttu-id="55b30-169">ItemShape</span><span class="sxs-lookup"><span data-stu-id="55b30-169">ItemShape</span></span>](itemshape.md)

