---
title: PlayOnPhone (services Web Exchange)
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
ms.openlocfilehash: e2c09a67255106ad9afddb86fa19b7a4a5762ee5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466247"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="0ee57-103">PlayOnPhone (services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="0ee57-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="0ee57-104">L’élément **PlayOnPhone** représente une demande de lecture d’un élément sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="0ee57-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="0ee57-105">**PlayOnPhoneType**</span><span class="sxs-lookup"><span data-stu-id="0ee57-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ee57-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0ee57-106">Attributes and elements</span></span>

<span data-ttu-id="0ee57-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0ee57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ee57-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0ee57-108">Attributes</span></span>

<span data-ttu-id="0ee57-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0ee57-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ee57-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0ee57-110">Child elements</span></span>

|<span data-ttu-id="0ee57-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ee57-111">**Element**</span></span>|<span data-ttu-id="0ee57-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ee57-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ee57-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="0ee57-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0ee57-114">Représente l’identificateur d’un élément à lire sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="0ee57-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="0ee57-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0ee57-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0ee57-116">DialString (services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="0ee57-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="0ee57-117">Représente la chaîne de numérotation du numéro de téléphone qui est appelé pour lire un élément par téléphone.</span><span class="sxs-lookup"><span data-stu-id="0ee57-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="0ee57-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0ee57-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ee57-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0ee57-119">Parent elements</span></span>

<span data-ttu-id="0ee57-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0ee57-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ee57-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ee57-121">Remarks</span></span>

<span data-ttu-id="0ee57-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0ee57-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ee57-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0ee57-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ee57-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0ee57-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ee57-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0ee57-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0ee57-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0ee57-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ee57-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0ee57-127">Validation File</span></span>  <br/> |<span data-ttu-id="0ee57-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0ee57-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ee57-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0ee57-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ee57-130">False</span><span class="sxs-lookup"><span data-stu-id="0ee57-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ee57-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ee57-131">See also</span></span>



- [<span data-ttu-id="0ee57-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0ee57-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

