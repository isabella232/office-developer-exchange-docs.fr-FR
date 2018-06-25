---
title: GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 82a737c7-da41-4777-8ad8-89851a0b602b
description: L’élément GetRooms est l’élément racine dans une requête pour obtenir une liste de salles au sein d’une liste de salles particulier.
ms.openlocfilehash: a787097752cfeee9489e5f118549c2d939ba4c9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756735"
---
# <a name="getrooms"></a><span data-ttu-id="aadbe-103">GetRooms</span><span class="sxs-lookup"><span data-stu-id="aadbe-103">GetRooms</span></span>

<span data-ttu-id="aadbe-104">L’élément **GetRooms** est l’élément racine dans une requête pour obtenir une liste de salles au sein d’une liste de salles particulier.</span><span class="sxs-lookup"><span data-stu-id="aadbe-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="aadbe-105">**GetRoomsType**</span><span class="sxs-lookup"><span data-stu-id="aadbe-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aadbe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aadbe-106">Attributes and elements</span></span>

<span data-ttu-id="aadbe-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aadbe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aadbe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aadbe-108">Attributes</span></span>

<span data-ttu-id="aadbe-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aadbe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aadbe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aadbe-110">Child elements</span></span>

|<span data-ttu-id="aadbe-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aadbe-111">**Element**</span></span>|<span data-ttu-id="aadbe-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="aadbe-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aadbe-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="aadbe-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="aadbe-114">Représente une adresse de messagerie qui identifie une liste de salles de réunion</span><span class="sxs-lookup"><span data-stu-id="aadbe-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aadbe-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aadbe-115">Parent elements</span></span>

<span data-ttu-id="aadbe-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aadbe-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="aadbe-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="aadbe-117">Text value</span></span>

<span data-ttu-id="aadbe-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aadbe-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aadbe-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="aadbe-119">Remarks</span></span>

<span data-ttu-id="aadbe-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aadbe-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aadbe-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aadbe-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aadbe-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aadbe-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aadbe-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aadbe-123">Schema Name</span></span>  <br/> |<span data-ttu-id="aadbe-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="aadbe-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aadbe-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aadbe-125">Validation File</span></span>  <br/> |<span data-ttu-id="aadbe-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aadbe-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aadbe-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aadbe-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="aadbe-128">False</span><span class="sxs-lookup"><span data-stu-id="aadbe-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aadbe-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aadbe-129">See also</span></span>



- [<span data-ttu-id="aadbe-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aadbe-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

