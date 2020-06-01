---
title: ServerReplyWithMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerReplyWithMessage
api_type:
- schema
ms.assetid: 113c6ff2-9592-44f0-b542-54e4d5122ccb
description: L’élément ServerReplyWithMessage indique l’ID du message de modèle à envoyer en tant que réponse aux messages entrants.
ms.openlocfilehash: faaa054018a17be3ff59b9fc385b3d846d39c3f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461974"
---
# <a name="serverreplywithmessage"></a><span data-ttu-id="7d811-103">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="7d811-103">ServerReplyWithMessage</span></span>

<span data-ttu-id="7d811-104">L’élément **ServerReplyWithMessage** indique l’ID du message de modèle à envoyer en tant que réponse aux messages entrants.</span><span class="sxs-lookup"><span data-stu-id="7d811-104">The **ServerReplyWithMessage** element indicates the ID of the template message that is to be sent as a reply to incoming messages.</span></span> 
  
```XML
<ServerReplyWithMessage>
    <ItemId>
</ServerReplyWithMessage>
```

 <span data-ttu-id="7d811-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="7d811-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d811-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7d811-106">Attributes and elements</span></span>

<span data-ttu-id="7d811-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7d811-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d811-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7d811-108">Attributes</span></span>

<span data-ttu-id="7d811-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7d811-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d811-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7d811-110">Child elements</span></span>

|<span data-ttu-id="7d811-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7d811-111">**Element**</span></span>|<span data-ttu-id="7d811-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d811-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d811-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="7d811-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7d811-114">Représente l’identificateur unique et la clé de modification d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d811-114">Represents the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d811-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7d811-115">Parent elements</span></span>

|<span data-ttu-id="7d811-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7d811-116">**Element**</span></span>|<span data-ttu-id="7d811-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d811-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d811-118">Actions</span><span class="sxs-lookup"><span data-stu-id="7d811-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="7d811-119">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="7d811-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d811-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7d811-120">Text value</span></span>

<span data-ttu-id="7d811-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d811-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7d811-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="7d811-122">Remarks</span></span>

<span data-ttu-id="7d811-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d811-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d811-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7d811-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d811-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7d811-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d811-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7d811-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7d811-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7d811-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d811-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7d811-128">Validation File</span></span>  <br/> |<span data-ttu-id="7d811-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7d811-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d811-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7d811-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d811-131">True</span><span class="sxs-lookup"><span data-stu-id="7d811-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d811-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d811-132">See also</span></span>



- [<span data-ttu-id="7d811-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7d811-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

