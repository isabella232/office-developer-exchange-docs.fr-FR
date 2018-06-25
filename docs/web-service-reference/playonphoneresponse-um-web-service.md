---
title: PlayOnPhoneResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: L’élément PlayOnPhoneResponse définit une réponse à une demande de (service web de messagerie unifiée) opération PlayOnPhone.
ms.openlocfilehash: 482739d924bbac1d58624e50596af48cc405a3ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828832"
---
# <a name="playonphoneresponse-um-web-service"></a><span data-ttu-id="9b927-103">PlayOnPhoneResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="9b927-103">PlayOnPhoneResponse (UM web service)</span></span>

<span data-ttu-id="9b927-104">L’élément **PlayOnPhoneResponse** définit une réponse à une demande de [l’opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="9b927-104">The **PlayOnPhoneResponse** element defines a response to a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="9b927-105">PlayOnPhoneResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="9b927-105">PlayOnPhoneResponse (UM web service)</span></span>](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 <span data-ttu-id="9b927-106">**string**</span><span class="sxs-lookup"><span data-stu-id="9b927-106">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b927-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9b927-107">Attributes and elements</span></span>

<span data-ttu-id="9b927-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9b927-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b927-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="9b927-109">Attributes</span></span>

<span data-ttu-id="9b927-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b927-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b927-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9b927-111">Child elements</span></span>

<span data-ttu-id="9b927-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b927-112">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b927-113">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9b927-113">Parent elements</span></span>

<span data-ttu-id="9b927-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b927-114">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9b927-115">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9b927-115">Text value</span></span>

<span data-ttu-id="9b927-116">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="9b927-116">A text value is required.</span></span> <span data-ttu-id="9b927-117">La valeur de text est l’identificateur d’appel à utiliser pour la valeur de [l’ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md) dans une requête [d’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) ou une [opération de déconnexion (service web de messagerie unifiée)](disconnect-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="9b927-117">The text value is the call identifier to use for the value of [CallId (UM web service)](callid-um-web-service.md) in a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request or a [Disconnect operation (UM web service)](disconnect-operation-um-web-service.md) request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9b927-118">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9b927-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b927-119">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9b927-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9b927-120">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9b927-120">Schema Name</span></span>  <br/> |<span data-ttu-id="9b927-121">Messages</span><span class="sxs-lookup"><span data-stu-id="9b927-121">Messages</span></span>  <br/> |
|<span data-ttu-id="9b927-122">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9b927-122">Validation File</span></span>  <br/> |<span data-ttu-id="9b927-123">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9b927-123">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9b927-124">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9b927-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="9b927-125">False</span><span class="sxs-lookup"><span data-stu-id="9b927-125">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b927-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9b927-126">See also</span></span>



[<span data-ttu-id="9b927-127">Opération PlayOnPhone (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="9b927-127">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

