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
description: L’élément Data contient les données d’un seul élément exporté ou d’un élément à charger dans une boîte aux lettres.
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526969"
---
# <a name="data-base64binary"></a><span data-ttu-id="f9bb4-103">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="f9bb4-103">Data (base64Binary)</span></span>

<span data-ttu-id="f9bb4-104">L’élément **Data** contient les données d’un seul élément exporté ou d’un élément à charger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f9bb4-104">The **Data** element contains the data of a single exported item or an item to upload into a mailbox.</span></span> 
  
```XML
<Data/>
```

<span data-ttu-id="f9bb4-105">**XS : base64Binary**</span><span class="sxs-lookup"><span data-stu-id="f9bb4-105">**xs:base64Binary**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f9bb4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f9bb4-106">Attributes and elements</span></span>

<span data-ttu-id="f9bb4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f9bb4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9bb4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f9bb4-108">Attributes</span></span>

<span data-ttu-id="f9bb4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f9bb4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9bb4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f9bb4-110">Child elements</span></span>

<span data-ttu-id="f9bb4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f9bb4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9bb4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f9bb4-112">Parent elements</span></span>

|<span data-ttu-id="f9bb4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9bb4-113">**Element**</span></span>|<span data-ttu-id="f9bb4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9bb4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9bb4-115">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9bb4-115">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="f9bb4-116">Contient l’État et les résultats d’une demande d’exportation d’un seul élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f9bb4-116">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="f9bb4-117">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="f9bb4-117">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="f9bb4-118">Représente un élément unique à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f9bb4-118">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f9bb4-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f9bb4-119">Text value</span></span>

<span data-ttu-id="f9bb4-120">L’élément **Data** contient les valeurs et les noms des propriétés d’un élément exporté ou d’un élément qui sera chargé dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f9bb4-120">The **Data** element contains the property names and values for an exported item or an item that will be uploaded into a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f9bb4-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="f9bb4-121">Remarks</span></span>

<span data-ttu-id="f9bb4-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f9bb4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9bb4-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f9bb4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9bb4-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f9bb4-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f9bb4-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f9bb4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f9bb4-126">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="f9bb4-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="f9bb4-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f9bb4-127">Validation File</span></span>  <br/> |<span data-ttu-id="f9bb4-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f9bb4-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f9bb4-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f9bb4-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9bb4-130">False</span><span class="sxs-lookup"><span data-stu-id="f9bb4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9bb4-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f9bb4-131">See also</span></span>

- [<span data-ttu-id="f9bb4-132">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="f9bb4-132">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="f9bb4-133">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="f9bb4-133">UploadItems operation</span></span>](uploaditems-operation.md)

