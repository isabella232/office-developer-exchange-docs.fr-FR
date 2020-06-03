---
title: PlayOnPhoneGreeting (service Web de messagerie unifiée)
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
description: L’élément PlayOnPhoneGreeting définit une demande de lecture d’un message d’accueil de la messagerie unifiée sur un téléphone.
ms.openlocfilehash: 197e4ba671e1711b73b1e7c239339db589357581
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529923"
---
# <a name="playonphonegreeting-um-web-service"></a><span data-ttu-id="0e16b-103">PlayOnPhoneGreeting (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0e16b-103">PlayOnPhoneGreeting (UM web service)</span></span>

<span data-ttu-id="0e16b-104">L’élément **PlayOnPhoneGreeting** définit une demande de lecture d’un message d’accueil de la messagerie unifiée sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="0e16b-104">The **PlayOnPhoneGreeting** element defines a request to play a Unified Messaging greeting on a telephone.</span></span> 
  
[<span data-ttu-id="0e16b-105">PlayOnPhoneGreeting (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0e16b-105">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 <span data-ttu-id="0e16b-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="0e16b-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e16b-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0e16b-107">Attributes and elements</span></span>

<span data-ttu-id="0e16b-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0e16b-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e16b-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="0e16b-109">Attributes</span></span>

<span data-ttu-id="0e16b-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0e16b-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e16b-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0e16b-111">Child elements</span></span>

|<span data-ttu-id="0e16b-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0e16b-112">**Element**</span></span>|<span data-ttu-id="0e16b-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="0e16b-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e16b-114">GreetingType (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0e16b-114">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md) <br/> |<span data-ttu-id="0e16b-115">Définit le type de message d’accueil à utiliser dans une demande d' [opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="0e16b-115">Defines the type of greeting to use in a [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0e16b-116">dialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0e16b-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="0e16b-117">Contient la valeur du numéro de téléphone à composer.</span><span class="sxs-lookup"><span data-stu-id="0e16b-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0e16b-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0e16b-118">Parent elements</span></span>

<span data-ttu-id="0e16b-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0e16b-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0e16b-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0e16b-120">Text value</span></span>

<span data-ttu-id="0e16b-121">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0e16b-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e16b-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0e16b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e16b-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0e16b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0e16b-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0e16b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0e16b-125">Messages</span><span class="sxs-lookup"><span data-stu-id="0e16b-125">Messages</span></span>  <br/> |
|<span data-ttu-id="0e16b-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0e16b-126">Validation File</span></span>  <br/> |<span data-ttu-id="0e16b-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0e16b-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0e16b-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0e16b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e16b-129">False</span><span class="sxs-lookup"><span data-stu-id="0e16b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e16b-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0e16b-130">See also</span></span>



[<span data-ttu-id="0e16b-131">Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0e16b-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

