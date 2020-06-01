---
title: PhysicalAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhysicalAddresses
api_type:
- schema
ms.assetid: 5276c5f2-9e08-43af-a0b2-da4ff1dcae2d
description: L’élément PhysicalAddresses contient une collection d’adresses physiques associées à un contact.
ms.openlocfilehash: b609abed481359fa6562f41a551645eb613ddfa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468879"
---
# <a name="physicaladdresses"></a><span data-ttu-id="7dec7-103">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="7dec7-103">PhysicalAddresses</span></span>

<span data-ttu-id="7dec7-104">L’élément **PhysicalAddresses** contient une collection d’adresses physiques associées à un contact.</span><span class="sxs-lookup"><span data-stu-id="7dec7-104">The **PhysicalAddresses** element contains a collection of physical addresses that are associated with a contact.</span></span> 
  
```xml
<PhysicalAddresses>
   <Entry/>
</PhysicalAddresses>
```

 <span data-ttu-id="7dec7-105">**PhysicalAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="7dec7-105">**PhysicalAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7dec7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7dec7-106">Attributes and elements</span></span>

<span data-ttu-id="7dec7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7dec7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7dec7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7dec7-108">Attributes</span></span>

<span data-ttu-id="7dec7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7dec7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7dec7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7dec7-110">Child elements</span></span>

|<span data-ttu-id="7dec7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7dec7-111">**Element**</span></span>|<span data-ttu-id="7dec7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7dec7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dec7-113">Entrée (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="7dec7-113">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="7dec7-114">Décrit une adresse physique unique pour un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="7dec7-114">Describes a single physical address for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7dec7-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7dec7-115">Parent elements</span></span>

|<span data-ttu-id="7dec7-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7dec7-116">**Element**</span></span>|<span data-ttu-id="7dec7-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7dec7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7dec7-118">Contact</span><span class="sxs-lookup"><span data-stu-id="7dec7-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="7dec7-119">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="7dec7-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7dec7-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7dec7-120">Remarks</span></span>

<span data-ttu-id="7dec7-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7dec7-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7dec7-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7dec7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7dec7-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7dec7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7dec7-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7dec7-124">Schema name</span></span>  <br/> |<span data-ttu-id="7dec7-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7dec7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7dec7-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7dec7-126">Validation file</span></span>  <br/> |<span data-ttu-id="7dec7-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7dec7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7dec7-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7dec7-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7dec7-129">False</span><span class="sxs-lookup"><span data-stu-id="7dec7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7dec7-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7dec7-130">See also</span></span>



- [<span data-ttu-id="7dec7-131">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7dec7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7dec7-132">Création de Contacts (Services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="7dec7-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[<span data-ttu-id="7dec7-133">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="7dec7-133">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="7dec7-134">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="7dec7-134">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

