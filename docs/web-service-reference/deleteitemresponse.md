---
title: Updateitemresponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponse
api_type:
- schema
ms.assetid: 86463d66-fe47-4a19-a81b-e24841e816ab
description: L’élément Updateitemresponse définit une réponse à une seule demande DeleteItem.
ms.openlocfilehash: 6aad30077e8867486012dd34bb1def97accffc2b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529195"
---
# <a name="deleteitemresponse"></a><span data-ttu-id="f7350-103">Updateitemresponse</span><span class="sxs-lookup"><span data-stu-id="f7350-103">DeleteItemResponse</span></span>

<span data-ttu-id="f7350-104">L’élément **updateitemresponse** définit une réponse à une seule demande DeleteItem.</span><span class="sxs-lookup"><span data-stu-id="f7350-104">The **DeleteItemResponse** element defines a response to a single DeleteItem request.</span></span> 
  
```xml
<DeleteItemResponse>
   <ResponseMessages/>
</DeleteItemResponse>
```

 <span data-ttu-id="f7350-105">**DeleteItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="f7350-105">**DeleteItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7350-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7350-106">Attributes and elements</span></span>

<span data-ttu-id="f7350-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7350-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7350-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7350-108">Attributes</span></span>

<span data-ttu-id="f7350-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f7350-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7350-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7350-110">Child elements</span></span>

|<span data-ttu-id="f7350-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7350-111">**Element**</span></span>|<span data-ttu-id="f7350-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7350-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7350-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f7350-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f7350-114">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7350-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7350-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7350-115">Parent elements</span></span>

<span data-ttu-id="f7350-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7350-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7350-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7350-117">Remarks</span></span>

<span data-ttu-id="f7350-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f7350-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7350-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7350-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7350-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7350-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f7350-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7350-121">Schema Name</span></span>  <br/> |<span data-ttu-id="f7350-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f7350-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f7350-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7350-123">Validation File</span></span>  <br/> |<span data-ttu-id="f7350-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f7350-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7350-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7350-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7350-126">False</span><span class="sxs-lookup"><span data-stu-id="f7350-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7350-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7350-127">See also</span></span>

- [<span data-ttu-id="f7350-128">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="f7350-128">DeleteItem operation</span></span>](deleteitem-operation.md)  
- [<span data-ttu-id="f7350-129">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="f7350-129">DeleteItem</span></span>](deleteitem.md)
- [<span data-ttu-id="f7350-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f7350-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

