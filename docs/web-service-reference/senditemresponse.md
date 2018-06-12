---
title: SendItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponse
api_type:
- schema
ms.assetid: 26ac41c7-57d9-473e-ab7a-bae93e1d2aba
description: L’élément SendItemResponse définit une réponse à une demande SendItem.
ms.openlocfilehash: 41f450e1d4c95f7ba389adcaa2ed7e18ea74d61c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829339"
---
# <a name="senditemresponse"></a><span data-ttu-id="298a5-103">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="298a5-103">SendItemResponse</span></span>

<span data-ttu-id="298a5-104">L’élément **SendItemResponse** définit une réponse à une demande SendItem.</span><span class="sxs-lookup"><span data-stu-id="298a5-104">The **SendItemResponse** element defines a response to a SendItem request.</span></span> 
  
```xml
<SendItemResponse>
   <ResponseMessages/>
</SendItemResponse>
```

 <span data-ttu-id="298a5-105">**SendItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="298a5-105">**SendItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="298a5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="298a5-106">Attributes and elements</span></span>

<span data-ttu-id="298a5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="298a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="298a5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="298a5-108">Attributes</span></span>

<span data-ttu-id="298a5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="298a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="298a5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="298a5-110">Child elements</span></span>

|<span data-ttu-id="298a5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="298a5-111">**Element**</span></span>|<span data-ttu-id="298a5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="298a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="298a5-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="298a5-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="298a5-114">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="298a5-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="298a5-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="298a5-115">Parent elements</span></span>

<span data-ttu-id="298a5-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="298a5-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="298a5-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="298a5-117">Remarks</span></span>

<span data-ttu-id="298a5-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="298a5-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="298a5-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="298a5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="298a5-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="298a5-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="298a5-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="298a5-121">Schema name</span></span>  <br/> |<span data-ttu-id="298a5-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="298a5-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="298a5-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="298a5-123">Validation file</span></span>  <br/> |<span data-ttu-id="298a5-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="298a5-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="298a5-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="298a5-125">Can be empty</span></span>  <br/> |<span data-ttu-id="298a5-126">False</span><span class="sxs-lookup"><span data-stu-id="298a5-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="298a5-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="298a5-127">See also</span></span>



[<span data-ttu-id="298a5-128">Opération SendItem</span><span class="sxs-lookup"><span data-stu-id="298a5-128">SendItem operation</span></span>](senditem-operation.md)
  
[<span data-ttu-id="298a5-129">SendItem</span><span class="sxs-lookup"><span data-stu-id="298a5-129">SendItem</span></span>](senditem.md)


- [<span data-ttu-id="298a5-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="298a5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

