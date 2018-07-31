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
description: L’élément OutOfOffice représente le message de réponse et un délai d’expiration pour l’envoi du message de réponse.
ms.openlocfilehash: f35b84d7a8a37c7a57b58c97fd0d37318bb50a33
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354266"
---
# <a name="outofoffice"></a><span data-ttu-id="a8da3-103">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="a8da3-103">OutOfOffice</span></span>

<span data-ttu-id="a8da3-104">L’élément **OutOfOffice** représente le message de réponse et un délai d’expiration pour l’envoi du message de réponse.</span><span class="sxs-lookup"><span data-stu-id="a8da3-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
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

<span data-ttu-id="a8da3-105">**OutOfOfficeMailTip**</span><span class="sxs-lookup"><span data-stu-id="a8da3-105">**OutOfOfficeMailTip**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a8da3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8da3-106">Attributes and elements</span></span>

<span data-ttu-id="a8da3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8da3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8da3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8da3-108">Attributes</span></span>

<span data-ttu-id="a8da3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8da3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8da3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8da3-110">Child elements</span></span>

|<span data-ttu-id="a8da3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8da3-111">**Element**</span></span>|<span data-ttu-id="a8da3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8da3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8da3-113">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="a8da3-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="a8da3-114">Contient un message d’absence du bureau (OOF) et la langue utilisée pour le message.</span><span class="sxs-lookup"><span data-stu-id="a8da3-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="a8da3-115">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="a8da3-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="a8da3-116">Contient la durée de l’état d’absence du bureau est activé si l’élément [OofState](oofstate.md) est défini sur planifiée.</span><span class="sxs-lookup"><span data-stu-id="a8da3-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8da3-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8da3-117">Parent elements</span></span>

|<span data-ttu-id="a8da3-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8da3-118">**Element**</span></span>|<span data-ttu-id="a8da3-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8da3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8da3-120">MailTips</span><span class="sxs-lookup"><span data-stu-id="a8da3-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="a8da3-121">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="a8da3-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8da3-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a8da3-122">Text value</span></span>

<span data-ttu-id="a8da3-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8da3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8da3-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8da3-124">Remarks</span></span>

<span data-ttu-id="a8da3-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8da3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8da3-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8da3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8da3-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8da3-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8da3-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8da3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a8da3-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a8da3-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8da3-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a8da3-130">Validation File</span></span>  <br/> |<span data-ttu-id="a8da3-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a8da3-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8da3-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8da3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8da3-133">False</span><span class="sxs-lookup"><span data-stu-id="a8da3-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8da3-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8da3-134">See also</span></span>

- [<span data-ttu-id="a8da3-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a8da3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

