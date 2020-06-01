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
ms.openlocfilehash: 159ae064827c2f9c2b470580ad5457264e8dae93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464048"
---
# <a name="fromconnectedaccounts"></a><span data-ttu-id="a573a-103">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="a573a-103">FromConnectedAccounts</span></span>

<span data-ttu-id="a573a-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **FromConnectedAccounts** représente les noms de compte de messagerie à partir de laquelle les messages entrants doivent ont été agrégées afin que l'exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="a573a-104">The **FromConnectedAccounts** element represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span> 
  
```XML
<FromConnectedAccounts>
    <String/>
</FromConnectedAccounts>
```

 <span data-ttu-id="a573a-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="a573a-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a573a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a573a-106">Attributes and elements</span></span>

<span data-ttu-id="a573a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a573a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a573a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a573a-108">Attributes</span></span>

<span data-ttu-id="a573a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a573a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a573a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a573a-110">Child elements</span></span>

|<span data-ttu-id="a573a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a573a-111">**Element**</span></span>|<span data-ttu-id="a573a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a573a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a573a-113">String</span><span class="sxs-lookup"><span data-stu-id="a573a-113">String</span></span>](string.md) <br/> |<span data-ttu-id="a573a-114">Représente un nom de compte de messagerie à partir de laquelle les messages entrants doivent ont été agrégées afin que l'exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="a573a-114">Represents an e-mail account name from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a573a-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a573a-115">Parent elements</span></span>

|<span data-ttu-id="a573a-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a573a-116">**Element**</span></span>|<span data-ttu-id="a573a-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a573a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a573a-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="a573a-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="a573a-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="a573a-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="a573a-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="a573a-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="a573a-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="a573a-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a573a-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a573a-122">Text value</span></span>

<span data-ttu-id="a573a-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a573a-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a573a-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="a573a-124">Remarks</span></span>

<span data-ttu-id="a573a-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a573a-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a573a-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a573a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a573a-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a573a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a573a-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a573a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a573a-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a573a-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a573a-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a573a-130">Validation File</span></span>  <br/> |<span data-ttu-id="a573a-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a573a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a573a-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a573a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a573a-133">True</span><span class="sxs-lookup"><span data-stu-id="a573a-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a573a-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a573a-134">See also</span></span>



- [<span data-ttu-id="a573a-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a573a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

