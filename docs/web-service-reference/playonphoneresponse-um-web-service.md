---
title: PlayOnPhoneResponse (service Web de messagerie unifiée)
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
description: L’élément PlayOnPhoneResponse définit une réponse à une opération PlayOnPhone (service Web de messagerie unifiée).
ms.openlocfilehash: ddb9cc9a8feaeb476e6502339fdc74d024797b9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459615"
---
# <a name="playonphoneresponse-um-web-service"></a><span data-ttu-id="5a942-103">PlayOnPhoneResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5a942-103">PlayOnPhoneResponse (UM web service)</span></span>

<span data-ttu-id="5a942-104">L’élément **PlayOnPhoneResponse** définit une réponse à une [opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="5a942-104">The **PlayOnPhoneResponse** element defines a response to a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="5a942-105">PlayOnPhoneResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5a942-105">PlayOnPhoneResponse (UM web service)</span></span>](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 <span data-ttu-id="5a942-106">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="5a942-106">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a942-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5a942-107">Attributes and elements</span></span>

<span data-ttu-id="5a942-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5a942-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a942-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="5a942-109">Attributes</span></span>

<span data-ttu-id="5a942-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5a942-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a942-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5a942-111">Child elements</span></span>

<span data-ttu-id="5a942-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5a942-112">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a942-113">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5a942-113">Parent elements</span></span>

<span data-ttu-id="5a942-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5a942-114">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5a942-115">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5a942-115">Text value</span></span>

<span data-ttu-id="5a942-116">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="5a942-116">A text value is required.</span></span> <span data-ttu-id="5a942-117">La valeur de texte est l’identificateur d’appel à utiliser pour la valeur de [CallId (service Web de messagerie unifiée)](callid-um-web-service.md) dans une demande [GetCallInfo Operation (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) ou une [opération de déconnexion (service Web de messagerie unifiée](disconnect-operation-um-web-service.md) ).</span><span class="sxs-lookup"><span data-stu-id="5a942-117">The text value is the call identifier to use for the value of [CallId (UM web service)](callid-um-web-service.md) in a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request or a [Disconnect operation (UM web service)](disconnect-operation-um-web-service.md) request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5a942-118">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5a942-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a942-119">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5a942-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5a942-120">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5a942-120">Schema Name</span></span>  <br/> |<span data-ttu-id="5a942-121">Messages</span><span class="sxs-lookup"><span data-stu-id="5a942-121">Messages</span></span>  <br/> |
|<span data-ttu-id="5a942-122">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5a942-122">Validation File</span></span>  <br/> |<span data-ttu-id="5a942-123">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5a942-123">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5a942-124">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5a942-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a942-125">False</span><span class="sxs-lookup"><span data-stu-id="5a942-125">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a942-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5a942-126">See also</span></span>



[<span data-ttu-id="5a942-127">Opération PlayOnPhone (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5a942-127">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

