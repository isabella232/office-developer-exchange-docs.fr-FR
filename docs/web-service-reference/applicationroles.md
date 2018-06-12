---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: L’élément ApplicationRoles spécifie les rôles d’application que l’application partenaire appelant utilise pour l’appel en cours.
ms.openlocfilehash: ff32b693dae573416263bcb7c0fbb552a933b8d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755218"
---
# <a name="applicationroles"></a><span data-ttu-id="0865d-103">ApplicationRoles</span><span class="sxs-lookup"><span data-stu-id="0865d-103">ApplicationRoles</span></span>

<span data-ttu-id="0865d-104">L’élément **ApplicationRoles** spécifie les rôles d’application que l’application partenaire appelant utilise pour l’appel en cours.</span><span class="sxs-lookup"><span data-stu-id="0865d-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="0865d-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="0865d-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0865d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0865d-106">Attributes and elements</span></span>

<span data-ttu-id="0865d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0865d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0865d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0865d-108">Attributes</span></span>

<span data-ttu-id="0865d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0865d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0865d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0865d-110">Child elements</span></span>

|<span data-ttu-id="0865d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0865d-111">**Element**</span></span>|<span data-ttu-id="0865d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0865d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0865d-113">Rôle</span><span class="sxs-lookup"><span data-stu-id="0865d-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="0865d-114">Spécifie une chaîne qui représente un rôle de gestion.</span><span class="sxs-lookup"><span data-stu-id="0865d-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0865d-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0865d-115">Parent elements</span></span>

|<span data-ttu-id="0865d-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0865d-116">**Element**</span></span>|<span data-ttu-id="0865d-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="0865d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0865d-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="0865d-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="0865d-119">Spécifie le rôle de gestion.</span><span class="sxs-lookup"><span data-stu-id="0865d-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0865d-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="0865d-120">Remarks</span></span>

<span data-ttu-id="0865d-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0865d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0865d-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0865d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0865d-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0865d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0865d-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0865d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0865d-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0865d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0865d-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="0865d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="0865d-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="0865d-127">Validation File</span></span>  <br/> |<span data-ttu-id="0865d-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="0865d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0865d-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0865d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0865d-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0865d-130">See also</span></span>

- [<span data-ttu-id="0865d-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0865d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

