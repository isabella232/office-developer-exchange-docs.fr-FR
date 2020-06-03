---
title: InvalidRecipient (infos-courrier)
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
ms.openlocfilehash: fddd75beb2228c50084bd38b4f4745064cc281dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530001"
---
# <a name="invalidrecipient-mailtips"></a><span data-ttu-id="b3aa1-103">InvalidRecipient (infos-courrier)</span><span class="sxs-lookup"><span data-stu-id="b3aa1-103">InvalidRecipient (MailTips)</span></span>

<span data-ttu-id="b3aa1-104">L’élément **InvalidRecipient** indique si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-104">The **InvalidRecipient** element indicates whether the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
```

 <span data-ttu-id="b3aa1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b3aa1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3aa1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b3aa1-106">Attributes and elements</span></span>

<span data-ttu-id="b3aa1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3aa1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b3aa1-108">Attributes</span></span>

<span data-ttu-id="b3aa1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3aa1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b3aa1-110">Child elements</span></span>

<span data-ttu-id="b3aa1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b3aa1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b3aa1-112">Parent elements</span></span>

|<span data-ttu-id="b3aa1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3aa1-113">**Element**</span></span>|<span data-ttu-id="b3aa1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3aa1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3aa1-115">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="b3aa1-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="b3aa1-116">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b3aa1-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b3aa1-117">Text value</span></span>

<span data-ttu-id="b3aa1-118">La valeur de texte de cet élément est **true** si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-118">The text value of this element is **true** if the recipient is invalid.</span></span> <span data-ttu-id="b3aa1-119">La valeur est **false** si le destinataire n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-119">The value is **false** if the recipient is not invalid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b3aa1-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="b3aa1-120">Remarks</span></span>

<span data-ttu-id="b3aa1-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3aa1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3aa1-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b3aa1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3aa1-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b3aa1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3aa1-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b3aa1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="b3aa1-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b3aa1-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b3aa1-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b3aa1-126">Validation File</span></span>  <br/> |<span data-ttu-id="b3aa1-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b3aa1-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3aa1-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b3aa1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="b3aa1-129">False</span><span class="sxs-lookup"><span data-stu-id="b3aa1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3aa1-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3aa1-130">See also</span></span>



- [<span data-ttu-id="b3aa1-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b3aa1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

