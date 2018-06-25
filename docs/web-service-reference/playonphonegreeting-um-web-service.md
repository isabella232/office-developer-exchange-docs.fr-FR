---
title: PlayOnPhoneGreeting (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: L’élément PlayOnPhoneGreeting définit une demande pour lire une messagerie unifiée message d’accueil sur un téléphone.
ms.openlocfilehash: c30140fc60b9e902517b4cc18deb9b61efa61e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828836"
---
# <a name="playonphonegreeting-um-web-service"></a><span data-ttu-id="59f67-103">PlayOnPhoneGreeting (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="59f67-103">PlayOnPhoneGreeting (UM web service)</span></span>

<span data-ttu-id="59f67-104">L’élément **PlayOnPhoneGreeting** définit une demande pour lire une messagerie unifiée message d’accueil sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="59f67-104">The **PlayOnPhoneGreeting** element defines a request to play a Unified Messaging greeting on a telephone.</span></span> 
  
[<span data-ttu-id="59f67-105">PlayOnPhoneGreeting (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="59f67-105">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 <span data-ttu-id="59f67-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="59f67-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59f67-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59f67-107">Attributes and elements</span></span>

<span data-ttu-id="59f67-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59f67-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59f67-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="59f67-109">Attributes</span></span>

<span data-ttu-id="59f67-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59f67-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59f67-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59f67-111">Child elements</span></span>

|<span data-ttu-id="59f67-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59f67-112">**Element**</span></span>|<span data-ttu-id="59f67-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="59f67-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59f67-114">GreetingType (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="59f67-114">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md) <br/> |<span data-ttu-id="59f67-115">Définit le type de message d’accueil à utiliser dans une requête [d’opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="59f67-115">Defines the type of greeting to use in a [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="59f67-116">dialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="59f67-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="59f67-117">Contient la valeur du numéro de téléphone à composer.</span><span class="sxs-lookup"><span data-stu-id="59f67-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59f67-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59f67-118">Parent elements</span></span>

<span data-ttu-id="59f67-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59f67-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="59f67-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="59f67-120">Text value</span></span>

<span data-ttu-id="59f67-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59f67-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59f67-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59f67-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59f67-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59f67-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59f67-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59f67-124">Schema Name</span></span>  <br/> |<span data-ttu-id="59f67-125">Messages</span><span class="sxs-lookup"><span data-stu-id="59f67-125">Messages</span></span>  <br/> |
|<span data-ttu-id="59f67-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59f67-126">Validation File</span></span>  <br/> |<span data-ttu-id="59f67-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="59f67-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59f67-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59f67-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="59f67-129">False</span><span class="sxs-lookup"><span data-stu-id="59f67-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59f67-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59f67-130">See also</span></span>



[<span data-ttu-id="59f67-131">Opération PlayOnPhoneGreeting (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="59f67-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

