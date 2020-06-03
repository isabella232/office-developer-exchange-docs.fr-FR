---
title: Imaddresss (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b95d0a8b-15a6-4711-b014-55698dbd679c
description: L’élément imaddresss spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 6714af5d88e50047f48da2f10dbb33d2e2feb724
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460441"
---
# <a name="imaddresses-arrayofstringattributedvaluestype"></a><span data-ttu-id="7b803-103">Imaddresss (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="7b803-103">ImAddresses (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="7b803-104">L’élément **Imaddresss** spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="7b803-104">The **ImAddresses** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses>
    <StringAttributedValue/>
</ImAddresses>
```

 <span data-ttu-id="7b803-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="7b803-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b803-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b803-106">Attributes and elements</span></span>

<span data-ttu-id="7b803-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b803-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b803-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b803-108">Attributes</span></span>

<span data-ttu-id="7b803-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b803-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b803-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b803-110">Child elements</span></span>

|<span data-ttu-id="7b803-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b803-111">**Element**</span></span>|<span data-ttu-id="7b803-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b803-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b803-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="7b803-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="7b803-114">Spécifie une instance dans un tableau d’attributs associés à un élément Persona.</span><span class="sxs-lookup"><span data-stu-id="7b803-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b803-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b803-115">Parent elements</span></span>

|<span data-ttu-id="7b803-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b803-116">**Element**</span></span>|<span data-ttu-id="7b803-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b803-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b803-118">Persona</span><span class="sxs-lookup"><span data-stu-id="7b803-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="7b803-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="7b803-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7b803-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b803-120">Remarks</span></span>

<span data-ttu-id="7b803-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7b803-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7b803-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b803-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b803-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b803-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b803-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b803-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b803-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b803-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7b803-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="7b803-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="7b803-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="7b803-127">Validation File</span></span>  <br/> |<span data-ttu-id="7b803-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="7b803-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b803-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b803-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7b803-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b803-130">See also</span></span>



- [<span data-ttu-id="7b803-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7b803-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

