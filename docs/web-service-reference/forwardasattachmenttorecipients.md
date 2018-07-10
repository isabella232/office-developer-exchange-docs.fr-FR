---
title: ForwardAsAttachmentToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardAsAttachmentToRecipients
api_type:
- schema
ms.assetid: 8649ea14-672f-43c9-b10a-a2b02efd5867
description: L'élément ForwardAsAttachmentToRecipients indique les adresses de messagerie à laquelle les messages sont transmis en tant que pièces jointes.
ms.openlocfilehash: 04d4f9c6228e6d0ab34a6eff5d5751f461a57e19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756467"
---
# <a name="forwardasattachmenttorecipients"></a><span data-ttu-id="ae27b-103">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="ae27b-103">ForwardAsAttachmentToRecipients</span></span>

<span data-ttu-id="ae27b-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **ForwardAsAttachmentToRecipients** indique les adresses de messagerie à laquelle les messages sont transmis en tant que pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="ae27b-104">The **ForwardAsAttachmentToRecipients** element indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span> 
  
```XML
<ForwardAsAttachmentToRecipients>
   <Address/>
</ForwardAsAttachmentToRecipients>
```

 <span data-ttu-id="ae27b-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="ae27b-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae27b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ae27b-106">Attributes and elements</span></span>

<span data-ttu-id="ae27b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ae27b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae27b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ae27b-108">Attributes</span></span>

<span data-ttu-id="ae27b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ae27b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae27b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ae27b-110">Child elements</span></span>

|<span data-ttu-id="ae27b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae27b-111">**Element**</span></span>|<span data-ttu-id="ae27b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae27b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae27b-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ae27b-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="ae27b-114">Représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="ae27b-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae27b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ae27b-115">Parent elements</span></span>

|<span data-ttu-id="ae27b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae27b-116">**Element**</span></span>|<span data-ttu-id="ae27b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae27b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae27b-118">Actions</span><span class="sxs-lookup"><span data-stu-id="ae27b-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="ae27b-119">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="ae27b-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae27b-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ae27b-120">Text value</span></span>

<span data-ttu-id="ae27b-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ae27b-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae27b-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="ae27b-122">Remarks</span></span>

<span data-ttu-id="ae27b-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae27b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae27b-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ae27b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae27b-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ae27b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae27b-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ae27b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ae27b-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ae27b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ae27b-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ae27b-128">Validation File</span></span>  <br/> |<span data-ttu-id="ae27b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ae27b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae27b-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ae27b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae27b-131">True</span><span class="sxs-lookup"><span data-stu-id="ae27b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae27b-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ae27b-132">See also</span></span>



- [<span data-ttu-id="ae27b-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ae27b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
