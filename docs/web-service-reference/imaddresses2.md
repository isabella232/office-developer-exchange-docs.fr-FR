---
title: ImAddresses2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 328f29b9-3a9c-4d9a-a85f-5ffff84e266a
description: L’élément ImAddresses2 spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: b2a9f61ba31c1324ac5563bb6ab6b30f0271c653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460763"
---
# <a name="imaddresses2"></a><span data-ttu-id="3bdd9-103">ImAddresses2</span><span class="sxs-lookup"><span data-stu-id="3bdd9-103">ImAddresses2</span></span>

<span data-ttu-id="3bdd9-104">L’élément **ImAddresses2** spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="3bdd9-104">The **ImAddresses2** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses2>
    <StringAttributedValue/>
</ImAddresses2>
```

 <span data-ttu-id="3bdd9-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="3bdd9-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3bdd9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3bdd9-106">Attributes and elements</span></span>

<span data-ttu-id="3bdd9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3bdd9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3bdd9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3bdd9-108">Attributes</span></span>

<span data-ttu-id="3bdd9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3bdd9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3bdd9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3bdd9-110">Child elements</span></span>

|<span data-ttu-id="3bdd9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3bdd9-111">**Element**</span></span>|<span data-ttu-id="3bdd9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3bdd9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bdd9-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="3bdd9-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="3bdd9-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="3bdd9-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3bdd9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3bdd9-115">Parent elements</span></span>

|<span data-ttu-id="3bdd9-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3bdd9-116">**Element**</span></span>|<span data-ttu-id="3bdd9-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3bdd9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bdd9-118">Persona</span><span class="sxs-lookup"><span data-stu-id="3bdd9-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="3bdd9-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="3bdd9-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3bdd9-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="3bdd9-120">Remarks</span></span>

<span data-ttu-id="3bdd9-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3bdd9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3bdd9-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3bdd9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3bdd9-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3bdd9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3bdd9-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3bdd9-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3bdd9-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3bdd9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3bdd9-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="3bdd9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="3bdd9-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="3bdd9-127">Validation File</span></span>  <br/> |<span data-ttu-id="3bdd9-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="3bdd9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3bdd9-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3bdd9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3bdd9-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3bdd9-130">See also</span></span>



- [<span data-ttu-id="3bdd9-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3bdd9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

