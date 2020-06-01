---
title: IsNDR
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNDR
api_type:
- schema
ms.assetid: 194f5836-7793-463a-a090-4386d1c2487a
description: L’élément IsNDR indique si les messages entrants doivent être des notifications d’échec de remise (NDR) afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 3476331ccece347686b7f98edf49df5d48b8562e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458158"
---
# <a name="isndr"></a><span data-ttu-id="3574f-103">IsNDR</span><span class="sxs-lookup"><span data-stu-id="3574f-103">IsNDR</span></span>

<span data-ttu-id="3574f-104">L’élément **IsNDR** indique si les messages entrants doivent être des notifications d’échec de remise (NDR) afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="3574f-104">The **IsNDR** element indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsNDR>true | false</IsNDR>
```

 <span data-ttu-id="3574f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3574f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3574f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3574f-106">Attributes and elements</span></span>

<span data-ttu-id="3574f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3574f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3574f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3574f-108">Attributes</span></span>

<span data-ttu-id="3574f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3574f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3574f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3574f-110">Child elements</span></span>

<span data-ttu-id="3574f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3574f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3574f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3574f-112">Parent elements</span></span>

|<span data-ttu-id="3574f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3574f-113">**Element**</span></span>|<span data-ttu-id="3574f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3574f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3574f-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="3574f-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="3574f-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="3574f-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="3574f-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="3574f-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="3574f-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="3574f-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3574f-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3574f-119">Text value</span></span>

<span data-ttu-id="3574f-120">Une valeur de texte **true** indique que le message doit être un rapport de non-remise afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="3574f-120">A text value of **true** indicates that the message must be an NDR in order for the condition or exception to apply.</span></span> <span data-ttu-id="3574f-121">La valeur **false** indique que le message ne doit pas être un rapport de non-remise afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="3574f-121">A value of **false** indicates that the message must not be an NDR in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3574f-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3574f-122">Remarks</span></span>

<span data-ttu-id="3574f-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3574f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3574f-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3574f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3574f-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3574f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3574f-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3574f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3574f-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3574f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3574f-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3574f-128">Validation File</span></span>  <br/> |<span data-ttu-id="3574f-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3574f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3574f-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3574f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3574f-131">True</span><span class="sxs-lookup"><span data-stu-id="3574f-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3574f-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3574f-132">See also</span></span>



- [<span data-ttu-id="3574f-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3574f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

