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
ms.openlocfilehash: 8f6393b617331e5878e48113c94ca3546cba095e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459047"
---
# <a name="roomlists"></a><span data-ttu-id="48493-103">RoomLists</span><span class="sxs-lookup"><span data-stu-id="48493-103">RoomLists</span></span>

<span data-ttu-id="48493-104">L’élément **RoomLists** est une liste d’une ou plusieurs adresses qui représentent une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="48493-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="48493-105">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="48493-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="48493-106">RoomLists</span><span class="sxs-lookup"><span data-stu-id="48493-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="48493-107">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="48493-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48493-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="48493-108">Attributes and elements</span></span>

<span data-ttu-id="48493-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="48493-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48493-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="48493-110">Attributes</span></span>

<span data-ttu-id="48493-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="48493-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48493-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="48493-112">Child elements</span></span>

|<span data-ttu-id="48493-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="48493-113">**Element**</span></span>|<span data-ttu-id="48493-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="48493-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48493-115">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="48493-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="48493-116">Définit l’adresse de messagerie et le nom d’affichage qui représente la liste de salles.</span><span class="sxs-lookup"><span data-stu-id="48493-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="48493-117">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="48493-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="48493-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="48493-118">Parent elements</span></span>

|<span data-ttu-id="48493-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="48493-119">**Element**</span></span>|<span data-ttu-id="48493-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="48493-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48493-121">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="48493-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="48493-122">Contient l’État et le résultat d’une demande d' [opération GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="48493-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="48493-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="48493-123">Remarks</span></span>

<span data-ttu-id="48493-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="48493-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48493-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="48493-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48493-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="48493-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="48493-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="48493-127">Schema Name</span></span>  <br/> |<span data-ttu-id="48493-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="48493-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="48493-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="48493-129">Validation File</span></span>  <br/> |<span data-ttu-id="48493-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="48493-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48493-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="48493-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="48493-132">False</span><span class="sxs-lookup"><span data-stu-id="48493-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48493-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="48493-133">See also</span></span>



[<span data-ttu-id="48493-134">Opération GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="48493-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="48493-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="48493-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

