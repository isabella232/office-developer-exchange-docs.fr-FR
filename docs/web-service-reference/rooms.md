---
title: Salons
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
description: L’élément Rooms est une liste d’un ou plusieurs éléments qui représentent des salles de réunion.
ms.openlocfilehash: f8b60a9680f6abba459ebecc96613abfdd93766d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466184"
---
# <a name="rooms"></a><span data-ttu-id="1e849-103">Salons</span><span class="sxs-lookup"><span data-stu-id="1e849-103">Rooms</span></span>

<span data-ttu-id="1e849-104">L’élément **rooms** est une liste d’un ou plusieurs éléments qui représentent des salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="1e849-104">The **Rooms** element is a list of one or more elements that represent meeting rooms.</span></span> 
  
[<span data-ttu-id="1e849-105">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="1e849-105">GetRoomsResponse</span></span>](getroomsresponse.md)
  
[<span data-ttu-id="1e849-106">Salons</span><span class="sxs-lookup"><span data-stu-id="1e849-106">Rooms</span></span>](rooms.md)
  
```xml
<Rooms>   <Room/></Rooms>
```

 <span data-ttu-id="1e849-107">**ArrayOfRoomsType**</span><span class="sxs-lookup"><span data-stu-id="1e849-107">**ArrayOfRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e849-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1e849-108">Attributes and elements</span></span>

<span data-ttu-id="1e849-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1e849-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e849-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="1e849-110">Attributes</span></span>

<span data-ttu-id="1e849-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1e849-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e849-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1e849-112">Child elements</span></span>

|<span data-ttu-id="1e849-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e849-113">**Element**</span></span>|<span data-ttu-id="1e849-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e849-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e849-115">Salle</span><span class="sxs-lookup"><span data-stu-id="1e849-115">Room</span></span>](room.md) <br/> |<span data-ttu-id="1e849-116">Définit une adresse de messagerie et un nom d’affichage qui représente une salle de réunion.</span><span class="sxs-lookup"><span data-stu-id="1e849-116">Defines an e-mail address and display name that represents a meeting room.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e849-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1e849-117">Parent elements</span></span>

|<span data-ttu-id="1e849-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e849-118">**Element**</span></span>|<span data-ttu-id="1e849-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e849-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e849-120">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="1e849-120">GetRoomsResponse</span></span>](getroomsresponse.md) <br/> ||
   
## <a name="remarks"></a><span data-ttu-id="1e849-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="1e849-121">Remarks</span></span>

<span data-ttu-id="1e849-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1e849-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e849-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1e849-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e849-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1e849-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1e849-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1e849-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1e849-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1e849-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1e849-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1e849-127">Validation File</span></span>  <br/> |<span data-ttu-id="1e849-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1e849-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1e849-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1e849-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e849-130">False</span><span class="sxs-lookup"><span data-stu-id="1e849-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e849-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1e849-131">See also</span></span>



[<span data-ttu-id="1e849-132">Opération GetRooms</span><span class="sxs-lookup"><span data-stu-id="1e849-132">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="1e849-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1e849-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

