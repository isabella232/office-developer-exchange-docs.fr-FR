---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: L’élément SyncFolderItems définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838662"
---
# <a name="syncfolderitems"></a><span data-ttu-id="ed73f-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ed73f-103">SyncFolderItems</span></span>

<span data-ttu-id="ed73f-104">L’élément **SyncFolderItems** définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed73f-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="ed73f-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="ed73f-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed73f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ed73f-106">Attributes and elements</span></span>

<span data-ttu-id="ed73f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ed73f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed73f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ed73f-108">Attributes</span></span>

<span data-ttu-id="ed73f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ed73f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed73f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ed73f-110">Child elements</span></span>

|<span data-ttu-id="ed73f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ed73f-111">**Element**</span></span>|<span data-ttu-id="ed73f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ed73f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed73f-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="ed73f-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="ed73f-114">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="ed73f-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="ed73f-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="ed73f-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="ed73f-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="ed73f-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="ed73f-117">Représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="ed73f-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="ed73f-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="ed73f-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="ed73f-119">SyncState</span><span class="sxs-lookup"><span data-stu-id="ed73f-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ed73f-120">Contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64.</span><span class="sxs-lookup"><span data-stu-id="ed73f-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="ed73f-121">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="ed73f-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="ed73f-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ed73f-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed73f-123">Ignorer</span><span class="sxs-lookup"><span data-stu-id="ed73f-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="ed73f-124">Identifie les éléments à ignorer lors de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="ed73f-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="ed73f-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ed73f-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ed73f-126">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="ed73f-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="ed73f-127">Indique le nombre maximal de modifications pouvant être renvoyés dans une réponse de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="ed73f-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="ed73f-128">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="ed73f-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="ed73f-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="ed73f-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="ed73f-130">Indique si seulement les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="ed73f-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="ed73f-131">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="ed73f-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed73f-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ed73f-132">Parent elements</span></span>

<span data-ttu-id="ed73f-133">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ed73f-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed73f-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="ed73f-134">Remarks</span></span>

<span data-ttu-id="ed73f-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="ed73f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed73f-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ed73f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed73f-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ed73f-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ed73f-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ed73f-138">Schema name</span></span>  <br/> |<span data-ttu-id="ed73f-139">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="ed73f-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="ed73f-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ed73f-140">Validation file</span></span>  <br/> |<span data-ttu-id="ed73f-141">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ed73f-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ed73f-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ed73f-142">Can be empty</span></span>  <br/> |<span data-ttu-id="ed73f-143">False</span><span class="sxs-lookup"><span data-stu-id="ed73f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed73f-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ed73f-144">See also</span></span>



[<span data-ttu-id="ed73f-145">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="ed73f-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="ed73f-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ed73f-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

