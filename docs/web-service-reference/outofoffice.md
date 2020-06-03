---
title: OutOfOffice
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: L’élément OutOfOffice représente le message de réponse et la durée d’envoi du message de réponse.
ms.openlocfilehash: 082a81b62e2b783b302b3e749e0066131a46d73e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456898"
---
# <a name="outofoffice"></a><span data-ttu-id="e70d5-103">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="e70d5-103">OutOfOffice</span></span>

<span data-ttu-id="e70d5-104">L’élément **OutOfOffice** représente le message de réponse et la durée d’envoi du message de réponse.</span><span class="sxs-lookup"><span data-stu-id="e70d5-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

```XML
<OutOfOffice>
   <ReplyBody/>
</OutOfOffice>
```

<span data-ttu-id="e70d5-105">**OutOfOfficeMailTip**</span><span class="sxs-lookup"><span data-stu-id="e70d5-105">**OutOfOfficeMailTip**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e70d5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e70d5-106">Attributes and elements</span></span>

<span data-ttu-id="e70d5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e70d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e70d5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e70d5-108">Attributes</span></span>

<span data-ttu-id="e70d5-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e70d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e70d5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e70d5-110">Child elements</span></span>

|<span data-ttu-id="e70d5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e70d5-111">**Element**</span></span>|<span data-ttu-id="e70d5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e70d5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e70d5-113">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="e70d5-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="e70d5-114">Contient un message d’absence du bureau et la langue utilisée pour le message.</span><span class="sxs-lookup"><span data-stu-id="e70d5-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="e70d5-115">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="e70d5-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="e70d5-116">Contient la durée pendant laquelle le statut OOF est activé si l’élément [OofState](oofstate.md) est défini sur planifié.</span><span class="sxs-lookup"><span data-stu-id="e70d5-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e70d5-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e70d5-117">Parent elements</span></span>

|<span data-ttu-id="e70d5-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e70d5-118">**Element**</span></span>|<span data-ttu-id="e70d5-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="e70d5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e70d5-120">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="e70d5-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="e70d5-121">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="e70d5-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e70d5-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e70d5-122">Text value</span></span>

<span data-ttu-id="e70d5-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e70d5-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e70d5-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="e70d5-124">Remarks</span></span>

<span data-ttu-id="e70d5-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e70d5-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e70d5-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e70d5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e70d5-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e70d5-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e70d5-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e70d5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e70d5-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e70d5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="e70d5-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e70d5-130">Validation File</span></span>  <br/> |<span data-ttu-id="e70d5-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e70d5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e70d5-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e70d5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e70d5-133">False</span><span class="sxs-lookup"><span data-stu-id="e70d5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e70d5-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e70d5-134">See also</span></span>

- [<span data-ttu-id="e70d5-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e70d5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

