---
title: OrganizationRelationshipSettingsCollection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 33456abf-a1b6-46da-a864-3ec8af2780de
description: L’élément OrganizationRelationshipSettingsCollection représente une liste de relations d’organisation qui correspondent à la requête. L’élément OrganizationRelationshipSettingsCollection est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 52f84d932e74393a844f5f55fbd1d09bfb0a5d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462422"
---
# <a name="organizationrelationshipsettingscollection-soap"></a><span data-ttu-id="cf077-105">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf077-105">OrganizationRelationshipSettingsCollection (SOAP)</span></span>

<span data-ttu-id="cf077-106">L’élément **OrganizationRelationshipSettingsCollection** représente une liste de relations d’organisation qui correspondent à la requête.</span><span class="sxs-lookup"><span data-stu-id="cf077-106">The **OrganizationRelationshipSettingsCollection** element represents a list of organization relationships that match the query.</span></span> <span data-ttu-id="cf077-107">L’élément **OrganizationRelationshipSettingsCollection** est réservé à un usage interne.</span><span class="sxs-lookup"><span data-stu-id="cf077-107">The **OrganizationRelationshipSettingsCollection** element is for internal use only.</span></span> <span data-ttu-id="cf077-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="cf077-108">This element is not used by clients.</span></span> 
  
```XML
<OrganizationRelationshipSettingsCollection>
   <OrganizationRelationshipSettings/>
</OrganizationRelationshipSettingsCollection>
```

 <span data-ttu-id="cf077-109">**OrganizationRelationshipSettingsCollection**</span><span class="sxs-lookup"><span data-stu-id="cf077-109">**OrganizationRelationshipSettingsCollection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf077-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cf077-110">Attributes and elements</span></span>

<span data-ttu-id="cf077-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cf077-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf077-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="cf077-112">Attributes</span></span>

<span data-ttu-id="cf077-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cf077-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf077-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cf077-114">Child elements</span></span>

|<span data-ttu-id="cf077-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf077-115">**Element**</span></span>|<span data-ttu-id="cf077-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf077-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf077-117">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf077-117">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="cf077-118">Représente la liste des relations d’organisation pour l’organisation et les adresses SMTP sélectionnées.</span><span class="sxs-lookup"><span data-stu-id="cf077-118">Represents the list of organization relationships for the selected organization and SMTP addresses.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf077-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cf077-119">Parent elements</span></span>

|<span data-ttu-id="cf077-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf077-120">**Element**</span></span>|<span data-ttu-id="cf077-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf077-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf077-122">Réponse (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf077-122">Response (GetOrganizationRelationship) (SOAP)</span></span>](response-getorganizationrelationshipsoap.md) <br/> |<span data-ttu-id="cf077-123">Contient les informations de réponse de l' [opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="cf077-123">Contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf077-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cf077-124">Text value</span></span>

<span data-ttu-id="cf077-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cf077-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf077-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cf077-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf077-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cf077-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cf077-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cf077-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cf077-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="cf077-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cf077-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cf077-130">Validation File</span></span>  <br/> |<span data-ttu-id="cf077-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cf077-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf077-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cf077-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf077-133">True</span><span class="sxs-lookup"><span data-stu-id="cf077-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf077-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf077-134">See also</span></span>



[<span data-ttu-id="cf077-135">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf077-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

