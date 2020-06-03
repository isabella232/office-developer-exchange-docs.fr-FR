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
description: L’élément UpdateDelegateResponse contient l’État et le résultat d’une demande d’opération UpdateDelegate.
ms.openlocfilehash: 9f11d87ac07dd51a5231d4546fac92e7ca95ad4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465050"
---
# <a name="updatedelegateresponse"></a><span data-ttu-id="175c3-103">UpdateDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="175c3-103">UpdateDelegateResponse</span></span>

<span data-ttu-id="175c3-104">L’élément **UpdateDelegateResponse** contient l’État et le résultat d’une demande d' [opération UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="175c3-104">The **UpdateDelegateResponse** element contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span> 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 <span data-ttu-id="175c3-105">**UpdateDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="175c3-105">**UpdateDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="175c3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="175c3-106">Attributes and elements</span></span>

<span data-ttu-id="175c3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="175c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="175c3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="175c3-108">Attributes</span></span>

<span data-ttu-id="175c3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="175c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="175c3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="175c3-110">Child elements</span></span>

|<span data-ttu-id="175c3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="175c3-111">**Element**</span></span>|<span data-ttu-id="175c3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="175c3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="175c3-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="175c3-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="175c3-114">Contient les messages de réponse pour une demande de gestion des délégués des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="175c3-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="175c3-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="175c3-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="175c3-116">Fournit une description textuelle de l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="175c3-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="175c3-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="175c3-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="175c3-118">Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.</span><span class="sxs-lookup"><span data-stu-id="175c3-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="175c3-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="175c3-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="175c3-120">Actuellement inutilisé et est réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="175c3-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="175c3-121">Il contient une valeur de 0.</span><span class="sxs-lookup"><span data-stu-id="175c3-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="175c3-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="175c3-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="175c3-123">Fournit des informations supplémentaires sur la réponse aux erreurs.</span><span class="sxs-lookup"><span data-stu-id="175c3-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="175c3-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="175c3-124">Parent elements</span></span>

<span data-ttu-id="175c3-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="175c3-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="175c3-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="175c3-126">Remarks</span></span>

<span data-ttu-id="175c3-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="175c3-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="175c3-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="175c3-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="175c3-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="175c3-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="175c3-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="175c3-130">Schema Name</span></span>  <br/> |<span data-ttu-id="175c3-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="175c3-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="175c3-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="175c3-132">Validation File</span></span>  <br/> |<span data-ttu-id="175c3-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="175c3-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="175c3-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="175c3-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="175c3-135">False</span><span class="sxs-lookup"><span data-stu-id="175c3-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="175c3-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="175c3-136">See also</span></span>



[<span data-ttu-id="175c3-137">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="175c3-137">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="175c3-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="175c3-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

