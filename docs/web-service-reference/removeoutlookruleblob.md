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
description: L’élément RemoveOutlookRuleBlob indique s’il faut supprimer le blob de règle Microsoft Outlook.
ms.openlocfilehash: b4202ab52bf16d1ad1546ec963cd8b9dacd2bd63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467668"
---
# <a name="removeoutlookruleblob"></a><span data-ttu-id="e0102-103">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="e0102-103">RemoveOutlookRuleBlob</span></span>

<span data-ttu-id="e0102-104">L’élément **RemoveOutlookRuleBlob** indique s’il faut supprimer le blob de règle Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="e0102-104">The **RemoveOutlookRuleBlob** element indicates whether to remove the Microsoft Outlook rule blob.</span></span> 
  
[<span data-ttu-id="e0102-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="e0102-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="e0102-106">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="e0102-106">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 <span data-ttu-id="e0102-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e0102-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0102-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e0102-108">Attributes and elements</span></span>

<span data-ttu-id="e0102-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e0102-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0102-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="e0102-110">Attributes</span></span>

<span data-ttu-id="e0102-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e0102-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0102-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e0102-112">Child elements</span></span>

<span data-ttu-id="e0102-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e0102-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0102-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e0102-114">Parent elements</span></span>

|<span data-ttu-id="e0102-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e0102-115">**Element**</span></span>|<span data-ttu-id="e0102-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="e0102-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0102-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="e0102-117">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="e0102-118">Définit une demande de mise à jour des règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="e0102-118">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e0102-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="e0102-119">Text value</span></span>

<span data-ttu-id="e0102-120">Une valeur de texte **true** indique que l’objet blob de la règle Outlook doit être supprimé.</span><span class="sxs-lookup"><span data-stu-id="e0102-120">A text value of **true** indicates that the Outlook rule blob should be removed.</span></span> <span data-ttu-id="e0102-121">Une valeur de texte **false** indique que l’objet blob de la règle Outlook ne doit pas être supprimé.</span><span class="sxs-lookup"><span data-stu-id="e0102-121">A text value of **false** indicates that the Outlook rule blob should not be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e0102-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="e0102-122">Remarks</span></span>

<span data-ttu-id="e0102-123">Définissez cet élément sur **true** pour autoriser la mise à jour des règles de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="e0102-123">Set this element to **true** to allow for an Inbox rule update.</span></span> 
  
<span data-ttu-id="e0102-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0102-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0102-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e0102-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0102-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e0102-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0102-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e0102-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e0102-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e0102-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0102-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e0102-129">Validation File</span></span>  <br/> |<span data-ttu-id="e0102-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e0102-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0102-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e0102-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0102-132">True</span><span class="sxs-lookup"><span data-stu-id="e0102-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0102-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e0102-133">See also</span></span>



[<span data-ttu-id="e0102-134">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="e0102-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="e0102-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e0102-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

