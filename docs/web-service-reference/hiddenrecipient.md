---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: L’élément HiddenRecipient indique que le destinataire a été ajouté par une stratégie d’organisation qui doit être masquée pour les utilisateurs non privilégiés.
ms.openlocfilehash: bfe57fabc02ff00c801672b71ccdb0bf1b916bd9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457640"
---
# <a name="hiddenrecipient"></a><span data-ttu-id="c8834-103">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="c8834-103">HiddenRecipient</span></span>

<span data-ttu-id="c8834-104">L’élément **HiddenRecipient** indique que le destinataire a été ajouté par une stratégie d’organisation qui doit être masquée pour les utilisateurs non privilégiés.</span><span class="sxs-lookup"><span data-stu-id="c8834-104">The **HiddenRecipient** element indicates that the recipient was added by an organization policy that should be hidden from unprivileged users.</span></span> 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 <span data-ttu-id="c8834-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c8834-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8834-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c8834-106">Attributes and elements</span></span>

<span data-ttu-id="c8834-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c8834-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8834-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c8834-108">Attributes</span></span>

<span data-ttu-id="c8834-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c8834-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8834-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c8834-110">Child elements</span></span>

<span data-ttu-id="c8834-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c8834-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8834-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c8834-112">Parent elements</span></span>

|<span data-ttu-id="c8834-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c8834-113">**Element**</span></span>|<span data-ttu-id="c8834-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c8834-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8834-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="c8834-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="c8834-116">Contient des informations pour un seul événement pour un destinataire.</span><span class="sxs-lookup"><span data-stu-id="c8834-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8834-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c8834-117">Text value</span></span>

<span data-ttu-id="c8834-118">Cet élément peut avoir la **valeur true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="c8834-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="c8834-119">La valeur **true** indique que l’utilisateur a été ajouté par une stratégie d’organisation ; la valeur **false** indique que l’utilisateur n’a pas été ajouté par une stratégie d’organisation.</span><span class="sxs-lookup"><span data-stu-id="c8834-119">A value of **true** indicates that the user was added by an organization policy; a value of **false** indicates that the user was not added by an organization policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c8834-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="c8834-120">Remarks</span></span>

<span data-ttu-id="c8834-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8834-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8834-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c8834-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8834-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c8834-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8834-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c8834-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c8834-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c8834-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8834-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c8834-126">Validation File</span></span>  <br/> |<span data-ttu-id="c8834-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c8834-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8834-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c8834-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8834-129">False</span><span class="sxs-lookup"><span data-stu-id="c8834-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8834-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c8834-130">See also</span></span>



- [<span data-ttu-id="c8834-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c8834-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

