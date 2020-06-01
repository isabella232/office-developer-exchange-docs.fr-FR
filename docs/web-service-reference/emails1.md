---
title: Emails1
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cc02bd86-c618-446a-92f0-749423cbc4ee
description: L’élément Emails1 spécifie un tableau de valeurs EmailAddressAttributedValue et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 916f87038cfe959045c93dba749f1dc3b85296e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456170"
---
# <a name="emails1"></a><span data-ttu-id="69e1d-103">Emails1</span><span class="sxs-lookup"><span data-stu-id="69e1d-103">Emails1</span></span>

<span data-ttu-id="69e1d-104">L’élément **Emails1** spécifie un tableau de valeurs **EmailAddressAttributedValue** et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="69e1d-104">The **Emails1** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails1>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails1>
```

 <span data-ttu-id="69e1d-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="69e1d-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69e1d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="69e1d-106">Attributes and elements</span></span>

<span data-ttu-id="69e1d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="69e1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69e1d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="69e1d-108">Attributes</span></span>

<span data-ttu-id="69e1d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="69e1d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69e1d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="69e1d-110">Child elements</span></span>

|<span data-ttu-id="69e1d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="69e1d-111">**Element**</span></span>|<span data-ttu-id="69e1d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="69e1d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69e1d-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="69e1d-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="69e1d-114">Spécifie une instance d’un tableau d’adresses de messagerie et les attributions associées.</span><span class="sxs-lookup"><span data-stu-id="69e1d-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69e1d-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="69e1d-115">Parent elements</span></span>

|<span data-ttu-id="69e1d-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="69e1d-116">**Element**</span></span>|<span data-ttu-id="69e1d-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="69e1d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69e1d-118">Persona</span><span class="sxs-lookup"><span data-stu-id="69e1d-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="69e1d-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="69e1d-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69e1d-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="69e1d-120">Remarks</span></span>

<span data-ttu-id="69e1d-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="69e1d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="69e1d-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="69e1d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69e1d-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="69e1d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69e1d-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="69e1d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69e1d-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="69e1d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="69e1d-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="69e1d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="69e1d-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="69e1d-127">Validation File</span></span>  <br/> |<span data-ttu-id="69e1d-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="69e1d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="69e1d-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="69e1d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="69e1d-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="69e1d-130">See also</span></span>



- [<span data-ttu-id="69e1d-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="69e1d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

