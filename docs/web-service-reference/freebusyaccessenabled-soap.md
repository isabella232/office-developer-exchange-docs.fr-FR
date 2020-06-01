---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: L’élément FreeBusyAccessEnabled représente l’indicateur FreeBusyAccessEnabled (). L’élément FreeBusyAccessEnabled est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: c148d8fa1301339f8579884dc02b6c9e452f3035
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461295"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="5e9b6-105">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5e9b6-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="5e9b6-106">L’élément **FreeBusyAccessEnabled** représente l’indicateur **FreeBusyAccessEnabled ()** .</span><span class="sxs-lookup"><span data-stu-id="5e9b6-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="5e9b6-107">L’élément **FreeBusyAccessEnabled** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="5e9b6-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="5e9b6-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5e9b6-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e9b6-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5e9b6-110">Attributes and elements</span></span>

<span data-ttu-id="5e9b6-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e9b6-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="5e9b6-112">Attributes</span></span>

<span data-ttu-id="5e9b6-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e9b6-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5e9b6-114">Child elements</span></span>

<span data-ttu-id="5e9b6-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e9b6-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5e9b6-116">Parent elements</span></span>

|<span data-ttu-id="5e9b6-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5e9b6-117">**Element**</span></span>|<span data-ttu-id="5e9b6-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="5e9b6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e9b6-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5e9b6-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="5e9b6-120">Représente une liste de relations d’organisation pour une seule organisation.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5e9b6-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5e9b6-121">Text value</span></span>

<span data-ttu-id="5e9b6-122">Une valeur de texte de **true** pour l’élément **FreeBusyAccessEnabled** indique que la relation de partage doit être utilisée pour récupérer les informations de disponibilité des utilisateurs de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="5e9b6-123">La valeur **false** indique que la relation de partage doit être supprimée.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5e9b6-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="5e9b6-124">Remarks</span></span>

<span data-ttu-id="5e9b6-125">Utilisez cet élément pour autoriser ou supprimer les informations de disponibilité du serveur.</span><span class="sxs-lookup"><span data-stu-id="5e9b6-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5e9b6-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5e9b6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e9b6-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5e9b6-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5e9b6-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5e9b6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5e9b6-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="5e9b6-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5e9b6-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5e9b6-130">Validation File</span></span>  <br/> |<span data-ttu-id="5e9b6-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5e9b6-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5e9b6-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5e9b6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e9b6-133">True</span><span class="sxs-lookup"><span data-stu-id="5e9b6-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e9b6-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5e9b6-134">See also</span></span>



[<span data-ttu-id="5e9b6-135">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5e9b6-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

