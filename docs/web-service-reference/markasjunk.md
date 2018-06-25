---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: L’élément MarkAsJunk spécifie la demande pour déplacer un élément vers le dossier courrier indésirable et d’ajouter l’expéditeur à la liste des expéditeurs bloqués.
ms.openlocfilehash: fbb3eee7ce350954888931ca55b27f596656b161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828350"
---
# <a name="markasjunk"></a><span data-ttu-id="30d59-103">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="30d59-103">MarkAsJunk</span></span>

<span data-ttu-id="30d59-104">L’élément **MarkAsJunk** spécifie la demande pour déplacer un élément vers le dossier courrier indésirable et d’ajouter l’expéditeur à la liste des expéditeurs bloqués.</span><span class="sxs-lookup"><span data-stu-id="30d59-104">The **MarkAsJunk** element specifies the request to move an item to the junk mail folder and to add the sender to the blocked sender list.</span></span> 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 <span data-ttu-id="30d59-105">**MarkAsJunkType**</span><span class="sxs-lookup"><span data-stu-id="30d59-105">**MarkAsJunkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30d59-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="30d59-106">Attributes and elements</span></span>

<span data-ttu-id="30d59-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="30d59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30d59-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="30d59-108">Attributes</span></span>

|<span data-ttu-id="30d59-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="30d59-109">**Attribute**</span></span>|<span data-ttu-id="30d59-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="30d59-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30d59-111">IsJunk</span><span class="sxs-lookup"><span data-stu-id="30d59-111">IsJunk</span></span>  <br/> |<span data-ttu-id="30d59-112">Une valeur de texte de **la valeur true** pour l’attribut **IsJunk** indique que l’expéditeur est ajouté à la liste des expéditeurs bloqués.</span><span class="sxs-lookup"><span data-stu-id="30d59-112">A text value of **true** for the **IsJunk** attribute indicates that the email sender is added to the blocked sender list.</span></span> <span data-ttu-id="30d59-113">La valeur **false** indique que l’expéditeur est supprimé de la liste des expéditeurs bloqués, si l’expéditeur figure déjà dans la liste.</span><span class="sxs-lookup"><span data-stu-id="30d59-113">A value of **false** indicates that the email sender is removed from the blocked sender list, if the email sender is already on the list.</span></span>  <br/> |
|<span data-ttu-id="30d59-114">MoveItem</span><span class="sxs-lookup"><span data-stu-id="30d59-114">MoveItem</span></span>  <br/> |<span data-ttu-id="30d59-115">Une valeur de texte de **la valeur true** pour l’attribut **MoveItem** indique que l’élément est déplacé vers le dossier de courrier indésirable par défaut.</span><span class="sxs-lookup"><span data-stu-id="30d59-115">A text value of **true** for the **MoveItem** attribute indicates that the item is moved to the default junk mail folder.</span></span> <span data-ttu-id="30d59-116">La valeur **false** indique que l’élément n’est pas déplacé vers le dossier de courrier indésirable par défaut.</span><span class="sxs-lookup"><span data-stu-id="30d59-116">A value of **false** indicates that the item is not moved to the default junk mail folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="30d59-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="30d59-117">Child elements</span></span>

[<span data-ttu-id="30d59-118">ItemId</span><span class="sxs-lookup"><span data-stu-id="30d59-118">ItemIds</span></span>](itemids.md)
  
### <a name="parent-elements"></a><span data-ttu-id="30d59-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="30d59-119">Parent elements</span></span>

<span data-ttu-id="30d59-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30d59-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30d59-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="30d59-121">Remarks</span></span>

<span data-ttu-id="30d59-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="30d59-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30d59-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="30d59-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30d59-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="30d59-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30d59-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="30d59-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30d59-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="30d59-126">Schema name</span></span>  <br/> |<span data-ttu-id="30d59-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="30d59-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30d59-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="30d59-128">Validation file</span></span>  <br/> |<span data-ttu-id="30d59-129">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30d59-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30d59-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="30d59-130">Can be empty</span></span>  <br/> ||
   

