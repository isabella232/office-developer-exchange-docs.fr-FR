---
title: DLExpansion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: L’élément DLExpansion contient un tableau de boîtes aux lettres contenues dans une liste de distribution.
ms.openlocfilehash: 079ad1c0f114d201f5d1b91c3fd9bb45b943cc1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456996"
---
# <a name="dlexpansion"></a><span data-ttu-id="7dfb0-103">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="7dfb0-103">DLExpansion</span></span>

<span data-ttu-id="7dfb0-104">L’élément **DLExpansion** contient un tableau de boîtes aux lettres contenues dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="7dfb0-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="7dfb0-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="7dfb0-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7dfb0-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="7dfb0-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7dfb0-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="7dfb0-108">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="7dfb0-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="7dfb0-109">**ArrayOfDLExpansionType**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7dfb0-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7dfb0-110">Attributes and elements</span></span>

<span data-ttu-id="7dfb0-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7dfb0-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="7dfb0-112">Attributes</span></span>

|<span data-ttu-id="7dfb0-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-113">**Attribute**</span></span>|<span data-ttu-id="7dfb0-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7dfb0-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="7dfb0-116">Représente l’index suivant qui doit être utilisé pour la requête suivante lorsque vous utilisez une vue de page indexée.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="7dfb0-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="7dfb0-118">Représente la nouvelle valeur de numérateur à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fractions.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="7dfb0-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="7dfb0-120">Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fractions.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="7dfb0-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="7dfb0-122">Indique si les résultats actuels contiennent le dernier élément de la requête afin de ne pas avoir besoin d’une pagination supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="7dfb0-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="7dfb0-124">Représente le nombre total d’éléments dans l’affichage.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7dfb0-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7dfb0-125">Child elements</span></span>

|<span data-ttu-id="7dfb0-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-126">**Element**</span></span>|<span data-ttu-id="7dfb0-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dfb0-128">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="7dfb0-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="7dfb0-129">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7dfb0-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7dfb0-130">Parent elements</span></span>

|<span data-ttu-id="7dfb0-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-131">**Element**</span></span>|<span data-ttu-id="7dfb0-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="7dfb0-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dfb0-133">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7dfb0-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="7dfb0-134">Contient l’État et le résultat d’une seule demande ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7dfb0-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="7dfb0-135">Remarks</span></span>

<span data-ttu-id="7dfb0-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7dfb0-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7dfb0-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7dfb0-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7dfb0-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7dfb0-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7dfb0-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7dfb0-139">Schema Name</span></span>  <br/> |<span data-ttu-id="7dfb0-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7dfb0-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="7dfb0-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7dfb0-141">Validation File</span></span>  <br/> |<span data-ttu-id="7dfb0-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7dfb0-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7dfb0-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7dfb0-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="7dfb0-144">False</span><span class="sxs-lookup"><span data-stu-id="7dfb0-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7dfb0-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7dfb0-145">See also</span></span>

- [<span data-ttu-id="7dfb0-146">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="7dfb0-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="7dfb0-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7dfb0-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="7dfb0-148">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7dfb0-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

