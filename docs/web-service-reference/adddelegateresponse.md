---
title: AddDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegateResponse
api_type:
- schema
ms.assetid: d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429
description: L’élément AddDelegateResponse contient l’état et les résultats d’une requête d’opération AddDelegate.
ms.openlocfilehash: a1d56e9994b3a7916fe0fbe40be1e6d8ff473730
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755160"
---
# <a name="adddelegateresponse"></a><span data-ttu-id="b1c57-103">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="b1c57-103">AddDelegateResponse</span></span>

<span data-ttu-id="b1c57-104">L’élément **AddDelegateResponse** contient l’état et les résultats d’une requête [d’opération AddDelegate](adddelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b1c57-104">The **AddDelegateResponse** element contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span> 
  
```xml
<AddDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddDelegateResponse>
```

 <span data-ttu-id="b1c57-105">**AddDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b1c57-105">**AddDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1c57-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b1c57-106">Attributes and elements</span></span>

<span data-ttu-id="b1c57-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b1c57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1c57-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b1c57-108">Attributes</span></span>

<span data-ttu-id="b1c57-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b1c57-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1c57-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b1c57-110">Child elements</span></span>

|<span data-ttu-id="b1c57-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b1c57-111">**Element**</span></span>|<span data-ttu-id="b1c57-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1c57-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1c57-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="b1c57-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="b1c57-114">Contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.</span><span class="sxs-lookup"><span data-stu-id="b1c57-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="b1c57-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="b1c57-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b1c57-116">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="b1c57-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b1c57-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b1c57-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b1c57-118">Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.</span><span class="sxs-lookup"><span data-stu-id="b1c57-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b1c57-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b1c57-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b1c57-120">Actuellement inutilisés et est réservé à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="b1c57-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b1c57-121">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="b1c57-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b1c57-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b1c57-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b1c57-123">Fournit des informations de réponse d’erreur.</span><span class="sxs-lookup"><span data-stu-id="b1c57-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b1c57-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b1c57-124">Parent elements</span></span>

<span data-ttu-id="b1c57-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b1c57-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b1c57-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="b1c57-126">Remarks</span></span>

<span data-ttu-id="b1c57-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="b1c57-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1c57-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b1c57-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1c57-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b1c57-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b1c57-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b1c57-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b1c57-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b1c57-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b1c57-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b1c57-132">Validation File</span></span>  <br/> |<span data-ttu-id="b1c57-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b1c57-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b1c57-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b1c57-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b1c57-135">False</span><span class="sxs-lookup"><span data-stu-id="b1c57-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b1c57-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b1c57-136">See also</span></span>

- [<span data-ttu-id="b1c57-137">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="b1c57-137">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="b1c57-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b1c57-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="b1c57-139">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="b1c57-139">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

