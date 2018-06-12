---
title: Type de données
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DataType
api_type:
- schema
ms.assetid: 267fe5aa-f9b1-4d4c-ac11-0f2e50ec2627
description: L’élément de type de données décrit le type de données qui sont partagés par un dossier partagé.
ms.openlocfilehash: b1adac8e3029abd64df96ab1560706babe4b12f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755804"
---
# <a name="datatype"></a><span data-ttu-id="dd5b8-103">Type de données</span><span class="sxs-lookup"><span data-stu-id="dd5b8-103">DataType</span></span>

<span data-ttu-id="dd5b8-104">L’élément de **type de données** décrit le type de données qui sont partagés par un dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="dd5b8-105">**SharingDataType**</span><span class="sxs-lookup"><span data-stu-id="dd5b8-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dd5b8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dd5b8-106">Attributes and elements</span></span>

<span data-ttu-id="dd5b8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd5b8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dd5b8-108">Attributes</span></span>

<span data-ttu-id="dd5b8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd5b8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dd5b8-110">Child elements</span></span>

<span data-ttu-id="dd5b8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd5b8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dd5b8-112">Parent elements</span></span>

|<span data-ttu-id="dd5b8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dd5b8-113">**Element**</span></span>|<span data-ttu-id="dd5b8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="dd5b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd5b8-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="dd5b8-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="dd5b8-116">Définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd5b8-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="dd5b8-117">Text value</span></span>

<span data-ttu-id="dd5b8-118">Le tableau suivant répertorie les valeurs possibles pour l’élément de **type de données** .</span><span class="sxs-lookup"><span data-stu-id="dd5b8-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="dd5b8-119">**Valeurs des éléments de type de données**</span><span class="sxs-lookup"><span data-stu-id="dd5b8-119">**DataType element values**</span></span>

|<span data-ttu-id="dd5b8-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="dd5b8-120">**Value**</span></span>|<span data-ttu-id="dd5b8-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="dd5b8-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dd5b8-122">Calendrier</span><span class="sxs-lookup"><span data-stu-id="dd5b8-122">Calendar</span></span>  <br/> |<span data-ttu-id="dd5b8-123">Indique que le dossier partagé contienne des informations de calendrier.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="dd5b8-124">Contacts</span><span class="sxs-lookup"><span data-stu-id="dd5b8-124">Contacts</span></span>  <br/> |<span data-ttu-id="dd5b8-125">Indique que le dossier partagé contienne des informations de contact.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd5b8-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="dd5b8-126">Remarks</span></span>

<span data-ttu-id="dd5b8-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd5b8-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd5b8-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dd5b8-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd5b8-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dd5b8-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd5b8-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dd5b8-130">Schema Name</span></span>  <br/> |<span data-ttu-id="dd5b8-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="dd5b8-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd5b8-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dd5b8-132">Validation File</span></span>  <br/> |<span data-ttu-id="dd5b8-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd5b8-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd5b8-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dd5b8-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd5b8-135">False</span><span class="sxs-lookup"><span data-stu-id="dd5b8-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd5b8-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dd5b8-136">See also</span></span>

- [<span data-ttu-id="dd5b8-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dd5b8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

