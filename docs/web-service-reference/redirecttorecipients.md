---
title: RedirectToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RedirectToRecipients
api_type:
- schema
ms.assetid: 00ef4a84-76d2-4669-b597-f52abbbc34f5
description: L'élément RedirectToRecipients indique les adresses de messagerie à laquelle les messages doivent être redirigé.
ms.openlocfilehash: ca0422f2ca678cabe1a88f99e617bee691f2e2f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829024"
---
# <a name="redirecttorecipients"></a><span data-ttu-id="f96c2-103">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="f96c2-103">RedirectToRecipients</span></span>

<span data-ttu-id="f96c2-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **RedirectToRecipients** indique les adresses de messagerie à laquelle les messages doivent être redirigé.</span><span class="sxs-lookup"><span data-stu-id="f96c2-104">The **RedirectToRecipients** element indicates the e-mail addresses to which messages are to be redirected.</span></span> 
  
```XML
<RedirectToRecipients>
   <Address/>
</RedirectToRecipients>
```

 <span data-ttu-id="f96c2-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="f96c2-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f96c2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f96c2-106">Attributes and elements</span></span>

<span data-ttu-id="f96c2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f96c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f96c2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f96c2-108">Attributes</span></span>

<span data-ttu-id="f96c2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f96c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f96c2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f96c2-110">Child elements</span></span>

|<span data-ttu-id="f96c2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f96c2-111">**Element**</span></span>|<span data-ttu-id="f96c2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f96c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f96c2-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f96c2-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="f96c2-114">Représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="f96c2-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f96c2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f96c2-115">Parent elements</span></span>

|<span data-ttu-id="f96c2-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f96c2-116">**Element**</span></span>|<span data-ttu-id="f96c2-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f96c2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f96c2-118">Actions</span><span class="sxs-lookup"><span data-stu-id="f96c2-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="f96c2-119">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="f96c2-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f96c2-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f96c2-120">Text value</span></span>

<span data-ttu-id="f96c2-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f96c2-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f96c2-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="f96c2-122">Remarks</span></span>

<span data-ttu-id="f96c2-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f96c2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f96c2-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f96c2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f96c2-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f96c2-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f96c2-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f96c2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f96c2-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f96c2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f96c2-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f96c2-128">Validation File</span></span>  <br/> |<span data-ttu-id="f96c2-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f96c2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f96c2-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f96c2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f96c2-131">True</span><span class="sxs-lookup"><span data-stu-id="f96c2-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f96c2-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f96c2-132">See also</span></span>



- [<span data-ttu-id="f96c2-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f96c2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

