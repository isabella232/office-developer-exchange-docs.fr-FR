---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: L’élément TargetApplicationUri définit l’URI de l’application cible. L’élément TargetApplicationUri est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 88968aac604b77cd057dbc69c396227a489ac9a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457087"
---
# <a name="targetapplicationuri-soap"></a><span data-ttu-id="ea6ec-105">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea6ec-105">TargetApplicationUri (SOAP)</span></span>

<span data-ttu-id="ea6ec-106">L’élément **TargetApplicationUri** définit l’URI de l’application cible.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-106">The **TargetApplicationUri** element defines the target application URI.</span></span> <span data-ttu-id="ea6ec-107">L’élément **TargetApplicationUri** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-107">The **TargetApplicationUri** element is for internal use only.</span></span> <span data-ttu-id="ea6ec-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-108">This element is not used by clients.</span></span> 
  
```XML
<TargetApplicationUri/>
```

 <span data-ttu-id="ea6ec-109">**Yuri**</span><span class="sxs-lookup"><span data-stu-id="ea6ec-109">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea6ec-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ea6ec-110">Attributes and elements</span></span>

<span data-ttu-id="ea6ec-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea6ec-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="ea6ec-112">Attributes</span></span>

<span data-ttu-id="ea6ec-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea6ec-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ea6ec-114">Child elements</span></span>

<span data-ttu-id="ea6ec-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea6ec-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ea6ec-116">Parent elements</span></span>

|<span data-ttu-id="ea6ec-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea6ec-117">**Element**</span></span>|<span data-ttu-id="ea6ec-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea6ec-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea6ec-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea6ec-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="ea6ec-120">Représente une liste de relations d’organisation pour une seule organisation.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-120">Represents a list of organization relationships for a single organization</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea6ec-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="ea6ec-121">Remarks</span></span>

<span data-ttu-id="ea6ec-122">Cet élément définit l’URI cible de l’organisation externe.</span><span class="sxs-lookup"><span data-stu-id="ea6ec-122">This element defines the target URI of the external organization.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea6ec-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ea6ec-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea6ec-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ea6ec-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ea6ec-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ea6ec-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ea6ec-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ea6ec-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ea6ec-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ea6ec-127">Validation File</span></span>  <br/> |<span data-ttu-id="ea6ec-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ea6ec-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea6ec-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ea6ec-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea6ec-130">True</span><span class="sxs-lookup"><span data-stu-id="ea6ec-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea6ec-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ea6ec-131">See also</span></span>



[<span data-ttu-id="ea6ec-132">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ea6ec-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

