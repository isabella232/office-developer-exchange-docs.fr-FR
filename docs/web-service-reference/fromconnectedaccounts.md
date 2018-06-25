---
title: FromConnectedAccounts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FromConnectedAccounts
api_type:
- schema
ms.assetid: d4d7ddd7-078d-4f1a-a26b-22dce0c49f3a
description: L'élément FromConnectedAccounts représente les noms de compte de messagerie à partir de laquelle les messages entrants doivent ont été agrégées afin que l'exception ou la condition à appliquer.
ms.openlocfilehash: 426e81bbbe96fb5fb4b36506438dc4af4f560eef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756488"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="c572f-103">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="c572f-103">FromConnectedAccounts</span></span>

<span data-ttu-id="c572f-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **FromConnectedAccounts** représente les noms de compte de messagerie à partir de laquelle les messages entrants doivent ont été agrégées afin que l'exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="c572f-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="c572f-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="c572f-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c572f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c572f-106">Attributes and elements</span></span>

<span data-ttu-id="c572f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c572f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c572f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c572f-108">Attributes</span></span>

<span data-ttu-id="c572f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c572f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c572f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c572f-110">Child elements</span></span>

|<span data-ttu-id="c572f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c572f-111">**Element**</span></span>|<span data-ttu-id="c572f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c572f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c572f-113">String</span><span class="sxs-lookup"><span data-stu-id="c572f-113">String</span></span>](string.md) <br/> |<span data-ttu-id="c572f-114">Représente un nom de compte de messagerie à partir de laquelle les messages entrants doivent ont été agrégées afin que l'exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="c572f-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c572f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c572f-115">Parent elements</span></span>

|<span data-ttu-id="c572f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c572f-116">**Element**</span></span>|<span data-ttu-id="c572f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c572f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c572f-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="c572f-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="c572f-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="c572f-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="c572f-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="c572f-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="c572f-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="c572f-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c572f-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c572f-122">Text value</span></span>

<span data-ttu-id="c572f-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c572f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c572f-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="c572f-124">Remarks</span></span>

<span data-ttu-id="c572f-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c572f-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c572f-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c572f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c572f-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c572f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c572f-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c572f-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c572f-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c572f-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c572f-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c572f-130">Validation File</span></span>  <br/> |<span data-ttu-id="c572f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c572f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c572f-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c572f-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c572f-133">True</span><span class="sxs-lookup"><span data-stu-id="c572f-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c572f-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c572f-134">See also</span></span>



- [<span data-ttu-id="c572f-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c572f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

