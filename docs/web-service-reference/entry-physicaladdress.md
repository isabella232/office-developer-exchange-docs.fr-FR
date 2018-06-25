---
title: Entrée (PhysicalAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: L’élément d’entrée décrit une seule adresse physique pour un élément de contact.
ms.openlocfilehash: 4551e6117e5f91d901fe160f37e8f67cb1bc5ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756195"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="97727-103">Entrée (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="97727-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="97727-104">L’élément **d’entrée** décrit une seule adresse physique pour un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="97727-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="97727-105">**PhysicalAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="97727-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97727-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="97727-106">Attributes and elements</span></span>

<span data-ttu-id="97727-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="97727-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97727-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="97727-108">Attributes</span></span>

|<span data-ttu-id="97727-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="97727-109">**Attribute**</span></span>|<span data-ttu-id="97727-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="97727-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97727-111">**Clé**</span><span class="sxs-lookup"><span data-stu-id="97727-111">**Key**</span></span> <br/> | <span data-ttu-id="97727-112">Identifie une adresse physique.</span><span class="sxs-lookup"><span data-stu-id="97727-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="97727-113">Les valeurs possibles de cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="97727-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="97727-114">-Business</span><span class="sxs-lookup"><span data-stu-id="97727-114">-  Business</span></span>  <br/><span data-ttu-id="97727-115">-Accueil</span><span class="sxs-lookup"><span data-stu-id="97727-115">-  Home</span></span>  <br/><span data-ttu-id="97727-116">-Autres</span><span class="sxs-lookup"><span data-stu-id="97727-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="97727-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="97727-117">Child elements</span></span>

|<span data-ttu-id="97727-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97727-118">**Element**</span></span>|<span data-ttu-id="97727-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="97727-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97727-120">Street</span><span class="sxs-lookup"><span data-stu-id="97727-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="97727-121">Représente une adresse postale pour un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="97727-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="97727-122">Ville</span><span class="sxs-lookup"><span data-stu-id="97727-122">City</span></span>](city.md) <br/> |<span data-ttu-id="97727-123">Représente le nom de la ville qui est associé à un contact.</span><span class="sxs-lookup"><span data-stu-id="97727-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="97727-124">State</span><span class="sxs-lookup"><span data-stu-id="97727-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="97727-125">Représente l’état de résidence pour un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="97727-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="97727-126">Countryorregion définit</span><span class="sxs-lookup"><span data-stu-id="97727-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="97727-127">Représente le pays ou la région pour l’adresse physique donnée.</span><span class="sxs-lookup"><span data-stu-id="97727-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|[<span data-ttu-id="97727-128">Code postal</span><span class="sxs-lookup"><span data-stu-id="97727-128">PostalCode</span></span>](postalcode.md) <br/> |<span data-ttu-id="97727-129">Représente le code postal pour un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="97727-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97727-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="97727-130">Parent elements</span></span>

|<span data-ttu-id="97727-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97727-131">**Element**</span></span>|<span data-ttu-id="97727-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="97727-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97727-133">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="97727-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="97727-134">Contient une collection d'adresses physiques associées à un contact.</span><span class="sxs-lookup"><span data-stu-id="97727-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97727-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="97727-135">Remarks</span></span>

<span data-ttu-id="97727-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="97727-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97727-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="97727-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97727-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="97727-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97727-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="97727-139">Schema Name</span></span>  <br/> |<span data-ttu-id="97727-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="97727-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="97727-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="97727-141">Validation File</span></span>  <br/> |<span data-ttu-id="97727-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97727-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97727-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="97727-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="97727-144">False</span><span class="sxs-lookup"><span data-stu-id="97727-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97727-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97727-145">See also</span></span>

- [<span data-ttu-id="97727-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97727-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="97727-147">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="97727-147">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="97727-148">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="97727-148">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="97727-149">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="97727-149">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

