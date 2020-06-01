---
title: IsVoicemail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsVoicemail
api_type:
- schema
ms.assetid: 96d81d6e-4b75-43ad-b151-2dd4fd57db94
description: L'élément IsVoicemail indique si les messages entrants doivent être des messages vocaux afin que l'exception ou la condition à appliquer.
ms.openlocfilehash: 8c60513a54cbf2398fde4b71ab1fbcf8a5efb608
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458137"
---
# <a name="isvoicemail"></a><span data-ttu-id="15486-103">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="15486-103">IsVoicemail</span></span>

<span data-ttu-id="15486-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **IsVoicemail** indique si les messages entrants doivent être des messages vocaux afin que l'exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="15486-104">The **IsVoicemail** element indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span> 
  
```XML
<IsVoicemail>true | false</IsVoicemail>
```

 <span data-ttu-id="15486-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="15486-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15486-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="15486-106">Attributes and elements</span></span>

<span data-ttu-id="15486-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="15486-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15486-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="15486-108">Attributes</span></span>

<span data-ttu-id="15486-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="15486-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15486-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="15486-110">Child elements</span></span>

<span data-ttu-id="15486-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15486-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15486-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="15486-112">Parent elements</span></span>

|<span data-ttu-id="15486-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="15486-113">**Element**</span></span>|<span data-ttu-id="15486-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="15486-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15486-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="15486-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="15486-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="15486-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="15486-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="15486-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="15486-118">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="15486-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15486-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="15486-119">Text value</span></span>

<span data-ttu-id="15486-p101">Une valeur texte **true** indique que le message doit être un message vocal afin que l'exception ou la condition à appliquer. La valeur **false** indique que le message ne doit pas être un message vocal afin que l'exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="15486-p101">A text value of **true** indicates that the message must be a voice mail message in order for the condition or exception to apply. A value of **false** indicates that the message must not be a voice mail message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="15486-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="15486-122">Remarks</span></span>

<span data-ttu-id="15486-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="15486-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15486-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="15486-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15486-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="15486-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="15486-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="15486-126">Schema Name</span></span>  <br/> |<span data-ttu-id="15486-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="15486-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="15486-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="15486-128">Validation File</span></span>  <br/> |<span data-ttu-id="15486-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="15486-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15486-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="15486-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="15486-131">True</span><span class="sxs-lookup"><span data-stu-id="15486-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15486-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15486-132">See also</span></span>



- [<span data-ttu-id="15486-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15486-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

