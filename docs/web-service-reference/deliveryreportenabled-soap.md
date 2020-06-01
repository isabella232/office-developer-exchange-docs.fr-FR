---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: L’élément DeliveryReportEnabled représente l’indicateur DeliveryReportEnabled (). L’élément DeliveryReportEnabled est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 2a163b3e6ceaa169cc8f76f395b7d501419a31ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458473"
---
# <a name="deliveryreportenabled-soap"></a><span data-ttu-id="55773-105">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="55773-105">DeliveryReportEnabled (SOAP)</span></span>

<span data-ttu-id="55773-106">L’élément **DeliveryReportEnabled** représente l’indicateur **DeliveryReportEnabled ()** .</span><span class="sxs-lookup"><span data-stu-id="55773-106">The **DeliveryReportEnabled** element represents the **DeliveryReportEnabled()** flag.</span></span> <span data-ttu-id="55773-107">L’élément **DeliveryReportEnabled** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="55773-107">The **DeliveryReportEnabled** element is for internal use only.</span></span> <span data-ttu-id="55773-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="55773-108">This element is not used by clients.</span></span> 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 <span data-ttu-id="55773-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="55773-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55773-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55773-110">Attributes and elements</span></span>

<span data-ttu-id="55773-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55773-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55773-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="55773-112">Attributes</span></span>

<span data-ttu-id="55773-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="55773-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55773-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55773-114">Child elements</span></span>

<span data-ttu-id="55773-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55773-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55773-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55773-116">Parent elements</span></span>

|<span data-ttu-id="55773-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55773-117">**Element**</span></span>|<span data-ttu-id="55773-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="55773-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55773-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="55773-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="55773-120">Représente une liste de relations d’organisation pour une seule organisation.</span><span class="sxs-lookup"><span data-stu-id="55773-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55773-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="55773-121">Text value</span></span>

<span data-ttu-id="55773-122">Une valeur de texte de true pour l’élément DeliveryReportEnabled indique que les rapports de remise des utilisateurs de l’organisation peuvent être utilisés.</span><span class="sxs-lookup"><span data-stu-id="55773-122">A text value of true for the DeliveryReportEnabled element indicates that the delivery reports from users in the organization can be used.</span></span> <span data-ttu-id="55773-123">La valeur false indique que les rapports de remise doivent être supprimés.</span><span class="sxs-lookup"><span data-stu-id="55773-123">A value of false indicates that the delivery reports should suppressed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55773-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="55773-124">Remarks</span></span>

<span data-ttu-id="55773-125">Utilisez cet élément pour autoriser ou supprimer des rapports de remise du serveur.</span><span class="sxs-lookup"><span data-stu-id="55773-125">Use this element to allow or suppress delivery reports from the server.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55773-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55773-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55773-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55773-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="55773-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55773-128">Schema Name</span></span>  <br/> |<span data-ttu-id="55773-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="55773-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="55773-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55773-130">Validation File</span></span>  <br/> |<span data-ttu-id="55773-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="55773-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55773-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55773-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="55773-133">True</span><span class="sxs-lookup"><span data-stu-id="55773-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55773-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55773-134">See also</span></span>

- [<span data-ttu-id="55773-135">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="55773-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

