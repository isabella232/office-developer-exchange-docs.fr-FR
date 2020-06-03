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
description: L’élément SyncFolderItems définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465148"
---
# <a name="syncfolderitems"></a><span data-ttu-id="de3c1-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="de3c1-103">SyncFolderItems</span></span>

<span data-ttu-id="de3c1-104">L’élément **SyncFolderItems** définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="de3c1-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="de3c1-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="de3c1-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de3c1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de3c1-106">Attributes and elements</span></span>

<span data-ttu-id="de3c1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de3c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de3c1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="de3c1-108">Attributes</span></span>

<span data-ttu-id="de3c1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="de3c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de3c1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de3c1-110">Child elements</span></span>

|<span data-ttu-id="de3c1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de3c1-111">**Element**</span></span>|<span data-ttu-id="de3c1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="de3c1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de3c1-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="de3c1-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="de3c1-114">Identifie les propriétés d’élément et le contenu à inclure dans une réponse SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="de3c1-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="de3c1-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="de3c1-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="de3c1-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="de3c1-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="de3c1-117">Représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="de3c1-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="de3c1-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="de3c1-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="de3c1-119">SyncState</span><span class="sxs-lookup"><span data-stu-id="de3c1-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="de3c1-120">Contient un formulaire codé en base64 des données de synchronisation qui sont mises à jour après chaque demande réussie.</span><span class="sxs-lookup"><span data-stu-id="de3c1-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="de3c1-121">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="de3c1-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="de3c1-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="de3c1-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="de3c1-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="de3c1-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="de3c1-124">Identifie les éléments à ignorer lors de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="de3c1-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="de3c1-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="de3c1-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="de3c1-126">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="de3c1-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="de3c1-127">Décrit le nombre maximal de modifications pouvant être renvoyées dans une réponse de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="de3c1-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="de3c1-128">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="de3c1-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="de3c1-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="de3c1-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="de3c1-130">Indique si les éléments ou les éléments et les informations associés uniquement sont renvoyés dans une réponse de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="de3c1-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="de3c1-131">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="de3c1-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de3c1-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de3c1-132">Parent elements</span></span>

<span data-ttu-id="de3c1-133">Aucun.</span><span class="sxs-lookup"><span data-stu-id="de3c1-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de3c1-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="de3c1-134">Remarks</span></span>

<span data-ttu-id="de3c1-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="de3c1-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de3c1-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de3c1-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de3c1-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de3c1-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de3c1-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de3c1-138">Schema name</span></span>  <br/> |<span data-ttu-id="de3c1-139">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="de3c1-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="de3c1-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de3c1-140">Validation file</span></span>  <br/> |<span data-ttu-id="de3c1-141">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="de3c1-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de3c1-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de3c1-142">Can be empty</span></span>  <br/> |<span data-ttu-id="de3c1-143">False</span><span class="sxs-lookup"><span data-stu-id="de3c1-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de3c1-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="de3c1-144">See also</span></span>



[<span data-ttu-id="de3c1-145">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="de3c1-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="de3c1-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="de3c1-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

