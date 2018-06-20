---
title: SetPlayOnPhoneDialString (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: L’élément SetPlayOnPhoneDialString définit une demande pour définir la chaîne de numérotation par défaut pour l’opération PlayOnPhone (service web de messagerie unifiée) et les demandes d’opérations (service web de messagerie unifiée) PlayOnPhoneGreeting.
ms.openlocfilehash: fd82dc6ef0dd90a2318da93191f657005b7a5c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829450"
---
# <a name="setplayonphonedialstring-um-web-service"></a><span data-ttu-id="e138d-103">SetPlayOnPhoneDialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e138d-103">SetPlayOnPhoneDialString (UM web service)</span></span>

<span data-ttu-id="e138d-104">L’élément **SetPlayOnPhoneDialString** définit une demande pour définir la chaîne de numérotation par défaut pour les demandes [PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) et [les opérations PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="e138d-104">The **SetPlayOnPhoneDialString** element defines a request to set the default dial string for [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) requests.</span></span> 
  
[<span data-ttu-id="e138d-105">SetPlayOnPhoneDialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e138d-105">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 <span data-ttu-id="e138d-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="e138d-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e138d-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e138d-107">Attributes and elements</span></span>

<span data-ttu-id="e138d-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e138d-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e138d-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="e138d-109">Attributes</span></span>

<span data-ttu-id="e138d-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e138d-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e138d-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e138d-111">Child elements</span></span>

|<span data-ttu-id="e138d-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e138d-112">**Element**</span></span>|<span data-ttu-id="e138d-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="e138d-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e138d-114">dialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e138d-114">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="e138d-115">Le numéro de téléphone à définir comme la chaîne de numérotation par défaut.</span><span class="sxs-lookup"><span data-stu-id="e138d-115">The telephone number to set as the default dial string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e138d-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e138d-116">Parent elements</span></span>

<span data-ttu-id="e138d-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e138d-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e138d-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e138d-118">Text value</span></span>

<span data-ttu-id="e138d-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e138d-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e138d-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e138d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e138d-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e138d-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e138d-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e138d-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e138d-123">Messages</span><span class="sxs-lookup"><span data-stu-id="e138d-123">Messages</span></span>  <br/> |
|<span data-ttu-id="e138d-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e138d-124">Validation File</span></span>  <br/> |<span data-ttu-id="e138d-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e138d-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e138d-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e138d-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="e138d-127">False</span><span class="sxs-lookup"><span data-stu-id="e138d-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e138d-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e138d-128">See also</span></span>



[<span data-ttu-id="e138d-129">Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e138d-129">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)

