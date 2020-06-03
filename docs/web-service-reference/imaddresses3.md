---
title: ImAddresses3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cab51a28-dfad-4c70-aafe-e239321b784e
description: L’élément ImAddresses3 spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 2f02a57b1a113abe39a2852f8f8dbbd2b5b803ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460749"
---
# <a name="imaddresses3"></a><span data-ttu-id="ff1b8-103">ImAddresses3</span><span class="sxs-lookup"><span data-stu-id="ff1b8-103">ImAddresses3</span></span>

<span data-ttu-id="ff1b8-104">L’élément **ImAddresses3** spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="ff1b8-104">The **ImAddresses3** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses3>
    <StringAttributedValue/>
</ImAddresses3>
```

 <span data-ttu-id="ff1b8-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="ff1b8-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff1b8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ff1b8-106">Attributes and elements</span></span>

<span data-ttu-id="ff1b8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ff1b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff1b8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ff1b8-108">Attributes</span></span>

<span data-ttu-id="ff1b8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ff1b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff1b8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ff1b8-110">Child elements</span></span>

|<span data-ttu-id="ff1b8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ff1b8-111">**Element**</span></span>|<span data-ttu-id="ff1b8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff1b8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff1b8-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="ff1b8-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="ff1b8-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="ff1b8-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff1b8-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ff1b8-115">Parent elements</span></span>

|<span data-ttu-id="ff1b8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ff1b8-116">**Element**</span></span>|<span data-ttu-id="ff1b8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff1b8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff1b8-118">Persona</span><span class="sxs-lookup"><span data-stu-id="ff1b8-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ff1b8-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="ff1b8-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ff1b8-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ff1b8-120">Remarks</span></span>

<span data-ttu-id="ff1b8-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ff1b8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ff1b8-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff1b8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff1b8-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ff1b8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff1b8-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ff1b8-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff1b8-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ff1b8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ff1b8-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="ff1b8-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ff1b8-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="ff1b8-127">Validation File</span></span>  <br/> |<span data-ttu-id="ff1b8-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="ff1b8-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff1b8-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ff1b8-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ff1b8-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff1b8-130">See also</span></span>



- [<span data-ttu-id="ff1b8-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ff1b8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

