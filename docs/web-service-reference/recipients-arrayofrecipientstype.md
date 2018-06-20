---
title: Destinataires (ArrayOfRecipientsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: f4b71403-cbae-4176-8b2e-3597048c057b
description: L’élément destinataires représente une collection de destinataires qui reçoivent une copie du message.
ms.openlocfilehash: b24a029bfacd6cc40e85a201b8ca90efd7790e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828991"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="b8fb7-103">Destinataires (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="b8fb7-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="b8fb7-104">L’élément **destinataires** représente une collection de destinataires qui reçoivent une copie du message.</span><span class="sxs-lookup"><span data-stu-id="b8fb7-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="b8fb7-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="b8fb7-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8fb7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b8fb7-106">Attributes and elements</span></span>

<span data-ttu-id="b8fb7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b8fb7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8fb7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b8fb7-108">Attributes</span></span>

<span data-ttu-id="b8fb7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b8fb7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8fb7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b8fb7-110">Child elements</span></span>

|<span data-ttu-id="b8fb7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b8fb7-111">**Element**</span></span>|<span data-ttu-id="b8fb7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b8fb7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8fb7-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="b8fb7-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b8fb7-114">Identifie un objet Active Directory à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="b8fb7-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8fb7-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b8fb7-115">Parent elements</span></span>

|<span data-ttu-id="b8fb7-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b8fb7-116">**Element**</span></span>|<span data-ttu-id="b8fb7-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b8fb7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8fb7-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="b8fb7-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="b8fb7-119">Contient les destinataires et les types de conseils de messagerie à récupérer.</span><span class="sxs-lookup"><span data-stu-id="b8fb7-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8fb7-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b8fb7-120">Text value</span></span>

<span data-ttu-id="b8fb7-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b8fb7-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b8fb7-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="b8fb7-122">Remarks</span></span>

<span data-ttu-id="b8fb7-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8fb7-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8fb7-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b8fb7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8fb7-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b8fb7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8fb7-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b8fb7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b8fb7-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b8fb7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b8fb7-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b8fb7-128">Validation File</span></span>  <br/> |<span data-ttu-id="b8fb7-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b8fb7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8fb7-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b8fb7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8fb7-131">False</span><span class="sxs-lookup"><span data-stu-id="b8fb7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8fb7-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b8fb7-132">See also</span></span>



- [<span data-ttu-id="b8fb7-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b8fb7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
