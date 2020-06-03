---
title: SetPlayOnPhoneDialString (service Web de messagerie unifiée)
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
description: L’élément SetPlayOnPhoneDialString définit une demande de définition de la chaîne de numérotation par défaut pour les opérations PlayOnPhone (service Web de messagerie unifiée) et PlayOnPhoneGreeting (service Web de messagerie unifiée).
ms.openlocfilehash: 40021e9dedafb5fafda91bf3612d8a6485dae8e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458627"
---
# <a name="setplayonphonedialstring-um-web-service"></a><span data-ttu-id="a1c56-103">SetPlayOnPhoneDialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a1c56-103">SetPlayOnPhoneDialString (UM web service)</span></span>

<span data-ttu-id="a1c56-104">L’élément **SetPlayOnPhoneDialString** définit une demande de définition de la chaîne de numérotation par défaut pour les [opérations PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) et [PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="a1c56-104">The **SetPlayOnPhoneDialString** element defines a request to set the default dial string for [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) requests.</span></span> 
  
[<span data-ttu-id="a1c56-105">SetPlayOnPhoneDialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a1c56-105">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 <span data-ttu-id="a1c56-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="a1c56-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1c56-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a1c56-107">Attributes and elements</span></span>

<span data-ttu-id="a1c56-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a1c56-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1c56-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="a1c56-109">Attributes</span></span>

<span data-ttu-id="a1c56-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a1c56-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1c56-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a1c56-111">Child elements</span></span>

|<span data-ttu-id="a1c56-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a1c56-112">**Element**</span></span>|<span data-ttu-id="a1c56-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="a1c56-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1c56-114">dialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a1c56-114">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="a1c56-115">Numéro de téléphone à définir comme chaîne de numérotation par défaut.</span><span class="sxs-lookup"><span data-stu-id="a1c56-115">The telephone number to set as the default dial string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1c56-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a1c56-116">Parent elements</span></span>

<span data-ttu-id="a1c56-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a1c56-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a1c56-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a1c56-118">Text value</span></span>

<span data-ttu-id="a1c56-119">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a1c56-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1c56-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a1c56-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1c56-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a1c56-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1c56-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a1c56-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a1c56-123">Messages</span><span class="sxs-lookup"><span data-stu-id="a1c56-123">Messages</span></span>  <br/> |
|<span data-ttu-id="a1c56-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a1c56-124">Validation File</span></span>  <br/> |<span data-ttu-id="a1c56-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a1c56-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1c56-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a1c56-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1c56-127">False</span><span class="sxs-lookup"><span data-stu-id="a1c56-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1c56-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a1c56-128">See also</span></span>



[<span data-ttu-id="a1c56-129">Opération SetPlayOnPhoneDialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="a1c56-129">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)

