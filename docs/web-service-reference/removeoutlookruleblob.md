---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: L’élément RemoveOutlookRuleBlob indique s’il faut supprimer l’objet blob règle de Microsoft Outlook.
ms.openlocfilehash: 45336e296c39161704ce6e0d51fba1d2c61797b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829102"
---
# <a name="removeoutlookruleblob"></a><span data-ttu-id="36d3d-103">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="36d3d-103">RemoveOutlookRuleBlob</span></span>

<span data-ttu-id="36d3d-104">L’élément **RemoveOutlookRuleBlob** indique s’il faut supprimer l’objet blob règle de Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="36d3d-104">The **RemoveOutlookRuleBlob** element indicates whether to remove the Microsoft Outlook rule blob.</span></span> 
  
[<span data-ttu-id="36d3d-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="36d3d-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="36d3d-106">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="36d3d-106">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 <span data-ttu-id="36d3d-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="36d3d-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36d3d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="36d3d-108">Attributes and elements</span></span>

<span data-ttu-id="36d3d-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="36d3d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36d3d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="36d3d-110">Attributes</span></span>

<span data-ttu-id="36d3d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="36d3d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36d3d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="36d3d-112">Child elements</span></span>

<span data-ttu-id="36d3d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="36d3d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36d3d-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="36d3d-114">Parent elements</span></span>

|<span data-ttu-id="36d3d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36d3d-115">**Element**</span></span>|<span data-ttu-id="36d3d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="36d3d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36d3d-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="36d3d-117">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="36d3d-118">Définit une demande pour mettre à jour les règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="36d3d-118">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36d3d-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="36d3d-119">Text value</span></span>

<span data-ttu-id="36d3d-120">Une valeur de texte de **la valeur true** indique que le blob règle Outlook doit être supprimé.</span><span class="sxs-lookup"><span data-stu-id="36d3d-120">A text value of **true** indicates that the Outlook rule blob should be removed.</span></span> <span data-ttu-id="36d3d-121">Texte la valeur **false** indique que le blob règle Outlook ne doit pas être supprimé.</span><span class="sxs-lookup"><span data-stu-id="36d3d-121">A text value of **false** indicates that the Outlook rule blob should not be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="36d3d-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="36d3d-122">Remarks</span></span>

<span data-ttu-id="36d3d-123">Définissez cet élément à **la valeur true** pour permettre une mise à jour des règles de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="36d3d-123">Set this element to **true** to allow for an Inbox rule update.</span></span> 
  
<span data-ttu-id="36d3d-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="36d3d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36d3d-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="36d3d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36d3d-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="36d3d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36d3d-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="36d3d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="36d3d-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="36d3d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="36d3d-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="36d3d-129">Validation File</span></span>  <br/> |<span data-ttu-id="36d3d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="36d3d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36d3d-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="36d3d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="36d3d-132">True</span><span class="sxs-lookup"><span data-stu-id="36d3d-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36d3d-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="36d3d-133">See also</span></span>



[<span data-ttu-id="36d3d-134">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="36d3d-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="36d3d-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36d3d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

