---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: L’élément SendItem est l’élément racine dans une demande d’envoi d’un élément dans la banque d’informations Exchange.
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829340"
---
# <a name="senditem"></a><span data-ttu-id="22ff8-103">SendItem</span><span class="sxs-lookup"><span data-stu-id="22ff8-103">SendItem</span></span>

<span data-ttu-id="22ff8-104">L’élément **SendItem** est l’élément racine dans une demande d’envoi d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="22ff8-104">The **SendItem** element is the root element in a request to send an item in the Exchange store.</span></span> 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 <span data-ttu-id="22ff8-105">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="22ff8-105">**SendItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22ff8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22ff8-106">Attributes and elements</span></span>

<span data-ttu-id="22ff8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22ff8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22ff8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22ff8-108">Attributes</span></span>

|<span data-ttu-id="22ff8-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="22ff8-109">**Attribute**</span></span>|<span data-ttu-id="22ff8-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="22ff8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22ff8-111">**SaveItemToFolder**</span><span class="sxs-lookup"><span data-stu-id="22ff8-111">**SaveItemToFolder**</span></span> <br/> |<span data-ttu-id="22ff8-112">Indique si une copie de l’élément envoyé est enregistrée.</span><span class="sxs-lookup"><span data-stu-id="22ff8-112">Identifies whether a copy of the sent item is saved.</span></span> <span data-ttu-id="22ff8-113">L’enregistrement action dépend de la valeur de **SaveItemToFolder** et si un élément [SavedItemFolderId](saveditemfolderid.md) est présent dans la demande.</span><span class="sxs-lookup"><span data-stu-id="22ff8-113">The save action depends on the value of **SaveItemToFolder** and whether a [SavedItemFolderId](saveditemfolderid.md) element is present in the request.</span></span> <span data-ttu-id="22ff8-114">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="22ff8-114">This element is required.</span></span>  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a><span data-ttu-id="22ff8-115">Attribut SaveItemToFolder</span><span class="sxs-lookup"><span data-stu-id="22ff8-115">SaveItemToFolder Attribute</span></span>

|<span data-ttu-id="22ff8-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="22ff8-116">**Value**</span></span>|<span data-ttu-id="22ff8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="22ff8-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="22ff8-118">**valeur True**</span><span class="sxs-lookup"><span data-stu-id="22ff8-118">**true**</span></span> <br/> |<span data-ttu-id="22ff8-119">Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément est enregistré dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="22ff8-119">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is saved in the Sent Items folder.</span></span> <span data-ttu-id="22ff8-120">Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, l’élément est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="22ff8-120">If the [SavedItemFolderId](saveditemfolderid.md) element is present, the item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="22ff8-121">**False**</span><span class="sxs-lookup"><span data-stu-id="22ff8-121">**false**</span></span> <br/> |<span data-ttu-id="22ff8-122">Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément n’est pas enregistré.</span><span class="sxs-lookup"><span data-stu-id="22ff8-122">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is not saved.</span></span> <span data-ttu-id="22ff8-123">Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, une réponse d’erreur s’afficheront avec un élément [ResponseCode](responsecode.md) qui contient la valeur **ErrorInvalidSendItemSaveSettings** .</span><span class="sxs-lookup"><span data-stu-id="22ff8-123">If the [SavedItemFolderId](saveditemfolderid.md) element is present, an error response will be returned with a [ResponseCode](responsecode.md) element that contains the **ErrorInvalidSendItemSaveSettings** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="22ff8-124">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22ff8-124">Child elements</span></span>

|<span data-ttu-id="22ff8-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22ff8-125">**Element**</span></span>|<span data-ttu-id="22ff8-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="22ff8-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22ff8-127">ItemId</span><span class="sxs-lookup"><span data-stu-id="22ff8-127">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="22ff8-128">Contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui servent à supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="22ff8-128">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="22ff8-129">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="22ff8-129">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="22ff8-130">Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="22ff8-130">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22ff8-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22ff8-131">Parent elements</span></span>

<span data-ttu-id="22ff8-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="22ff8-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="22ff8-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="22ff8-133">Remarks</span></span>

<span data-ttu-id="22ff8-134">Si un élément dans le dossier éléments envoyés est envoyé, l’élément envoyé est supprimé et une copie de celle-ci est placée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="22ff8-134">If an item in the Sent Items folder is sent, the sent item is deleted and a copy of it is put in the Sent Items folder.</span></span>
  
<span data-ttu-id="22ff8-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="22ff8-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22ff8-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22ff8-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22ff8-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22ff8-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="22ff8-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22ff8-138">Schema Name</span></span>  <br/> |<span data-ttu-id="22ff8-139">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="22ff8-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="22ff8-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22ff8-140">Validation File</span></span>  <br/> |<span data-ttu-id="22ff8-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="22ff8-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22ff8-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22ff8-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="22ff8-143">False</span><span class="sxs-lookup"><span data-stu-id="22ff8-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22ff8-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22ff8-144">See also</span></span>



[<span data-ttu-id="22ff8-145">Opération SendItem</span><span class="sxs-lookup"><span data-stu-id="22ff8-145">SendItem operation</span></span>](senditem-operation.md)

