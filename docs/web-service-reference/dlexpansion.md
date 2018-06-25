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
description: L’élément DLExpansion contient un tableau de boîtes aux lettres qui sont contenus dans une liste de distribution.
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756025"
---
# <a name="dlexpansion"></a><span data-ttu-id="77d74-103">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="77d74-103">DLExpansion</span></span>

<span data-ttu-id="77d74-104">L’élément **DLExpansion** contient un tableau de boîtes aux lettres qui sont contenus dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="77d74-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="77d74-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="77d74-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="77d74-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="77d74-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="77d74-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77d74-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="77d74-108">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="77d74-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="77d74-109">**ArrayOfDLExpansionType**</span><span class="sxs-lookup"><span data-stu-id="77d74-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77d74-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="77d74-110">Attributes and elements</span></span>

<span data-ttu-id="77d74-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="77d74-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77d74-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="77d74-112">Attributes</span></span>

|<span data-ttu-id="77d74-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="77d74-113">**Attribute**</span></span>|<span data-ttu-id="77d74-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="77d74-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="77d74-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="77d74-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="77d74-116">Représente l’index suivant doit être utilisé pour la requête suivante lorsque vous utilisez un affichage de page indexés.</span><span class="sxs-lookup"><span data-stu-id="77d74-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="77d74-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="77d74-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="77d74-118">Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.</span><span class="sxs-lookup"><span data-stu-id="77d74-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="77d74-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="77d74-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="77d74-120">Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.</span><span class="sxs-lookup"><span data-stu-id="77d74-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="77d74-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="77d74-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="77d74-122">Indique si les résultats actuels contient le dernier élément dans la requête afin que le fichier d’échange supplémentaire n’est pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="77d74-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="77d74-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="77d74-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="77d74-124">Représente le nombre total d’éléments dans l’affichage.</span><span class="sxs-lookup"><span data-stu-id="77d74-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="77d74-125">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="77d74-125">Child elements</span></span>

|<span data-ttu-id="77d74-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="77d74-126">**Element**</span></span>|<span data-ttu-id="77d74-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="77d74-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77d74-128">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="77d74-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="77d74-129">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="77d74-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77d74-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="77d74-130">Parent elements</span></span>

|<span data-ttu-id="77d74-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="77d74-131">**Element**</span></span>|<span data-ttu-id="77d74-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="77d74-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77d74-133">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77d74-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="77d74-134">Contient l’état et les résultats d’une seule demande ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="77d74-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="77d74-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="77d74-135">Remarks</span></span>

<span data-ttu-id="77d74-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="77d74-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77d74-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="77d74-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77d74-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="77d74-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77d74-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="77d74-139">Schema Name</span></span>  <br/> |<span data-ttu-id="77d74-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="77d74-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="77d74-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="77d74-141">Validation File</span></span>  <br/> |<span data-ttu-id="77d74-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="77d74-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77d74-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="77d74-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="77d74-144">False</span><span class="sxs-lookup"><span data-stu-id="77d74-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77d74-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="77d74-145">See also</span></span>

- [<span data-ttu-id="77d74-146">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="77d74-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="77d74-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="77d74-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="77d74-148">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="77d74-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

