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
description: L’élément SendItem est l’élément racine dans une demande d’envoi d’un élément dans la Banque d’Exchange.
ms.openlocfilehash: 28f0d484dd079146c998cb7317bd2d80c6739e19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530564"
---
# <a name="senditem"></a><span data-ttu-id="bef07-103">SendItem</span><span class="sxs-lookup"><span data-stu-id="bef07-103">SendItem</span></span>

<span data-ttu-id="bef07-104">L’élément **SendItem** est l’élément racine dans une demande d’envoi d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="bef07-104">The **SendItem** element is the root element in a request to send an item in the Exchange store.</span></span> 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 <span data-ttu-id="bef07-105">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="bef07-105">**SendItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bef07-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bef07-106">Attributes and elements</span></span>

<span data-ttu-id="bef07-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bef07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bef07-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bef07-108">Attributes</span></span>

|<span data-ttu-id="bef07-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bef07-109">**Attribute**</span></span>|<span data-ttu-id="bef07-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bef07-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bef07-111">**SaveItemToFolder**</span><span class="sxs-lookup"><span data-stu-id="bef07-111">**SaveItemToFolder**</span></span> <br/> |<span data-ttu-id="bef07-112">Identifie si une copie de l’élément envoyé est enregistrée.</span><span class="sxs-lookup"><span data-stu-id="bef07-112">Identifies whether a copy of the sent item is saved.</span></span> <span data-ttu-id="bef07-113">L’action enregistrer dépend de la valeur de **SaveItemToFolder** et de la présence ou non d’un élément [SavedItemFolderId](saveditemfolderid.md) dans la demande.</span><span class="sxs-lookup"><span data-stu-id="bef07-113">The save action depends on the value of **SaveItemToFolder** and whether a [SavedItemFolderId](saveditemfolderid.md) element is present in the request.</span></span> <span data-ttu-id="bef07-114">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="bef07-114">This element is required.</span></span>  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a><span data-ttu-id="bef07-115">Attribut SaveItemToFolder</span><span class="sxs-lookup"><span data-stu-id="bef07-115">SaveItemToFolder Attribute</span></span>

|<span data-ttu-id="bef07-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="bef07-116">**Value**</span></span>|<span data-ttu-id="bef07-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="bef07-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bef07-118">**a**</span><span class="sxs-lookup"><span data-stu-id="bef07-118">**true**</span></span> <br/> |<span data-ttu-id="bef07-119">Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément est enregistré dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="bef07-119">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is saved in the Sent Items folder.</span></span> <span data-ttu-id="bef07-120">Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, l’élément est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId](saveditemfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="bef07-120">If the [SavedItemFolderId](saveditemfolderid.md) element is present, the item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="bef07-121">**true**</span><span class="sxs-lookup"><span data-stu-id="bef07-121">**false**</span></span> <br/> |<span data-ttu-id="bef07-122">Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément n’est pas enregistré.</span><span class="sxs-lookup"><span data-stu-id="bef07-122">If the [SavedItemFolderId](saveditemfolderid.md) element is not present, the item is not saved.</span></span> <span data-ttu-id="bef07-123">Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, une réponse d’erreur est renvoyée avec un élément [ResponseCode](responsecode.md) qui contient la valeur **ErrorInvalidSendItemSaveSettings** .</span><span class="sxs-lookup"><span data-stu-id="bef07-123">If the [SavedItemFolderId](saveditemfolderid.md) element is present, an error response will be returned with a [ResponseCode](responsecode.md) element that contains the **ErrorInvalidSendItemSaveSettings** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bef07-124">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bef07-124">Child elements</span></span>

|<span data-ttu-id="bef07-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bef07-125">**Element**</span></span>|<span data-ttu-id="bef07-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="bef07-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bef07-127">ItemIds</span><span class="sxs-lookup"><span data-stu-id="bef07-127">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="bef07-128">Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="bef07-128">Contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bef07-129">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="bef07-129">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="bef07-130">Identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="bef07-130">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bef07-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bef07-131">Parent elements</span></span>

<span data-ttu-id="bef07-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bef07-132">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bef07-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="bef07-133">Remarks</span></span>

<span data-ttu-id="bef07-134">Si un élément du dossier éléments envoyés est envoyé, l’élément envoyé est supprimé et une copie est placée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="bef07-134">If an item in the Sent Items folder is sent, the sent item is deleted and a copy of it is put in the Sent Items folder.</span></span>
  
<span data-ttu-id="bef07-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bef07-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bef07-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bef07-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bef07-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bef07-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bef07-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bef07-138">Schema Name</span></span>  <br/> |<span data-ttu-id="bef07-139">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bef07-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bef07-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bef07-140">Validation File</span></span>  <br/> |<span data-ttu-id="bef07-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bef07-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bef07-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bef07-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="bef07-143">False</span><span class="sxs-lookup"><span data-stu-id="bef07-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bef07-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bef07-144">See also</span></span>



[<span data-ttu-id="bef07-145">Opération SendItem</span><span class="sxs-lookup"><span data-stu-id="bef07-145">SendItem operation</span></span>](senditem-operation.md)

