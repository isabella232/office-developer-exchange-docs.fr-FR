---
title: HasChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 15ff513d-f39e-44ed-a13f-ab3f86fa37e1
description: L’élément HasChanged indique si la photo d’un utilisateur a été modifiée.
ms.openlocfilehash: d777220f55d33cde548d8257cf249b57481a43f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462786"
---
# <a name="haschanged"></a><span data-ttu-id="4d0fe-103">HasChanged</span><span class="sxs-lookup"><span data-stu-id="4d0fe-103">HasChanged</span></span>

<span data-ttu-id="4d0fe-104">L’élément **HasChanged** indique si la photo d’un utilisateur a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-104">The **HasChanged** element indicates whether a user's photo has changed.</span></span> 
  
```XML
<HasChanged> true | false </HasChanged>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="4d0fe-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d0fe-105">Attributes and elements</span></span>

<span data-ttu-id="4d0fe-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d0fe-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d0fe-107">Attributes</span></span>

<span data-ttu-id="4d0fe-108">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d0fe-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d0fe-109">Child elements</span></span>

<span data-ttu-id="4d0fe-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4d0fe-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d0fe-111">Parent elements</span></span>

[<span data-ttu-id="4d0fe-112">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="4d0fe-112">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
  
## <a name="text-value"></a><span data-ttu-id="4d0fe-113">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4d0fe-113">Text value</span></span>

<span data-ttu-id="4d0fe-114">Une valeur de texte de **true** pour l’élément **HasChanged** indique que la photo a changé depuis son dernier renvoi.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-114">A text value of **true** for the **HasChanged** element indicates that the photo has changed since the last time it was returned.</span></span> <span data-ttu-id="4d0fe-115">La valeur **false** indique que la photo n’a pas été modifiée depuis son dernier renvoi.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-115">A value of **false** indicates that the photo has not changed since the last time it was returned.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4d0fe-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="4d0fe-116">Remarks</span></span>

<span data-ttu-id="4d0fe-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d0fe-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d0fe-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d0fe-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d0fe-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d0fe-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d0fe-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d0fe-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d0fe-121">Schema name</span></span>  <br/> |<span data-ttu-id="4d0fe-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4d0fe-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d0fe-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d0fe-123">Validation file</span></span>  <br/> |<span data-ttu-id="4d0fe-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d0fe-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d0fe-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d0fe-125">Can be empty</span></span>  <br/> ||
   

