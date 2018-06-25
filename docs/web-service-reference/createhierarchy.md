---
title: CreateHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateHierarchy
api_type:
- schema
ms.assetid: 630b5610-1c19-4d4a-a5df-8cebb9afd2f4
description: L’élément CreateHierarchy indique si un client peut créer une table de hiérarchie. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a5b428fe453dbc31761309b017367a7d25a01b76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755707"
---
# <a name="createhierarchy"></a><span data-ttu-id="e8579-104">CreateHierarchy</span><span class="sxs-lookup"><span data-stu-id="e8579-104">CreateHierarchy</span></span>

<span data-ttu-id="e8579-105">L’élément **CreateHierarchy** indique si un client peut créer une table de hiérarchie.</span><span class="sxs-lookup"><span data-stu-id="e8579-105">The **CreateHierarchy** element indicates whether a client can create a hierarchy table.</span></span> <span data-ttu-id="e8579-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e8579-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateHierarchy>true or false</CreateHierarchy>
```

 <span data-ttu-id="e8579-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e8579-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8579-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e8579-108">Attributes and elements</span></span>

<span data-ttu-id="e8579-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e8579-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8579-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="e8579-110">Attributes</span></span>

<span data-ttu-id="e8579-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e8579-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8579-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e8579-112">Child elements</span></span>

<span data-ttu-id="e8579-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e8579-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8579-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e8579-114">Parent elements</span></span>

|<span data-ttu-id="e8579-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e8579-115">**Element**</span></span>|<span data-ttu-id="e8579-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="e8579-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8579-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="e8579-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="e8579-118">Contient les droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="e8579-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="e8579-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="e8579-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8579-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e8579-120">Text value</span></span>

<span data-ttu-id="e8579-121">Une valeur de texte de **la valeur true** indique qu’un client peut créer une table de hiérarchie.</span><span class="sxs-lookup"><span data-stu-id="e8579-121">A text value of **true** indicates that a client can create a hierarchy table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e8579-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="e8579-122">Remarks</span></span>

<span data-ttu-id="e8579-123">Cette propriété est utilisée uniquement avec des objets folder.</span><span class="sxs-lookup"><span data-stu-id="e8579-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="e8579-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e8579-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8579-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e8579-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8579-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e8579-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8579-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e8579-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e8579-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e8579-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8579-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e8579-129">Validation File</span></span>  <br/> |<span data-ttu-id="e8579-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e8579-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8579-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e8579-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8579-132">False</span><span class="sxs-lookup"><span data-stu-id="e8579-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8579-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e8579-133">See also</span></span>



- [<span data-ttu-id="e8579-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e8579-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e8579-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="e8579-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

