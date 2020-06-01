---
title: DeliveryRestricted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: L’élément DeliveryRestricted indique si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire.
ms.openlocfilehash: 58fc85873326179d7745db4ba7d4854a76ced6a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462688"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="dc9f5-103">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="dc9f5-103">DeliveryRestricted</span></span>

<span data-ttu-id="dc9f5-104">L’élément **DeliveryRestricted** indique si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="dc9f5-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="dc9f5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc9f5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dc9f5-106">Attributes and elements</span></span>

<span data-ttu-id="dc9f5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc9f5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dc9f5-108">Attributes</span></span>

<span data-ttu-id="dc9f5-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc9f5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dc9f5-110">Child elements</span></span>

<span data-ttu-id="dc9f5-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc9f5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dc9f5-112">Parent elements</span></span>

|<span data-ttu-id="dc9f5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dc9f5-113">**Element**</span></span>|<span data-ttu-id="dc9f5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="dc9f5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc9f5-115">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="dc9f5-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="dc9f5-116">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dc9f5-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="dc9f5-117">Text value</span></span>

<span data-ttu-id="dc9f5-118">La valeur texte de cet élément est **true** si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="dc9f5-119">La valeur est **false** si les restrictions de remise n’empêchent pas le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dc9f5-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="dc9f5-120">Remarks</span></span>

<span data-ttu-id="dc9f5-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="dc9f5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc9f5-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dc9f5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc9f5-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dc9f5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc9f5-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dc9f5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="dc9f5-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dc9f5-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc9f5-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dc9f5-126">Validation File</span></span>  <br/> |<span data-ttu-id="dc9f5-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dc9f5-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc9f5-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dc9f5-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc9f5-129">False</span><span class="sxs-lookup"><span data-stu-id="dc9f5-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc9f5-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dc9f5-130">See also</span></span>

- [<span data-ttu-id="dc9f5-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dc9f5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

