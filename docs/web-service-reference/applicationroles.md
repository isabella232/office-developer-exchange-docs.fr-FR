---
title: ApplicationRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: L’élément ApplicationRoles spécifie les rôles d’application utilisés par l’application partenaire appelante pour l’appel actif.
ms.openlocfilehash: 8dfe5c745896d02217cbf91375d355954a4e22eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464699"
---
# <a name="applicationroles"></a><span data-ttu-id="00d95-103">ApplicationRoles</span><span class="sxs-lookup"><span data-stu-id="00d95-103">ApplicationRoles</span></span>

<span data-ttu-id="00d95-104">L’élément **ApplicationRoles** spécifie les rôles d’application utilisés par l’application partenaire appelante pour l’appel actif.</span><span class="sxs-lookup"><span data-stu-id="00d95-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="00d95-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="00d95-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00d95-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00d95-106">Attributes and elements</span></span>

<span data-ttu-id="00d95-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00d95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00d95-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00d95-108">Attributes</span></span>

<span data-ttu-id="00d95-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00d95-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00d95-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00d95-110">Child elements</span></span>

|<span data-ttu-id="00d95-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00d95-111">**Element**</span></span>|<span data-ttu-id="00d95-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="00d95-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00d95-113">Role</span><span class="sxs-lookup"><span data-stu-id="00d95-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="00d95-114">Spécifie une chaîne qui représente un rôle de gestion.</span><span class="sxs-lookup"><span data-stu-id="00d95-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00d95-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00d95-115">Parent elements</span></span>

|<span data-ttu-id="00d95-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00d95-116">**Element**</span></span>|<span data-ttu-id="00d95-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="00d95-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00d95-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="00d95-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="00d95-119">Spécifie le rôle de gestion.</span><span class="sxs-lookup"><span data-stu-id="00d95-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00d95-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="00d95-120">Remarks</span></span>

<span data-ttu-id="00d95-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00d95-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00d95-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00d95-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00d95-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00d95-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00d95-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00d95-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00d95-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00d95-125">Schema Name</span></span>  <br/> |<span data-ttu-id="00d95-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="00d95-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="00d95-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="00d95-127">Validation File</span></span>  <br/> |<span data-ttu-id="00d95-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="00d95-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="00d95-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00d95-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="00d95-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00d95-130">See also</span></span>

- [<span data-ttu-id="00d95-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00d95-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

