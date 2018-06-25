---
title: Salles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rooms
api_type:
- schema
ms.assetid: 57b6079a-3d83-4429-861e-c551e9e1a991
description: L’élément de salles est une liste d’un ou plusieurs éléments qui représentent des salles de réunion.
ms.openlocfilehash: e95112d3d565da29c309e45710ffc0ea9b4d5064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829249"
---
# <a name="rooms"></a><span data-ttu-id="40ba1-103">Salles</span><span class="sxs-lookup"><span data-stu-id="40ba1-103">Rooms</span></span>

<span data-ttu-id="40ba1-104">L’élément de **salles** est une liste d’un ou plusieurs éléments qui représentent des salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="40ba1-104">The **Rooms** element is a list of one or more elements that represent meeting rooms.</span></span> 
  
[<span data-ttu-id="40ba1-105">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="40ba1-105">GetRoomsResponse</span></span>](getroomsresponse.md)
  
[<span data-ttu-id="40ba1-106">Salles</span><span class="sxs-lookup"><span data-stu-id="40ba1-106">Rooms</span></span>](rooms.md)
  
```xml
<Rooms>   <Room/></Rooms>
```

 <span data-ttu-id="40ba1-107">**ArrayOfRoomsType**</span><span class="sxs-lookup"><span data-stu-id="40ba1-107">**ArrayOfRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40ba1-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="40ba1-108">Attributes and elements</span></span>

<span data-ttu-id="40ba1-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="40ba1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40ba1-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="40ba1-110">Attributes</span></span>

<span data-ttu-id="40ba1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="40ba1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40ba1-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="40ba1-112">Child elements</span></span>

|<span data-ttu-id="40ba1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40ba1-113">**Element**</span></span>|<span data-ttu-id="40ba1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="40ba1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40ba1-115">Salle</span><span class="sxs-lookup"><span data-stu-id="40ba1-115">Room</span></span>](room.md) <br/> |<span data-ttu-id="40ba1-116">Définit une adresse de messagerie et le nom complet qui représente une salle de réunion.</span><span class="sxs-lookup"><span data-stu-id="40ba1-116">Defines an e-mail address and display name that represents a meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40ba1-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="40ba1-117">Parent elements</span></span>

|<span data-ttu-id="40ba1-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40ba1-118">**Element**</span></span>|<span data-ttu-id="40ba1-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="40ba1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40ba1-120">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="40ba1-120">GetRoomsResponse</span></span>](getroomsresponse.md) <br/> ||
   
## <a name="remarks"></a><span data-ttu-id="40ba1-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="40ba1-121">Remarks</span></span>

<span data-ttu-id="40ba1-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="40ba1-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40ba1-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="40ba1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40ba1-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="40ba1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="40ba1-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="40ba1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="40ba1-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="40ba1-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="40ba1-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="40ba1-127">Validation File</span></span>  <br/> |<span data-ttu-id="40ba1-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="40ba1-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="40ba1-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="40ba1-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="40ba1-130">False</span><span class="sxs-lookup"><span data-stu-id="40ba1-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40ba1-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40ba1-131">See also</span></span>



[<span data-ttu-id="40ba1-132">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="40ba1-132">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="40ba1-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="40ba1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

