---
title: IsPermissionControlled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPermissionControlled
api_type:
- schema
ms.assetid: a2fd0340-f31f-4389-a1cd-7e93b40bb3c6
description: L’élément IsPermissionControlled indique si les messages entrants doivent être contrôlés par des autorisations (protection RMS) afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 5fba06c1c56512f4a362f773f119ea346a4c0d2b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460385"
---
# <a name="ispermissioncontrolled"></a><span data-ttu-id="67b36-103">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="67b36-103">IsPermissionControlled</span></span>

<span data-ttu-id="67b36-104">L’élément **IsPermissionControlled** indique si les messages entrants doivent être contrôlés par des autorisations (protection RMS) afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="67b36-104">The **IsPermissionControlled** element indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsPermissionControlled>true | false</IsPermissionControlled>
```

 <span data-ttu-id="67b36-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="67b36-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67b36-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="67b36-106">Attributes and elements</span></span>

<span data-ttu-id="67b36-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="67b36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67b36-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="67b36-108">Attributes</span></span>

<span data-ttu-id="67b36-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="67b36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67b36-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="67b36-110">Child elements</span></span>

<span data-ttu-id="67b36-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="67b36-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67b36-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="67b36-112">Parent elements</span></span>

|<span data-ttu-id="67b36-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67b36-113">**Element**</span></span>|<span data-ttu-id="67b36-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="67b36-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67b36-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="67b36-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="67b36-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="67b36-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="67b36-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="67b36-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="67b36-118">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="67b36-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67b36-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="67b36-119">Text value</span></span>

<span data-ttu-id="67b36-120">Une valeur de texte **true** indique que le message doit être protégé par RMS afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="67b36-120">A text value of **true** indicates that the message must be RMS protected in order for the condition or exception to apply.</span></span> <span data-ttu-id="67b36-121">La valeur **false** indique que le message ne doit pas être protégé par RMS afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="67b36-121">A value of **false** indicates that the message must not be RMS protected in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="67b36-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="67b36-122">Remarks</span></span>

<span data-ttu-id="67b36-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="67b36-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67b36-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="67b36-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67b36-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="67b36-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="67b36-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="67b36-126">Schema Name</span></span>  <br/> |<span data-ttu-id="67b36-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="67b36-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="67b36-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="67b36-128">Validation File</span></span>  <br/> |<span data-ttu-id="67b36-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="67b36-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="67b36-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="67b36-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="67b36-131">True</span><span class="sxs-lookup"><span data-stu-id="67b36-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67b36-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="67b36-132">See also</span></span>



- [<span data-ttu-id="67b36-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="67b36-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

