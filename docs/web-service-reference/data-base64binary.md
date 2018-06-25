---
title: Données (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: L’élément de données contient les données d’un seul élément exporté ou un élément à télécharger dans une boîte aux lettres.
ms.openlocfilehash: 9560273e31a64edb2254489961733dfe7360ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755786"
---
# <a name="data-base64binary"></a><span data-ttu-id="1bd3a-103">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="1bd3a-103">Data (base64Binary)</span></span>

<span data-ttu-id="1bd3a-104">L’élément de **données** contient les données d’un seul élément exporté ou un élément à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1bd3a-104">The **Data** element contains the data of a single exported item or an item to upload into a mailbox.</span></span> 
  
```XML
<Data/>
```

<span data-ttu-id="1bd3a-105">**xs : base64Binary**</span><span class="sxs-lookup"><span data-stu-id="1bd3a-105">**xs:base64Binary**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1bd3a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1bd3a-106">Attributes and elements</span></span>

<span data-ttu-id="1bd3a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1bd3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bd3a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1bd3a-108">Attributes</span></span>

<span data-ttu-id="1bd3a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1bd3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1bd3a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1bd3a-110">Child elements</span></span>

<span data-ttu-id="1bd3a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1bd3a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1bd3a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1bd3a-112">Parent elements</span></span>

|<span data-ttu-id="1bd3a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1bd3a-113">**Element**</span></span>|<span data-ttu-id="1bd3a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bd3a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bd3a-115">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1bd3a-115">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="1bd3a-116">Contient l’état et les résultats d’une demande pour exporter un élément de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="1bd3a-116">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="1bd3a-117">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="1bd3a-117">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="1bd3a-118">Représente un seul élément à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1bd3a-118">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1bd3a-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1bd3a-119">Text value</span></span>

<span data-ttu-id="1bd3a-120">L’élément de **données** contient les noms de propriétés et les valeurs d’un élément exporté ou un élément dans une boîte aux lettres sera téléchargé.</span><span class="sxs-lookup"><span data-stu-id="1bd3a-120">The **Data** element contains the property names and values for an exported item or an item that will be uploaded into a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1bd3a-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="1bd3a-121">Remarks</span></span>

<span data-ttu-id="1bd3a-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1bd3a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bd3a-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1bd3a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bd3a-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1bd3a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1bd3a-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1bd3a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1bd3a-126">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="1bd3a-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="1bd3a-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1bd3a-127">Validation File</span></span>  <br/> |<span data-ttu-id="1bd3a-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1bd3a-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1bd3a-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1bd3a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="1bd3a-130">False</span><span class="sxs-lookup"><span data-stu-id="1bd3a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1bd3a-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1bd3a-131">See also</span></span>

- [<span data-ttu-id="1bd3a-132">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="1bd3a-132">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="1bd3a-133">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="1bd3a-133">UploadItems operation</span></span>](uploaditems-operation.md)

