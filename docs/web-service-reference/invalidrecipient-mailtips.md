---
title: InvalidRecipient (Infos-courrier)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: L’élément InvalidRecipient indique si le destinataire n’est pas valide.
ms.openlocfilehash: addb86ece2be3091ac55a52ee2f16f5c5f72ae41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827958"
---
# <a name="invalidrecipient-mailtips"></a><span data-ttu-id="e6ce7-103">InvalidRecipient (Infos-courrier)</span><span class="sxs-lookup"><span data-stu-id="e6ce7-103">InvalidRecipient (MailTips)</span></span>

<span data-ttu-id="e6ce7-104">L’élément **InvalidRecipient** indique si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-104">The **InvalidRecipient** element indicates whether the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
```

 <span data-ttu-id="e6ce7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e6ce7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6ce7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e6ce7-106">Attributes and elements</span></span>

<span data-ttu-id="e6ce7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6ce7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e6ce7-108">Attributes</span></span>

<span data-ttu-id="e6ce7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6ce7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e6ce7-110">Child elements</span></span>

<span data-ttu-id="e6ce7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e6ce7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e6ce7-112">Parent elements</span></span>

|<span data-ttu-id="e6ce7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e6ce7-113">**Element**</span></span>|<span data-ttu-id="e6ce7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e6ce7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6ce7-115">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="e6ce7-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="e6ce7-116">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e6ce7-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e6ce7-117">Text value</span></span>

<span data-ttu-id="e6ce7-118">La valeur de texte de cet élément est **la valeur true** si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-118">The text value of this element is **true** if the recipient is invalid.</span></span> <span data-ttu-id="e6ce7-119">La valeur est **false** si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-119">The value is **false** if the recipient is not invalid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e6ce7-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="e6ce7-120">Remarks</span></span>

<span data-ttu-id="e6ce7-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6ce7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6ce7-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e6ce7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6ce7-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e6ce7-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6ce7-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e6ce7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e6ce7-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e6ce7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6ce7-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e6ce7-126">Validation File</span></span>  <br/> |<span data-ttu-id="e6ce7-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e6ce7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6ce7-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e6ce7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6ce7-129">False</span><span class="sxs-lookup"><span data-stu-id="e6ce7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6ce7-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e6ce7-130">See also</span></span>



- [<span data-ttu-id="e6ce7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e6ce7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

