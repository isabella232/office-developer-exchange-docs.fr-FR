---
title: Suppression
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
description: L’élément Supprimer indique si un client peut supprimer un dossier ou un élément.
ms.openlocfilehash: 8a00a24ea63fa564ecefb96a5caed3a9199690eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755843"
---
# <a name="delete"></a><span data-ttu-id="089ba-103">Suppression</span><span class="sxs-lookup"><span data-stu-id="089ba-103">Delete</span></span>

<span data-ttu-id="089ba-104">L’élément **Supprimer** indique si un client peut supprimer un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="089ba-104">The **Delete** element indicates whether a client can delete a folder or item.</span></span> 
  
```XML
<Delete>true or false</Delete>
```

<span data-ttu-id="089ba-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="089ba-105">**boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="089ba-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="089ba-106">Attributes and elements</span></span>

<span data-ttu-id="089ba-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="089ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="089ba-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="089ba-108">Attributes</span></span>

<span data-ttu-id="089ba-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="089ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="089ba-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="089ba-110">Child elements</span></span>

<span data-ttu-id="089ba-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="089ba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="089ba-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="089ba-112">Parent elements</span></span>

|<span data-ttu-id="089ba-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="089ba-113">**Element**</span></span>|<span data-ttu-id="089ba-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="089ba-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="089ba-115">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="089ba-115">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="089ba-116">Contient les droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="089ba-116">Contains the rights of the client based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="089ba-117">Actions</span><span class="sxs-lookup"><span data-stu-id="089ba-117">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="089ba-118">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="089ba-118">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="089ba-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="089ba-119">Text value</span></span>

<span data-ttu-id="089ba-120">Texte la valeur **true** indique qu’un client peut supprimer un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="089ba-120">A text value of **true** indicates that a client can delete an item or folder.</span></span> <span data-ttu-id="089ba-121">La valeur **false** indique qu’un client ne peut pas supprimer un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="089ba-121">A value of **false** indicates that a client cannot delete an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="089ba-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="089ba-122">Remarks</span></span>

<span data-ttu-id="089ba-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="089ba-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="089ba-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="089ba-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="089ba-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="089ba-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="089ba-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="089ba-126">Schema Name</span></span>  <br/> |<span data-ttu-id="089ba-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="089ba-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="089ba-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="089ba-128">Validation File</span></span>  <br/> |<span data-ttu-id="089ba-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="089ba-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="089ba-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="089ba-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="089ba-131">False</span><span class="sxs-lookup"><span data-stu-id="089ba-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="089ba-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="089ba-132">See also</span></span>

- [<span data-ttu-id="089ba-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="089ba-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="089ba-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="089ba-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

