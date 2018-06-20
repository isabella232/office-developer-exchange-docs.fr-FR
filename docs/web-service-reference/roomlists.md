---
title: RoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomLists
api_type:
- schema
ms.assetid: 2b190823-b11e-4635-97e4-3aba5865fd05
description: L’élément RoomLists est une liste d’une ou plusieurs adresses qui représentent une liste de salles de réunion.
ms.openlocfilehash: eb03c34aeb5d80c4a9c6c92471e4094c63f04c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829252"
---
# <a name="roomlists"></a><span data-ttu-id="86447-103">RoomLists</span><span class="sxs-lookup"><span data-stu-id="86447-103">RoomLists</span></span>

<span data-ttu-id="86447-104">L’élément **RoomLists** est une liste d’une ou plusieurs adresses qui représentent une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="86447-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="86447-105">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="86447-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="86447-106">RoomLists</span><span class="sxs-lookup"><span data-stu-id="86447-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="86447-107">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="86447-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86447-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="86447-108">Attributes and elements</span></span>

<span data-ttu-id="86447-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="86447-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86447-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="86447-110">Attributes</span></span>

<span data-ttu-id="86447-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86447-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86447-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="86447-112">Child elements</span></span>

|<span data-ttu-id="86447-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="86447-113">**Element**</span></span>|<span data-ttu-id="86447-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="86447-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86447-115">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="86447-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="86447-116">Définit l’adresse de messagerie et le nom complet qui représente la liste de salles.</span><span class="sxs-lookup"><span data-stu-id="86447-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="86447-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="86447-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86447-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="86447-118">Parent elements</span></span>

|<span data-ttu-id="86447-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="86447-119">**Element**</span></span>|<span data-ttu-id="86447-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="86447-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86447-121">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="86447-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="86447-122">Contient l’état et les résultats d’une demande [d’opération GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="86447-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="86447-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="86447-123">Remarks</span></span>

<span data-ttu-id="86447-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="86447-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86447-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="86447-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86447-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="86447-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="86447-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="86447-127">Schema Name</span></span>  <br/> |<span data-ttu-id="86447-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="86447-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="86447-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="86447-129">Validation File</span></span>  <br/> |<span data-ttu-id="86447-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="86447-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86447-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="86447-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="86447-132">False</span><span class="sxs-lookup"><span data-stu-id="86447-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86447-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="86447-133">See also</span></span>



[<span data-ttu-id="86447-134">Opération GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="86447-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="86447-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86447-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

