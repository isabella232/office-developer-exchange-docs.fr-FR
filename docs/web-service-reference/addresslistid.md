---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: L’élément AddressListId Spécifie l’identificateur d’une liste d’adresses.
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755185"
---
# <a name="addresslistid"></a><span data-ttu-id="524d5-103">AddressListId</span><span class="sxs-lookup"><span data-stu-id="524d5-103">AddressListId</span></span>

<span data-ttu-id="524d5-104">L’élément **AddressListId** Spécifie l’identificateur d’une liste d’adresses.</span><span class="sxs-lookup"><span data-stu-id="524d5-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="524d5-105">**AddressListIdType**</span><span class="sxs-lookup"><span data-stu-id="524d5-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="524d5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="524d5-106">Attributes and elements</span></span>

<span data-ttu-id="524d5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="524d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="524d5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="524d5-108">Attributes</span></span>

|<span data-ttu-id="524d5-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="524d5-109">**Attribute**</span></span>|<span data-ttu-id="524d5-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="524d5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="524d5-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="524d5-111">**Id**</span></span> <br/> |<span data-ttu-id="524d5-112">Identificateur de liste adresse chaîne.</span><span class="sxs-lookup"><span data-stu-id="524d5-112">A string address list identifier.</span></span> <span data-ttu-id="524d5-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="524d5-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="524d5-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="524d5-114">Child elements</span></span>

<span data-ttu-id="524d5-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="524d5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="524d5-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="524d5-116">Parent elements</span></span>

|<span data-ttu-id="524d5-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="524d5-117">**Element**</span></span>|<span data-ttu-id="524d5-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="524d5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="524d5-119">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="524d5-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="524d5-120">Indique le dossier qui est ciblé pour les actions qui utilisent des dossiers.</span><span class="sxs-lookup"><span data-stu-id="524d5-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="524d5-121">Cet élément doit être présent lors de la copie, suppression, déplacement et en définissant l’état de lecture sur les éléments de conversation dans un dossier cible.</span><span class="sxs-lookup"><span data-stu-id="524d5-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="524d5-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="524d5-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="524d5-123">Spécifie l’identificateur du dossier dans lequel sont copiés les éléments de messagerie électronique.</span><span class="sxs-lookup"><span data-stu-id="524d5-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="524d5-124">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="524d5-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="524d5-125">Indique le dossier de destination de copie et les actions de déplacement.</span><span class="sxs-lookup"><span data-stu-id="524d5-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="524d5-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="524d5-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="524d5-127">Spécifie l’identificateur du dossier vers lequel les éléments de messagerie électronique sont déplacés</span><span class="sxs-lookup"><span data-stu-id="524d5-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="524d5-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="524d5-128">Remarks</span></span>

<span data-ttu-id="524d5-129">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="524d5-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="524d5-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="524d5-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="524d5-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="524d5-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="524d5-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="524d5-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="524d5-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="524d5-133">Schema Name</span></span>  <br/> |<span data-ttu-id="524d5-134">Schéma type</span><span class="sxs-lookup"><span data-stu-id="524d5-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="524d5-135">Validation File</span><span class="sxs-lookup"><span data-stu-id="524d5-135">Validation File</span></span>  <br/> |<span data-ttu-id="524d5-136">types.xsd</span><span class="sxs-lookup"><span data-stu-id="524d5-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="524d5-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="524d5-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="524d5-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="524d5-138">See also</span></span>

- [<span data-ttu-id="524d5-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="524d5-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

