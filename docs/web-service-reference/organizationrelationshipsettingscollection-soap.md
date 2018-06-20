---
title: OrganizationRelationshipSettingsCollection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 33456abf-a1b6-46da-a864-3ec8af2780de
description: L’élément OrganizationRelationshipSettingsCollection représente une liste des relations qui correspondent à la requête. L’élément OrganizationRelationshipSettingsCollection est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 18e71ce39d48598868d677a37d5ba439fa6d59c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828663"
---
# <a name="organizationrelationshipsettingscollection-soap"></a><span data-ttu-id="05969-105">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05969-105">OrganizationRelationshipSettingsCollection (SOAP)</span></span>

<span data-ttu-id="05969-106">L’élément **OrganizationRelationshipSettingsCollection** représente une liste des relations qui correspondent à la requête.</span><span class="sxs-lookup"><span data-stu-id="05969-106">The **OrganizationRelationshipSettingsCollection** element represents a list of organization relationships that match the query.</span></span> <span data-ttu-id="05969-107">L’élément **OrganizationRelationshipSettingsCollection** est à usage interne uniquement.</span><span class="sxs-lookup"><span data-stu-id="05969-107">The **OrganizationRelationshipSettingsCollection** element is for internal use only.</span></span> <span data-ttu-id="05969-108">Cet élément n’est pas utilisé par les clients.</span><span class="sxs-lookup"><span data-stu-id="05969-108">This element is not used by clients.</span></span> 
  
```XML
<OrganizationRelationshipSettingsCollection>
   <OrganizationRelationshipSettings/>
</OrganizationRelationshipSettingsCollection>
```

 <span data-ttu-id="05969-109">**OrganizationRelationshipSettingsCollection**</span><span class="sxs-lookup"><span data-stu-id="05969-109">**OrganizationRelationshipSettingsCollection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05969-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05969-110">Attributes and elements</span></span>

<span data-ttu-id="05969-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05969-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05969-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="05969-112">Attributes</span></span>

<span data-ttu-id="05969-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05969-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05969-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05969-114">Child elements</span></span>

|<span data-ttu-id="05969-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05969-115">**Element**</span></span>|<span data-ttu-id="05969-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="05969-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05969-117">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05969-117">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="05969-118">Représente la liste des relations d’organisation pour l’organisation sélectionnée et les adresses SMTP.</span><span class="sxs-lookup"><span data-stu-id="05969-118">Represents the list of organization relationships for the selected organization and SMTP addresses.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05969-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05969-119">Parent elements</span></span>

|<span data-ttu-id="05969-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05969-120">**Element**</span></span>|<span data-ttu-id="05969-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="05969-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05969-122">Réponse (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05969-122">Response (GetOrganizationRelationship) (SOAP)</span></span>](response-getorganizationrelationshipsoap.md) <br/> |<span data-ttu-id="05969-123">Contient les informations de réponse de [l’opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="05969-123">Contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05969-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="05969-124">Text value</span></span>

<span data-ttu-id="05969-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05969-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05969-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05969-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05969-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05969-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="05969-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05969-128">Schema Name</span></span>  <br/> |<span data-ttu-id="05969-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="05969-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="05969-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05969-130">Validation File</span></span>  <br/> |<span data-ttu-id="05969-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="05969-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="05969-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05969-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="05969-133">True</span><span class="sxs-lookup"><span data-stu-id="05969-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05969-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05969-134">See also</span></span>



[<span data-ttu-id="05969-135">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="05969-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

