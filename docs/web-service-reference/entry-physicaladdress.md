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
description: L’élément Entry décrit une adresse physique unique pour un élément de contact.
ms.openlocfilehash: 5e8343e9abebeeff8c2b81327b2e0f4ddcf45364
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459629"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="46d46-103">Entrée (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="46d46-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="46d46-104">L’élément **entry** décrit une adresse physique unique pour un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="46d46-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="46d46-105">**PhysicalAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="46d46-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46d46-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="46d46-106">Attributes and elements</span></span>

<span data-ttu-id="46d46-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="46d46-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46d46-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="46d46-108">Attributes</span></span>

|<span data-ttu-id="46d46-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="46d46-109">**Attribute**</span></span>|<span data-ttu-id="46d46-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="46d46-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46d46-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="46d46-111">**Key**</span></span> <br/> | <span data-ttu-id="46d46-112">Identifie une adresse physique.</span><span class="sxs-lookup"><span data-stu-id="46d46-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="46d46-113">Les valeurs possibles pour cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="46d46-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="46d46-114">-Business</span><span class="sxs-lookup"><span data-stu-id="46d46-114">-  Business</span></span>  <br/><span data-ttu-id="46d46-115">-Accueil</span><span class="sxs-lookup"><span data-stu-id="46d46-115">-  Home</span></span>  <br/><span data-ttu-id="46d46-116">-Autre</span><span class="sxs-lookup"><span data-stu-id="46d46-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="46d46-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="46d46-117">Child elements</span></span>

|<span data-ttu-id="46d46-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="46d46-118">**Element**</span></span>|<span data-ttu-id="46d46-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="46d46-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46d46-120">Street</span><span class="sxs-lookup"><span data-stu-id="46d46-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="46d46-121">Représente l’adresse d’un contact.</span><span class="sxs-lookup"><span data-stu-id="46d46-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="46d46-122">City</span><span class="sxs-lookup"><span data-stu-id="46d46-122">City</span></span>](city.md) <br/> |<span data-ttu-id="46d46-123">Représente le nom de la ville qui est associé à un contact.</span><span class="sxs-lookup"><span data-stu-id="46d46-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="46d46-124">State</span><span class="sxs-lookup"><span data-stu-id="46d46-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="46d46-125">Représente l’état de résidence d’un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="46d46-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="46d46-126">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="46d46-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="46d46-127">Représente le pays ou la région d’une adresse physique donnée.</span><span class="sxs-lookup"><span data-stu-id="46d46-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|[<span data-ttu-id="46d46-128">PostalCode</span><span class="sxs-lookup"><span data-stu-id="46d46-128">PostalCode</span></span>](postalcode.md) <br/> |<span data-ttu-id="46d46-129">Représente le code postal d’un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="46d46-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="46d46-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="46d46-130">Parent elements</span></span>

|<span data-ttu-id="46d46-131">**Élément**</span><span class="sxs-lookup"><span data-stu-id="46d46-131">**Element**</span></span>|<span data-ttu-id="46d46-132">**Description**</span><span class="sxs-lookup"><span data-stu-id="46d46-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46d46-133">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="46d46-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="46d46-134">Contient une collection d'adresses physiques associées à un contact.</span><span class="sxs-lookup"><span data-stu-id="46d46-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46d46-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="46d46-135">Remarks</span></span>

<span data-ttu-id="46d46-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="46d46-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46d46-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="46d46-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46d46-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="46d46-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46d46-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="46d46-139">Schema Name</span></span>  <br/> |<span data-ttu-id="46d46-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="46d46-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="46d46-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="46d46-141">Validation File</span></span>  <br/> |<span data-ttu-id="46d46-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46d46-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46d46-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="46d46-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="46d46-144">False</span><span class="sxs-lookup"><span data-stu-id="46d46-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46d46-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="46d46-145">See also</span></span>

- [<span data-ttu-id="46d46-146">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="46d46-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="46d46-147">Création de Contacts (Services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="46d46-147">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="46d46-148">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="46d46-148">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="46d46-149">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="46d46-149">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

