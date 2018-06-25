---
title: UnknownEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntry
api_type:
- schema
ms.assetid: 3cb4c62e-052a-4326-8639-8c41dfd047b2
description: L’élément UnknownEntry représente une entrée d’autorisation inconnu unique qui ne peut pas être résolue en fonction du service d’annuaire Active Directory. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 11939ad39c83ac2d15ec7fface6f530d3f60e12a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838834"
---
# <a name="unknownentry"></a><span data-ttu-id="96144-104">UnknownEntry</span><span class="sxs-lookup"><span data-stu-id="96144-104">UnknownEntry</span></span>

<span data-ttu-id="96144-105">L’élément **UnknownEntry** représente une entrée d’autorisation inconnu unique qui ne peut pas être résolue en fonction du service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="96144-105">The **UnknownEntry** element represents a single unknown permission entry that cannot be resolved against the Active Directory directory service.</span></span> <span data-ttu-id="96144-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="96144-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UnknownEntry/>
```

 <span data-ttu-id="96144-107">**string**</span><span class="sxs-lookup"><span data-stu-id="96144-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96144-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="96144-108">Attributes and elements</span></span>

<span data-ttu-id="96144-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="96144-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96144-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="96144-110">Attributes</span></span>

<span data-ttu-id="96144-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="96144-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96144-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="96144-112">Child elements</span></span>

<span data-ttu-id="96144-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="96144-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96144-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="96144-114">Parent elements</span></span>

|<span data-ttu-id="96144-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="96144-115">**Element**</span></span>|<span data-ttu-id="96144-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="96144-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96144-117">UnknownEntries</span><span class="sxs-lookup"><span data-stu-id="96144-117">UnknownEntries</span></span>](unknownentries.md) <br/> |<span data-ttu-id="96144-118">Contient un tableau d’entrées d’autorisation inconnu qui ne peut pas être résolu par rapport à Active Directory.</span><span class="sxs-lookup"><span data-stu-id="96144-118">Contains an array of unknown permission entries that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="96144-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="96144-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96144-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="96144-120">Text value</span></span>

<span data-ttu-id="96144-121">La valeur de texte représente une entrée d’autorisation ne peut pas être résolue par rapport à Active Directory.</span><span class="sxs-lookup"><span data-stu-id="96144-121">The text value represents a permission entry that cannot be resolved against Active Directory.</span></span> <span data-ttu-id="96144-122">La valeur de texte représente un identificateur de sécurité (SID).</span><span class="sxs-lookup"><span data-stu-id="96144-122">The text value represents a security identifier (SID).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96144-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="96144-123">Remarks</span></span>

<span data-ttu-id="96144-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="96144-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96144-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="96144-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96144-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="96144-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96144-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="96144-127">Schema Name</span></span>  <br/> |<span data-ttu-id="96144-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="96144-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="96144-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="96144-129">Validation File</span></span>  <br/> |<span data-ttu-id="96144-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="96144-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96144-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="96144-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="96144-132">False</span><span class="sxs-lookup"><span data-stu-id="96144-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96144-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="96144-133">See also</span></span>



- [<span data-ttu-id="96144-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="96144-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="96144-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="96144-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

