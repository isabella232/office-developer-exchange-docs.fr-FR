---
title: Emails3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f4dc589-4530-4a35-b2a6-0c83cac23637
description: L’élément Emails3 spécifie un tableau de valeurs EmailAddressAttributedValue et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 1d174000d59883446bb7f61af90278d197ef5ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756126"
---
# <a name="emails3"></a><span data-ttu-id="d2271-103">Emails3</span><span class="sxs-lookup"><span data-stu-id="d2271-103">Emails3</span></span>

<span data-ttu-id="d2271-104">L’élément **Emails3** spécifie un tableau de valeurs **EmailAddressAttributedValue** et les identificateurs de leurs attributions source pour le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="d2271-104">The **Emails3** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails3>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails3>
```

 <span data-ttu-id="d2271-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="d2271-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2271-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d2271-106">Attributes and elements</span></span>

<span data-ttu-id="d2271-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d2271-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2271-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d2271-108">Attributes</span></span>

<span data-ttu-id="d2271-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d2271-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2271-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d2271-110">Child elements</span></span>

|<span data-ttu-id="d2271-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2271-111">**Element**</span></span>|<span data-ttu-id="d2271-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2271-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2271-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d2271-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="d2271-114">Spécifie une instance d’un tableau d’adresses de messagerie et leurs attributions associées.</span><span class="sxs-lookup"><span data-stu-id="d2271-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2271-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d2271-115">Parent elements</span></span>

|<span data-ttu-id="d2271-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2271-116">**Element**</span></span>|<span data-ttu-id="d2271-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2271-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2271-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="d2271-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="d2271-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="d2271-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2271-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d2271-120">Remarks</span></span>

<span data-ttu-id="d2271-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d2271-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2271-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2271-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2271-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d2271-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2271-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d2271-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2271-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d2271-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d2271-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d2271-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d2271-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="d2271-127">Validation File</span></span>  <br/> |<span data-ttu-id="d2271-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2271-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2271-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d2271-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d2271-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2271-130">See also</span></span>



- [<span data-ttu-id="d2271-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2271-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

