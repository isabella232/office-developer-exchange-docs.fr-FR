---
title: GetAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachmentResponse
api_type:
- schema
ms.assetid: cb65f449-309b-4b6e-8d22-d1967135490c
description: L’élément GetAttachmentResponse définit une réponse à une demande GetAttachment.
ms.openlocfilehash: 05a9e84236c791dcec99182dfca0352e44efca46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756526"
---
# <a name="getattachmentresponse"></a><span data-ttu-id="33729-103">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="33729-103">GetAttachmentResponse</span></span>

<span data-ttu-id="33729-104">L’élément **GetAttachmentResponse** définit une réponse à une demande GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="33729-104">The **GetAttachmentResponse** element defines a response to a GetAttachment request.</span></span> 
  
```xml
<GetAttachmentResponse>
   <ResponseMessages/>
</GetAttachmentResponse>
```

 <span data-ttu-id="33729-105">**GetAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="33729-105">**GetAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33729-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="33729-106">Attributes and elements</span></span>

<span data-ttu-id="33729-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="33729-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33729-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="33729-108">Attributes</span></span>

<span data-ttu-id="33729-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="33729-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33729-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="33729-110">Child elements</span></span>

|<span data-ttu-id="33729-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="33729-111">**Element**</span></span>|<span data-ttu-id="33729-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="33729-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33729-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="33729-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="33729-114">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="33729-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33729-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="33729-115">Parent elements</span></span>

<span data-ttu-id="33729-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="33729-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33729-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="33729-117">Remarks</span></span>

<span data-ttu-id="33729-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="33729-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33729-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="33729-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33729-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="33729-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33729-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="33729-121">Schema name</span></span>  <br/> |<span data-ttu-id="33729-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="33729-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="33729-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="33729-123">Validation file</span></span>  <br/> |<span data-ttu-id="33729-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33729-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33729-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="33729-125">Can be empty</span></span>  <br/> |<span data-ttu-id="33729-126">False</span><span class="sxs-lookup"><span data-stu-id="33729-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33729-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="33729-127">See also</span></span>



[<span data-ttu-id="33729-128">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="33729-128">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="33729-129">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="33729-129">GetAttachment</span></span>](getattachment.md)

