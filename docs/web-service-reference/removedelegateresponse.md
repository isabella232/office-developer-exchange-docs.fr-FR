---
title: RemoveDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegateResponse
api_type:
- schema
ms.assetid: eef56c53-d0a7-4342-9ce6-4dbb6b1a1369
description: L’élément RemoveDelegateResponse contient l’État et le résultat d’une demande d’opération RemoveDelegate.
ms.openlocfilehash: 4c7a8b81528435b72576c116bc97f611544c24d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468935"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="33ca1-103">RemoveDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="33ca1-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="33ca1-104">L’élément **RemoveDelegateResponse** contient l’État et le résultat d’une demande d' [opération RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="33ca1-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="33ca1-105">**RemoveDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="33ca1-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33ca1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="33ca1-106">Attributes and elements</span></span>

<span data-ttu-id="33ca1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="33ca1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33ca1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="33ca1-108">Attributes</span></span>

<span data-ttu-id="33ca1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="33ca1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33ca1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="33ca1-110">Child elements</span></span>

|<span data-ttu-id="33ca1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="33ca1-111">**Element**</span></span>|<span data-ttu-id="33ca1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="33ca1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33ca1-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="33ca1-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="33ca1-114">Contient les messages de réponse pour une demande de gestion des délégués des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="33ca1-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="33ca1-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="33ca1-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="33ca1-116">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="33ca1-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="33ca1-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="33ca1-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="33ca1-118">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="33ca1-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="33ca1-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="33ca1-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="33ca1-120">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="33ca1-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="33ca1-121">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="33ca1-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="33ca1-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="33ca1-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="33ca1-123">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="33ca1-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33ca1-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="33ca1-124">Parent elements</span></span>

<span data-ttu-id="33ca1-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="33ca1-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33ca1-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="33ca1-126">Remarks</span></span>

<span data-ttu-id="33ca1-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="33ca1-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33ca1-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="33ca1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33ca1-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="33ca1-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33ca1-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="33ca1-130">Schema Name</span></span>  <br/> |<span data-ttu-id="33ca1-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="33ca1-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="33ca1-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="33ca1-132">Validation File</span></span>  <br/> |<span data-ttu-id="33ca1-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="33ca1-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33ca1-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="33ca1-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="33ca1-135">False</span><span class="sxs-lookup"><span data-stu-id="33ca1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33ca1-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="33ca1-136">See also</span></span>



[<span data-ttu-id="33ca1-137">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="33ca1-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="33ca1-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="33ca1-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

