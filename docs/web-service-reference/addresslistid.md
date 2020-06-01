---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: L’élément AddressListId spécifie l’identificateur d’une liste d’adresses.
ms.openlocfilehash: c33944bf6e41903a5de596628e1ce7ba9f7421e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463607"
---
# <a name="addresslistid"></a><span data-ttu-id="11e44-103">AddressListId</span><span class="sxs-lookup"><span data-stu-id="11e44-103">AddressListId</span></span>

<span data-ttu-id="11e44-104">L’élément **AddressListId** spécifie l’identificateur d’une liste d’adresses.</span><span class="sxs-lookup"><span data-stu-id="11e44-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="11e44-105">**AddressListIdType**</span><span class="sxs-lookup"><span data-stu-id="11e44-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11e44-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="11e44-106">Attributes and elements</span></span>

<span data-ttu-id="11e44-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="11e44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11e44-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="11e44-108">Attributes</span></span>

|<span data-ttu-id="11e44-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="11e44-109">**Attribute**</span></span>|<span data-ttu-id="11e44-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="11e44-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="11e44-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="11e44-111">**Id**</span></span> <br/> |<span data-ttu-id="11e44-112">Identificateur de la liste d’adresses de chaînes.</span><span class="sxs-lookup"><span data-stu-id="11e44-112">A string address list identifier.</span></span> <span data-ttu-id="11e44-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="11e44-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="11e44-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="11e44-114">Child elements</span></span>

<span data-ttu-id="11e44-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="11e44-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="11e44-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="11e44-116">Parent elements</span></span>

|<span data-ttu-id="11e44-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="11e44-117">**Element**</span></span>|<span data-ttu-id="11e44-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="11e44-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11e44-119">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="11e44-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="11e44-120">Indique le dossier ciblé pour les actions qui utilisent des dossiers.</span><span class="sxs-lookup"><span data-stu-id="11e44-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="11e44-121">Cet élément doit être présent lors de la copie, la suppression, le mouvement et la définition de l’état de lecture des éléments de conversation dans un dossier cible.</span><span class="sxs-lookup"><span data-stu-id="11e44-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="11e44-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="11e44-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="11e44-123">Spécifie l’identificateur du dossier dans lequel les éléments de courrier sont copiés.</span><span class="sxs-lookup"><span data-stu-id="11e44-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="11e44-124">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="11e44-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="11e44-125">Indique le dossier de destination pour les actions de copie et de déplacement.</span><span class="sxs-lookup"><span data-stu-id="11e44-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="11e44-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="11e44-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="11e44-127">Spécifie l’identificateur du dossier vers lequel les éléments de courrier sont déplacés.</span><span class="sxs-lookup"><span data-stu-id="11e44-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="11e44-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="11e44-128">Remarks</span></span>

<span data-ttu-id="11e44-129">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="11e44-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="11e44-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="11e44-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11e44-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="11e44-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11e44-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="11e44-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11e44-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="11e44-133">Schema Name</span></span>  <br/> |<span data-ttu-id="11e44-134">Schéma type</span><span class="sxs-lookup"><span data-stu-id="11e44-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="11e44-135">Validation File</span><span class="sxs-lookup"><span data-stu-id="11e44-135">Validation File</span></span>  <br/> |<span data-ttu-id="11e44-136">types. xsd</span><span class="sxs-lookup"><span data-stu-id="11e44-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="11e44-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="11e44-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="11e44-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="11e44-138">See also</span></span>

- [<span data-ttu-id="11e44-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="11e44-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

