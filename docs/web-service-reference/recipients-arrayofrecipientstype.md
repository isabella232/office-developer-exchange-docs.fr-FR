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
description: L’élément Recipients représente une collection de destinataires qui reçoivent une copie du message.
ms.openlocfilehash: 0e18152a8143b888ad27f48137c06613694f5713
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463873"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="42092-103">Destinataires (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="42092-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="42092-104">L’élément **Recipients** représente une collection de destinataires qui reçoivent une copie du message.</span><span class="sxs-lookup"><span data-stu-id="42092-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="42092-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="42092-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42092-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="42092-106">Attributes and elements</span></span>

<span data-ttu-id="42092-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="42092-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42092-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="42092-108">Attributes</span></span>

<span data-ttu-id="42092-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="42092-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42092-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="42092-110">Child elements</span></span>

|<span data-ttu-id="42092-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="42092-111">**Element**</span></span>|<span data-ttu-id="42092-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="42092-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42092-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="42092-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="42092-114">Identifie un objet Active Directory à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="42092-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="42092-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="42092-115">Parent elements</span></span>

|<span data-ttu-id="42092-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="42092-116">**Element**</span></span>|<span data-ttu-id="42092-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="42092-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42092-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="42092-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="42092-119">Contient les destinataires et les types de conseils de messagerie à récupérer.</span><span class="sxs-lookup"><span data-stu-id="42092-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="42092-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="42092-120">Text value</span></span>

<span data-ttu-id="42092-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="42092-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="42092-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="42092-122">Remarks</span></span>

<span data-ttu-id="42092-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="42092-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42092-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="42092-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42092-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="42092-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42092-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="42092-126">Schema Name</span></span>  <br/> |<span data-ttu-id="42092-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="42092-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="42092-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="42092-128">Validation File</span></span>  <br/> |<span data-ttu-id="42092-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="42092-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="42092-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="42092-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="42092-131">False</span><span class="sxs-lookup"><span data-stu-id="42092-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42092-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="42092-132">See also</span></span>



- [<span data-ttu-id="42092-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="42092-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

