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
description: L’élément DeliveryRestricted indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire.
ms.openlocfilehash: ba1c6e00b93c9e442a427fe98a5e15bf5fe1effd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755892"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="123bb-103">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="123bb-103">DeliveryRestricted</span></span>

<span data-ttu-id="123bb-104">L’élément **DeliveryRestricted** indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="123bb-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="123bb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="123bb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="123bb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="123bb-106">Attributes and elements</span></span>

<span data-ttu-id="123bb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="123bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="123bb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="123bb-108">Attributes</span></span>

<span data-ttu-id="123bb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="123bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="123bb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="123bb-110">Child elements</span></span>

<span data-ttu-id="123bb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="123bb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="123bb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="123bb-112">Parent elements</span></span>

|<span data-ttu-id="123bb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="123bb-113">**Element**</span></span>|<span data-ttu-id="123bb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="123bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="123bb-115">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="123bb-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="123bb-116">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="123bb-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="123bb-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="123bb-117">Text value</span></span>

<span data-ttu-id="123bb-118">La valeur de texte de cet élément est **la valeur true** si les restrictions de remise empêchera le message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="123bb-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="123bb-119">La valeur est **false** si les restrictions de remise n’empêcheront pas de message de l’expéditeur d’atteindre le destinataire.</span><span class="sxs-lookup"><span data-stu-id="123bb-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="123bb-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="123bb-120">Remarks</span></span>

<span data-ttu-id="123bb-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="123bb-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="123bb-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="123bb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="123bb-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="123bb-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="123bb-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="123bb-124">Schema Name</span></span>  <br/> |<span data-ttu-id="123bb-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="123bb-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="123bb-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="123bb-126">Validation File</span></span>  <br/> |<span data-ttu-id="123bb-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="123bb-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="123bb-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="123bb-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="123bb-129">False</span><span class="sxs-lookup"><span data-stu-id="123bb-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="123bb-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="123bb-130">See also</span></span>

- [<span data-ttu-id="123bb-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="123bb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

