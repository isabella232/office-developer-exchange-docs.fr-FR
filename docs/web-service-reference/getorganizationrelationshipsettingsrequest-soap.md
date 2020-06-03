---
title: GetOrganizationRelationshipSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4e8aa3b3-4bfc-40c3-b96b-9f7062b09309
description: L’élément GetOrganizationRelationshipSettingsRequest représente les paramètres d’un appel à l’opération SOAP (GetOrganizationRelationshipSettings Operation). L’élément GetOrganizationRelationshipSettingsRequest est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 053bbb8cbe2ccdcf6d544ab1fc92bb81765997e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452733"
---
# <a name="getorganizationrelationshipsettingsrequest-soap"></a><span data-ttu-id="e50b8-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e50b8-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>

<span data-ttu-id="e50b8-106">L’élément **GetOrganizationRelationshipSettingsRequest** représente les paramètres d’un appel à l’opération [SOAP (GetOrganizationRelationshipSettings Operation)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="e50b8-106">The **GetOrganizationRelationshipSettingsRequest** element represents the parameters of a call to the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation.</span></span> <span data-ttu-id="e50b8-107">L’élément **GetOrganizationRelationshipSettingsRequest** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="e50b8-107">The **GetOrganizationRelationshipSettingsRequest** element is for internal use only.</span></span> <span data-ttu-id="e50b8-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="e50b8-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsRequest>
   <Domains/>
</GetOrganizationRelationshipSettingsRequest>
```

 <span data-ttu-id="e50b8-109">**GetOrganizationRelationshipSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="e50b8-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e50b8-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e50b8-110">Attributes and elements</span></span>

<span data-ttu-id="e50b8-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e50b8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e50b8-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="e50b8-112">Attributes</span></span>

<span data-ttu-id="e50b8-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e50b8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e50b8-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e50b8-114">Child elements</span></span>

|<span data-ttu-id="e50b8-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e50b8-115">**Element**</span></span>|<span data-ttu-id="e50b8-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="e50b8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e50b8-117">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e50b8-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="e50b8-118">Représente une collection d’identificateurs de domaine.</span><span class="sxs-lookup"><span data-stu-id="e50b8-118">Represents a collection of domain identifiers.</span></span>  <br/> |
|||
   
### <a name="parent-elements"></a><span data-ttu-id="e50b8-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e50b8-119">Parent elements</span></span>

<span data-ttu-id="e50b8-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e50b8-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e50b8-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e50b8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e50b8-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e50b8-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e50b8-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e50b8-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e50b8-124">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="e50b8-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e50b8-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e50b8-125">Validation File</span></span>  <br/> |<span data-ttu-id="e50b8-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e50b8-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e50b8-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e50b8-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e50b8-128">True</span><span class="sxs-lookup"><span data-stu-id="e50b8-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e50b8-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e50b8-129">See also</span></span>



[<span data-ttu-id="e50b8-130">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e50b8-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

