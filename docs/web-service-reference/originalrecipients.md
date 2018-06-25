---
title: OriginalRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalRecipients
api_type:
- schema
ms.assetid: e4af86a5-85af-4239-8055-e29f0acf77c1
description: L'élément OriginalRecipients représente une liste d'adresses de messagerie des destinataires du message de premier.
ms.openlocfilehash: 8f99368409dbfb5ac798b691be65c7fd64f32660
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828665"
---
# <a name="originalrecipients"></a><span data-ttu-id="43998-103">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="43998-103">OriginalRecipients</span></span>

<span data-ttu-id="43998-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **OriginalRecipients** représente une liste d'adresses de messagerie des destinataires du message de premier.</span><span class="sxs-lookup"><span data-stu-id="43998-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="43998-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="43998-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43998-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="43998-106">Attributes and elements</span></span>

<span data-ttu-id="43998-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="43998-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43998-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="43998-108">Attributes</span></span>

<span data-ttu-id="43998-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="43998-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43998-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="43998-110">Child elements</span></span>

|<span data-ttu-id="43998-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="43998-111">**Element**</span></span>|<span data-ttu-id="43998-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="43998-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43998-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="43998-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="43998-114">Contient une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="43998-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="43998-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="43998-115">Parent elements</span></span>

|<span data-ttu-id="43998-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="43998-116">**Element**</span></span>|<span data-ttu-id="43998-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="43998-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43998-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="43998-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="43998-119">Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="43998-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="43998-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="43998-120">Remarks</span></span>

<span data-ttu-id="43998-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="43998-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43998-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="43998-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43998-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="43998-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43998-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="43998-124">Schema Name</span></span>  <br/> |<span data-ttu-id="43998-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="43998-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="43998-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="43998-126">Validation File</span></span>  <br/> |<span data-ttu-id="43998-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43998-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43998-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="43998-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="43998-129">False</span><span class="sxs-lookup"><span data-stu-id="43998-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43998-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="43998-130">See also</span></span>



[<span data-ttu-id="43998-131">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="43998-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="43998-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="43998-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

