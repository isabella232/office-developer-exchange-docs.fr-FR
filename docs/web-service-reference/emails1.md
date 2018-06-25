---
title: Emails1
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cc02bd86-c618-446a-92f0-749423cbc4ee
description: L’élément Emails1 spécifie un tableau de valeurs EmailAddressAttributedValue et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: f1a1223244c91731b1a5a1beb9daed6d680d3bc4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756122"
---
# <a name="emails1"></a><span data-ttu-id="9082c-103">Emails1</span><span class="sxs-lookup"><span data-stu-id="9082c-103">Emails1</span></span>

<span data-ttu-id="9082c-104">L’élément **Emails1** spécifie un tableau de valeurs **EmailAddressAttributedValue** et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="9082c-104">The **Emails1** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails1>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails1>
```

 <span data-ttu-id="9082c-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9082c-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9082c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9082c-106">Attributes and elements</span></span>

<span data-ttu-id="9082c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9082c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9082c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9082c-108">Attributes</span></span>

<span data-ttu-id="9082c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9082c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9082c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9082c-110">Child elements</span></span>

|<span data-ttu-id="9082c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9082c-111">**Element**</span></span>|<span data-ttu-id="9082c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9082c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9082c-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9082c-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="9082c-114">Spécifie une instance d’un tableau d’adresses de messagerie et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="9082c-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9082c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9082c-115">Parent elements</span></span>

|<span data-ttu-id="9082c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9082c-116">**Element**</span></span>|<span data-ttu-id="9082c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="9082c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9082c-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="9082c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9082c-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="9082c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9082c-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9082c-120">Remarks</span></span>

<span data-ttu-id="9082c-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9082c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9082c-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9082c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9082c-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9082c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9082c-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9082c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9082c-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9082c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9082c-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="9082c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9082c-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="9082c-127">Validation File</span></span>  <br/> |<span data-ttu-id="9082c-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9082c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9082c-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9082c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9082c-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9082c-130">See also</span></span>



- [<span data-ttu-id="9082c-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9082c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

