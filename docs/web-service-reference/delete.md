---
title: Supprimer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: aa45f0c1-a80d-4b6c-8a85-375b6de515f4
description: L’élément delete indique si un client peut supprimer un dossier ou un élément.
ms.openlocfilehash: 5460f9e49b126ca6b039c6f11aaa3c6eb4a40544
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457353"
---
# <a name="delete"></a><span data-ttu-id="3e5f6-103">Supprimer</span><span class="sxs-lookup"><span data-stu-id="3e5f6-103">Delete</span></span>

<span data-ttu-id="3e5f6-104">L’élément **Delete** indique si un client peut supprimer un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-104">The **Delete** element indicates whether a client can delete a folder or item.</span></span> 
  
```XML
<Delete>true or false</Delete>
```

<span data-ttu-id="3e5f6-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="3e5f6-105">**boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3e5f6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e5f6-106">Attributes and elements</span></span>

<span data-ttu-id="3e5f6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e5f6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e5f6-108">Attributes</span></span>

<span data-ttu-id="3e5f6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e5f6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e5f6-110">Child elements</span></span>

<span data-ttu-id="3e5f6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3e5f6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e5f6-112">Parent elements</span></span>

|<span data-ttu-id="3e5f6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e5f6-113">**Element**</span></span>|<span data-ttu-id="3e5f6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e5f6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e5f6-115">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="3e5f6-115">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="3e5f6-116">Contient les droits du client en fonction des paramètres d’autorisation de l’élément ou du dossier.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-116">Contains the rights of the client based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="3e5f6-117">Actions</span><span class="sxs-lookup"><span data-stu-id="3e5f6-117">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="3e5f6-118">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-118">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e5f6-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3e5f6-119">Text value</span></span>

<span data-ttu-id="3e5f6-120">Une valeur de texte **true** indique qu’un client peut supprimer un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-120">A text value of **true** indicates that a client can delete an item or folder.</span></span> <span data-ttu-id="3e5f6-121">La valeur **false** indique qu’un client ne peut pas supprimer un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-121">A value of **false** indicates that a client cannot delete an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3e5f6-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e5f6-122">Remarks</span></span>

<span data-ttu-id="3e5f6-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e5f6-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e5f6-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e5f6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e5f6-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e5f6-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e5f6-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e5f6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3e5f6-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3e5f6-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e5f6-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e5f6-128">Validation File</span></span>  <br/> |<span data-ttu-id="3e5f6-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3e5f6-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e5f6-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e5f6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e5f6-131">False</span><span class="sxs-lookup"><span data-stu-id="3e5f6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e5f6-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e5f6-132">See also</span></span>

- [<span data-ttu-id="3e5f6-133">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e5f6-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="3e5f6-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="3e5f6-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

