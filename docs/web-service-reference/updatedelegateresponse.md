---
title: UpdateDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegateResponse
api_type:
- schema
ms.assetid: cd336add-fbcc-4f61-9867-d4c08a60e142
description: L’élément UpdateDelegateResponse contient l’état et les résultats d’une requête d’opération UpdateDelegate.
ms.openlocfilehash: b90dd7d8011cf75831481b8f2b92df80d9a67d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838846"
---
# <a name="updatedelegateresponse"></a><span data-ttu-id="65592-103">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="65592-103">UpdateDelegateResponse</span></span>

<span data-ttu-id="65592-104">L’élément **UpdateDelegateResponse** contient l’état et les résultats d’une requête [d’opération UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65592-104">The **UpdateDelegateResponse** element contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span> 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 <span data-ttu-id="65592-105">**UpdateDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="65592-105">**UpdateDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65592-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65592-106">Attributes and elements</span></span>

<span data-ttu-id="65592-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65592-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65592-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="65592-108">Attributes</span></span>

<span data-ttu-id="65592-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65592-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65592-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65592-110">Child elements</span></span>

|<span data-ttu-id="65592-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65592-111">**Element**</span></span>|<span data-ttu-id="65592-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="65592-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65592-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="65592-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="65592-114">Contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.</span><span class="sxs-lookup"><span data-stu-id="65592-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="65592-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="65592-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="65592-116">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="65592-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="65592-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="65592-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="65592-118">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="65592-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="65592-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="65592-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="65592-120">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="65592-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="65592-121">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="65592-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="65592-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="65592-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="65592-123">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="65592-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65592-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65592-124">Parent elements</span></span>

<span data-ttu-id="65592-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65592-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="65592-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="65592-126">Remarks</span></span>

<span data-ttu-id="65592-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="65592-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65592-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65592-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65592-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65592-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65592-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65592-130">Schema Name</span></span>  <br/> |<span data-ttu-id="65592-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="65592-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="65592-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65592-132">Validation File</span></span>  <br/> |<span data-ttu-id="65592-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="65592-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65592-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65592-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="65592-135">False</span><span class="sxs-lookup"><span data-stu-id="65592-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65592-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65592-136">See also</span></span>



[<span data-ttu-id="65592-137">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="65592-137">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="65592-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="65592-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

