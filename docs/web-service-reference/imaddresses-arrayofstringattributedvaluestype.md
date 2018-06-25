---
title: ImAddresses (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b95d0a8b-15a6-4711-b014-55698dbd679c
description: L’élément ImAddresses spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 6f238e26083366320ba04b187e3e41771cbd14ba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827863"
---
# <a name="imaddresses-arrayofstringattributedvaluestype"></a><span data-ttu-id="f81e0-103">ImAddresses (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="f81e0-103">ImAddresses (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="f81e0-104">L’élément **ImAddresses** spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="f81e0-104">The **ImAddresses** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses>
    <StringAttributedValue/>
</ImAddresses>
```

 <span data-ttu-id="f81e0-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="f81e0-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f81e0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f81e0-106">Attributes and elements</span></span>

<span data-ttu-id="f81e0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f81e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f81e0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f81e0-108">Attributes</span></span>

<span data-ttu-id="f81e0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f81e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f81e0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f81e0-110">Child elements</span></span>

|<span data-ttu-id="f81e0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f81e0-111">**Element**</span></span>|<span data-ttu-id="f81e0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f81e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f81e0-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="f81e0-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="f81e0-114">Spécifie une instance d’un tableau d’attributs associés à un élément personnage.</span><span class="sxs-lookup"><span data-stu-id="f81e0-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f81e0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f81e0-115">Parent elements</span></span>

|<span data-ttu-id="f81e0-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f81e0-116">**Element**</span></span>|<span data-ttu-id="f81e0-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f81e0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f81e0-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="f81e0-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f81e0-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="f81e0-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f81e0-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="f81e0-120">Remarks</span></span>

<span data-ttu-id="f81e0-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f81e0-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f81e0-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f81e0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f81e0-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f81e0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f81e0-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f81e0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f81e0-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f81e0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f81e0-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="f81e0-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f81e0-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="f81e0-127">Validation File</span></span>  <br/> |<span data-ttu-id="f81e0-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="f81e0-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f81e0-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f81e0-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f81e0-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f81e0-130">See also</span></span>



- [<span data-ttu-id="f81e0-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f81e0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

