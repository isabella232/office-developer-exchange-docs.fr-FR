---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: L’élément UserRoles spécifie les rôles d’utilisateur que l’utilisateur appelant, ou l’utilisateur qui agit comme application partenaire, souhaite appliquer à l’appel actif.
ms.openlocfilehash: 5155b82781321b16d1b58fdcaffe7b8cf2372717
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467129"
---
# <a name="userroles"></a><span data-ttu-id="2719b-103">UserRoles</span><span class="sxs-lookup"><span data-stu-id="2719b-103">UserRoles</span></span>

<span data-ttu-id="2719b-104">L’élément **UserRoles** spécifie les rôles d’utilisateur que l’utilisateur appelant, ou l’utilisateur qui agit comme application partenaire, souhaite appliquer à l’appel actif.</span><span class="sxs-lookup"><span data-stu-id="2719b-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="2719b-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="2719b-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2719b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2719b-106">Attributes and elements</span></span>

<span data-ttu-id="2719b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2719b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2719b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2719b-108">Attributes</span></span>

<span data-ttu-id="2719b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2719b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2719b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2719b-110">Child elements</span></span>

[<span data-ttu-id="2719b-111">Role</span><span class="sxs-lookup"><span data-stu-id="2719b-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="2719b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2719b-112">Parent elements</span></span>

[<span data-ttu-id="2719b-113">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="2719b-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="2719b-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="2719b-114">Remarks</span></span>

<span data-ttu-id="2719b-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2719b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2719b-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2719b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2719b-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2719b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2719b-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2719b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2719b-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2719b-119">Schema name</span></span>  <br/> |<span data-ttu-id="2719b-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2719b-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="2719b-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2719b-121">Validation file</span></span>  <br/> |<span data-ttu-id="2719b-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2719b-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2719b-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2719b-123">Can be empty</span></span>  <br/> ||
   

