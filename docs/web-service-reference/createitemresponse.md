---
title: CreateItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponse
api_type:
- schema
ms.assetid: 742a46a0-2475-45a0-b44f-90639a3f5a43
description: L’élément CreateItemResponse définit une réponse à une demande CreateItem.
ms.openlocfilehash: af7349888a2f194a8f4ff1043ec8c38a90b3dfff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458844"
---
# <a name="createitemresponse"></a><span data-ttu-id="28e29-103">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="28e29-103">CreateItemResponse</span></span>

<span data-ttu-id="28e29-104">L’élément **CreateItemResponse** définit une réponse à une demande CreateItem.</span><span class="sxs-lookup"><span data-stu-id="28e29-104">The **CreateItemResponse** element defines a response to a CreateItem request.</span></span> 
  
```xml
<CreateItemResponse>
   <ResponseMessages/>
</CreateItemResponse>
```

 <span data-ttu-id="28e29-105">**CreateItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="28e29-105">**CreateItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28e29-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28e29-106">Attributes and elements</span></span>

<span data-ttu-id="28e29-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28e29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28e29-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="28e29-108">Attributes</span></span>

<span data-ttu-id="28e29-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="28e29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28e29-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28e29-110">Child elements</span></span>

|<span data-ttu-id="28e29-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28e29-111">**Element**</span></span>|<span data-ttu-id="28e29-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="28e29-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28e29-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="28e29-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="28e29-114">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="28e29-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28e29-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28e29-115">Parent elements</span></span>

<span data-ttu-id="28e29-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28e29-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28e29-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="28e29-117">Remarks</span></span>

<span data-ttu-id="28e29-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="28e29-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28e29-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28e29-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28e29-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28e29-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28e29-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28e29-121">Schema name</span></span>  <br/> |<span data-ttu-id="28e29-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="28e29-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28e29-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28e29-123">Validation file</span></span>  <br/> |<span data-ttu-id="28e29-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="28e29-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28e29-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28e29-125">Can be empty</span></span>  <br/> |<span data-ttu-id="28e29-126">False</span><span class="sxs-lookup"><span data-stu-id="28e29-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28e29-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28e29-127">See also</span></span>



[<span data-ttu-id="28e29-128">Opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="28e29-128">CreateItem operation</span></span>](createitem-operation.md)
  
[<span data-ttu-id="28e29-129">CreateItem</span><span class="sxs-lookup"><span data-stu-id="28e29-129">CreateItem</span></span>](createitem.md)


- [<span data-ttu-id="28e29-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="28e29-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

