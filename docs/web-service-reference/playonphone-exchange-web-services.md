---
title: PlayOnPhone (Exchange Web Services)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 486612be-470c-4f99-929a-f2b283e055c1
description: L’élément PlayOnPhone représente une demande de lecture d’un élément sur un téléphone.
ms.openlocfilehash: 75493a31940ea609fd6cf454e91ca5881fb7e678
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828816"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="d5fd8-103">PlayOnPhone (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="d5fd8-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="d5fd8-104">L’élément **PlayOnPhone** représente une demande de lecture d’un élément sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="d5fd8-105">**PlayOnPhoneType**</span><span class="sxs-lookup"><span data-stu-id="d5fd8-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5fd8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d5fd8-106">Attributes and elements</span></span>

<span data-ttu-id="d5fd8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5fd8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d5fd8-108">Attributes</span></span>

<span data-ttu-id="d5fd8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5fd8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d5fd8-110">Child elements</span></span>

|<span data-ttu-id="d5fd8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5fd8-111">**Element**</span></span>|<span data-ttu-id="d5fd8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5fd8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5fd8-113">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="d5fd8-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d5fd8-114">Représente l’identificateur d’un élément à lire sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="d5fd8-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d5fd8-116">DialString (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="d5fd8-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="d5fd8-117">Représente la chaîne de numérotation du numéro de téléphone qui est appelée pour lire un élément par téléphone.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="d5fd8-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5fd8-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d5fd8-119">Parent elements</span></span>

<span data-ttu-id="d5fd8-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5fd8-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="d5fd8-121">Remarks</span></span>

<span data-ttu-id="d5fd8-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="d5fd8-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5fd8-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d5fd8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5fd8-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d5fd8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5fd8-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d5fd8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d5fd8-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d5fd8-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5fd8-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d5fd8-127">Validation File</span></span>  <br/> |<span data-ttu-id="d5fd8-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d5fd8-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5fd8-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d5fd8-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5fd8-130">False</span><span class="sxs-lookup"><span data-stu-id="d5fd8-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5fd8-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d5fd8-131">See also</span></span>



- [<span data-ttu-id="d5fd8-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d5fd8-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

