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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465148"
---
# <a name="syncfolderitems"></a><span data-ttu-id="7a976-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7a976-103">SyncFolderItems</span></span>

<span data-ttu-id="7a976-104">L’élément **SyncFolderItems** définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a976-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="7a976-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="7a976-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a976-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a976-106">Attributes and elements</span></span>

<span data-ttu-id="7a976-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a976-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a976-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a976-108">Attributes</span></span>

<span data-ttu-id="7a976-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7a976-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a976-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a976-110">Child elements</span></span>

|<span data-ttu-id="7a976-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a976-111">**Element**</span></span>|<span data-ttu-id="7a976-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a976-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a976-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="7a976-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="7a976-114">Identifie les propriétés d’élément et le contenu à inclure dans une réponse SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="7a976-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="7a976-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7a976-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="7a976-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="7a976-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="7a976-117">Représente le dossier qui contient les éléments à synchroniser.</span><span class="sxs-lookup"><span data-stu-id="7a976-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="7a976-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7a976-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="7a976-119">SyncState</span><span class="sxs-lookup"><span data-stu-id="7a976-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7a976-120">Contient un formulaire codé en base64 des données de synchronisation qui sont mises à jour après chaque demande réussie.</span><span class="sxs-lookup"><span data-stu-id="7a976-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="7a976-121">Il est utilisé pour identifier l’état de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="7a976-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="7a976-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7a976-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7a976-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="7a976-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="7a976-124">Identifie les éléments à ignorer lors de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="7a976-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="7a976-125">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7a976-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7a976-126">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="7a976-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="7a976-127">Décrit le nombre maximal de modifications pouvant être renvoyées dans une réponse de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="7a976-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="7a976-128">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="7a976-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="7a976-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="7a976-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="7a976-130">Indique si les éléments ou les éléments et les informations associés uniquement sont renvoyés dans une réponse de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="7a976-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="7a976-131">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="7a976-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a976-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a976-132">Parent elements</span></span>

<span data-ttu-id="7a976-133">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a976-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a976-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a976-134">Remarks</span></span>

<span data-ttu-id="7a976-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7a976-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a976-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7a976-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a976-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7a976-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a976-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7a976-138">Schema name</span></span>  <br/> |<span data-ttu-id="7a976-139">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="7a976-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="7a976-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7a976-140">Validation file</span></span>  <br/> |<span data-ttu-id="7a976-141">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7a976-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a976-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7a976-142">Can be empty</span></span>  <br/> |<span data-ttu-id="7a976-143">False</span><span class="sxs-lookup"><span data-stu-id="7a976-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a976-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a976-144">See also</span></span>



[<span data-ttu-id="7a976-145">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7a976-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="7a976-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7a976-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

