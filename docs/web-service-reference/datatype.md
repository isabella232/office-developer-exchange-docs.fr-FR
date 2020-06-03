---
title: DataType
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
description: L’élément DataType décrit le type de données partagées par un dossier partagé.
ms.openlocfilehash: a7df8d38e10f0ab31038d790d8f35208d1be66d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458830"
---
# <a name="datatype"></a><span data-ttu-id="63e54-103">DataType</span><span class="sxs-lookup"><span data-stu-id="63e54-103">DataType</span></span>

<span data-ttu-id="63e54-104">L’élément **DataType** décrit le type de données partagées par un dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="63e54-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="63e54-105">**SharingDataType**</span><span class="sxs-lookup"><span data-stu-id="63e54-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="63e54-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="63e54-106">Attributes and elements</span></span>

<span data-ttu-id="63e54-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="63e54-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63e54-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="63e54-108">Attributes</span></span>

<span data-ttu-id="63e54-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="63e54-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63e54-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="63e54-110">Child elements</span></span>

<span data-ttu-id="63e54-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="63e54-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63e54-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="63e54-112">Parent elements</span></span>

|<span data-ttu-id="63e54-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63e54-113">**Element**</span></span>|<span data-ttu-id="63e54-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="63e54-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63e54-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="63e54-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="63e54-116">Définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.</span><span class="sxs-lookup"><span data-stu-id="63e54-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63e54-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="63e54-117">Text value</span></span>

<span data-ttu-id="63e54-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **DataType** .</span><span class="sxs-lookup"><span data-stu-id="63e54-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="63e54-119">**Valeurs des éléments DataType**</span><span class="sxs-lookup"><span data-stu-id="63e54-119">**DataType element values**</span></span>

|<span data-ttu-id="63e54-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="63e54-120">**Value**</span></span>|<span data-ttu-id="63e54-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="63e54-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="63e54-122">Calendrier</span><span class="sxs-lookup"><span data-stu-id="63e54-122">Calendar</span></span>  <br/> |<span data-ttu-id="63e54-123">Indique que le dossier partagé contient des informations de calendrier.</span><span class="sxs-lookup"><span data-stu-id="63e54-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="63e54-124">Contacts</span><span class="sxs-lookup"><span data-stu-id="63e54-124">Contacts</span></span>  <br/> |<span data-ttu-id="63e54-125">Indique que le dossier partagé contient des informations de contact.</span><span class="sxs-lookup"><span data-stu-id="63e54-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63e54-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="63e54-126">Remarks</span></span>

<span data-ttu-id="63e54-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="63e54-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63e54-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="63e54-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63e54-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="63e54-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63e54-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="63e54-130">Schema Name</span></span>  <br/> |<span data-ttu-id="63e54-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="63e54-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="63e54-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="63e54-132">Validation File</span></span>  <br/> |<span data-ttu-id="63e54-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="63e54-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63e54-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="63e54-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="63e54-135">False</span><span class="sxs-lookup"><span data-stu-id="63e54-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63e54-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="63e54-136">See also</span></span>

- [<span data-ttu-id="63e54-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="63e54-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

