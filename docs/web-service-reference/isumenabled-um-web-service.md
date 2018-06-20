---
title: IsUMEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: L’élément IsUMEnabled indique si une boîte aux lettres est activé pour la messagerie unifiée.
ms.openlocfilehash: 5f4d59c5497158e5afbc8bb5db4900bd129df50b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828113"
---
# <a name="isumenabled-um-web-service"></a><span data-ttu-id="08e05-103">IsUMEnabled (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="08e05-103">IsUMEnabled (UM web service)</span></span>

<span data-ttu-id="08e05-104">L’élément **IsUMEnabled** indique si une boîte aux lettres est activé pour la messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="08e05-104">The **IsUMEnabled** element indicates whether a mailbox is enabled for Unified Messaging.</span></span> 
  
```xml
<IsUMEnabled/>
```

 <span data-ttu-id="08e05-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="08e05-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08e05-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08e05-106">Attributes and elements</span></span>

<span data-ttu-id="08e05-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08e05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08e05-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="08e05-108">Attributes</span></span>

<span data-ttu-id="08e05-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08e05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08e05-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08e05-110">Child elements</span></span>

<span data-ttu-id="08e05-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08e05-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08e05-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08e05-112">Parent elements</span></span>

<span data-ttu-id="08e05-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08e05-113">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="08e05-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="08e05-114">Text value</span></span>

<span data-ttu-id="08e05-115">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="08e05-115">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="08e05-116">La valeur **true** indique que la boîte aux lettres est activé pour la messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="08e05-116">A value of **true** indicates that the mailbox is enabled for Unified Messaging.</span></span> <span data-ttu-id="08e05-117">La valeur **false** signifie que la boîte aux lettres n’est pas activé pour la messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="08e05-117">A value of **false** means that the mailbox is not enabled for Unified Messaging.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="08e05-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="08e05-118">Remarks</span></span>

<span data-ttu-id="08e05-119">Pour déterminer si une boîte aux lettres est activée pour la messagerie unifiée, utilisez l' [opération IsUMEnabled (service web de messagerie unifiée)](isumenabled-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="08e05-119">To determine whether a mailbox is enabled for Unified Messaging, use the [IsUMEnabled operation (UM web service)](isumenabled-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08e05-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="08e05-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08e05-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="08e05-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="08e05-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="08e05-122">Schema Name</span></span>  <br/> |<span data-ttu-id="08e05-123">Messages</span><span class="sxs-lookup"><span data-stu-id="08e05-123">Messages</span></span>  <br/> |
|<span data-ttu-id="08e05-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="08e05-124">Validation File</span></span>  <br/> |<span data-ttu-id="08e05-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="08e05-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08e05-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="08e05-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="08e05-127">False</span><span class="sxs-lookup"><span data-stu-id="08e05-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08e05-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08e05-128">See also</span></span>



[<span data-ttu-id="08e05-129">Opération IsUMEnabled (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="08e05-129">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)


[<span data-ttu-id="08e05-130">Unified Messaging service XML des éléments web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="08e05-130">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

