---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: L’élément UserRoles spécifie les rôles d’utilisateur que l’utilisateur ou l’application partenaire appelant agissant en tant que l’utilisateur souhaite s’appliquent à l’appel en cours.
ms.openlocfilehash: 19dc1a7e00decb9141326b53b650d72101013c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838974"
---
# <a name="userroles"></a><span data-ttu-id="9f1ba-103">UserRoles</span><span class="sxs-lookup"><span data-stu-id="9f1ba-103">UserRoles</span></span>

<span data-ttu-id="9f1ba-104">L’élément **UserRoles** spécifie les rôles d’utilisateur que l’utilisateur ou l’application partenaire appelant agissant en tant que l’utilisateur souhaite s’appliquent à l’appel en cours.</span><span class="sxs-lookup"><span data-stu-id="9f1ba-104">The **UserRoles** element specifies the user roles that the calling user, or the user that the calling partner application is acting as, wants to apply to the current call.</span></span> 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 <span data-ttu-id="9f1ba-105">**NonEmptyArrayOfRoleType**</span><span class="sxs-lookup"><span data-stu-id="9f1ba-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f1ba-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9f1ba-106">Attributes and elements</span></span>

<span data-ttu-id="9f1ba-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9f1ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f1ba-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9f1ba-108">Attributes</span></span>

<span data-ttu-id="9f1ba-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9f1ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f1ba-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9f1ba-110">Child elements</span></span>

[<span data-ttu-id="9f1ba-111">Rôle</span><span class="sxs-lookup"><span data-stu-id="9f1ba-111">Role</span></span>](role.md)
  
### <a name="parent-elements"></a><span data-ttu-id="9f1ba-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9f1ba-112">Parent elements</span></span>

[<span data-ttu-id="9f1ba-113">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="9f1ba-113">ManagementRole</span></span>](managementrole.md)
  
## <a name="remarks"></a><span data-ttu-id="9f1ba-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="9f1ba-114">Remarks</span></span>

<span data-ttu-id="9f1ba-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9f1ba-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f1ba-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f1ba-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f1ba-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9f1ba-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f1ba-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9f1ba-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f1ba-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9f1ba-119">Schema name</span></span>  <br/> |<span data-ttu-id="9f1ba-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9f1ba-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f1ba-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9f1ba-121">Validation file</span></span>  <br/> |<span data-ttu-id="9f1ba-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9f1ba-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f1ba-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9f1ba-123">Can be empty</span></span>  <br/> ||
   

