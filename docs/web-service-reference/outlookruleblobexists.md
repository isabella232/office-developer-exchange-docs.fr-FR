---
title: OutlookRuleBlobExists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutlookRuleBlobExists
api_type:
- schema
ms.assetid: ae1bc448-deb9-4b5b-ab38-4b276abcb650
description: L’élément OutlookRuleBlobExists indique si un objet blob règle de Microsoft Outlook existe dans la boîte aux lettres de l’utilisateur.
ms.openlocfilehash: a738377cd3c1d69b90ac39ca479b03b3220d5bc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828679"
---
# <a name="outlookruleblobexists"></a><span data-ttu-id="27644-103">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="27644-103">OutlookRuleBlobExists</span></span>

<span data-ttu-id="27644-104">L’élément **OutlookRuleBlobExists** indique si un objet blob règle de Microsoft Outlook existe dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="27644-104">The **OutlookRuleBlobExists** element indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span> 
  
[<span data-ttu-id="27644-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="27644-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="27644-106">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="27644-106">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
```

 <span data-ttu-id="27644-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="27644-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27644-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="27644-108">Attributes and elements</span></span>

<span data-ttu-id="27644-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="27644-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27644-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="27644-110">Attributes</span></span>

<span data-ttu-id="27644-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="27644-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27644-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="27644-112">Child elements</span></span>

<span data-ttu-id="27644-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="27644-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27644-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="27644-114">Parent elements</span></span>

|<span data-ttu-id="27644-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="27644-115">**Element**</span></span>|<span data-ttu-id="27644-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="27644-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27644-117">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="27644-117">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="27644-118">Représente une réponse à une demande [d’opération GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="27644-118">Represents a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27644-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="27644-119">Text value</span></span>

<span data-ttu-id="27644-120">Une valeur de texte de **la valeur true** indique qu’un blob de règle Outlook existe.</span><span class="sxs-lookup"><span data-stu-id="27644-120">A text value of **true** indicates that an Outlook rule blob exists.</span></span> <span data-ttu-id="27644-121">Texte la valeur **false** indique qu’un blob de règle Outlook n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="27644-121">A text value of **false** indicates that an Outlook rule blob does not exist.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="27644-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="27644-122">Remarks</span></span>

<span data-ttu-id="27644-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="27644-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27644-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="27644-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27644-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="27644-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27644-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="27644-126">Schema Name</span></span>  <br/> |<span data-ttu-id="27644-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="27644-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27644-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="27644-128">Validation File</span></span>  <br/> |<span data-ttu-id="27644-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27644-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27644-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="27644-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="27644-131">True</span><span class="sxs-lookup"><span data-stu-id="27644-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27644-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="27644-132">See also</span></span>



- [<span data-ttu-id="27644-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="27644-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

