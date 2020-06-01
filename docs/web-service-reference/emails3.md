---
title: Emails3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f4dc589-4530-4a35-b2a6-0c83cac23637
description: L’élément Emails3 spécifie un tableau de valeurs EmailAddressAttributedValue et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: 0505b0ea248a3ab2de7ec18a344fa57651f84cca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460721"
---
# <a name="emails3"></a><span data-ttu-id="fc794-103">Emails3</span><span class="sxs-lookup"><span data-stu-id="fc794-103">Emails3</span></span>

<span data-ttu-id="fc794-104">L’élément **Emails3** spécifie un tableau de valeurs **EmailAddressAttributedValue** et les identificateurs de leurs attributions sources pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="fc794-104">The **Emails3** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails3>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails3>
```

 <span data-ttu-id="fc794-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="fc794-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc794-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fc794-106">Attributes and elements</span></span>

<span data-ttu-id="fc794-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fc794-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc794-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fc794-108">Attributes</span></span>

<span data-ttu-id="fc794-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fc794-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc794-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fc794-110">Child elements</span></span>

|<span data-ttu-id="fc794-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc794-111">**Element**</span></span>|<span data-ttu-id="fc794-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc794-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc794-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="fc794-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="fc794-114">Spécifie une instance d’un tableau d’adresses de messagerie et les attributions associées.</span><span class="sxs-lookup"><span data-stu-id="fc794-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc794-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fc794-115">Parent elements</span></span>

|<span data-ttu-id="fc794-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc794-116">**Element**</span></span>|<span data-ttu-id="fc794-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc794-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc794-118">Persona</span><span class="sxs-lookup"><span data-stu-id="fc794-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="fc794-119">Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="fc794-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc794-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="fc794-120">Remarks</span></span>

<span data-ttu-id="fc794-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fc794-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fc794-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc794-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc794-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fc794-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc794-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fc794-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc794-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fc794-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fc794-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="fc794-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="fc794-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="fc794-127">Validation File</span></span>  <br/> |<span data-ttu-id="fc794-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="fc794-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc794-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fc794-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fc794-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fc794-130">See also</span></span>



- [<span data-ttu-id="fc794-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fc794-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

