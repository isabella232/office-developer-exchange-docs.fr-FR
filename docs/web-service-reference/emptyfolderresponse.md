---
title: EmptyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c900be49-3c90-41aa-aba5-bcf1116ec2aa
description: L’élément EmptyFolderResponse définit une réponse à une demande d’opération EmptyFolder.
ms.openlocfilehash: ab753351a1eb7deba83823875989816ba75b9809
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756151"
---
# <a name="emptyfolderresponse"></a><span data-ttu-id="d3ec4-103">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d3ec4-103">EmptyFolderResponse</span></span>

<span data-ttu-id="d3ec4-104">L’élément **EmptyFolderResponse** définit une réponse à une demande [d’opération EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d3ec4-104">The **EmptyFolderResponse** element defines a response to an [EmptyFolder operation](emptyfolder-operation.md) request.</span></span> 
  
```XML
<EmptyFolderResponse>
   <ResponseMessages/>
</EmptyFolderResponse>
```

 <span data-ttu-id="d3ec4-105">**EmptyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="d3ec4-105">**EmptyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3ec4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3ec4-106">Attributes and elements</span></span>

<span data-ttu-id="d3ec4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3ec4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3ec4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3ec4-108">Attributes</span></span>

<span data-ttu-id="d3ec4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3ec4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3ec4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3ec4-110">Child elements</span></span>

|<span data-ttu-id="d3ec4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3ec4-111">**Element**</span></span>|<span data-ttu-id="d3ec4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3ec4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3ec4-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3ec4-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d3ec4-114">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3ec4-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3ec4-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3ec4-115">Parent elements</span></span>

<span data-ttu-id="d3ec4-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3ec4-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3ec4-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="d3ec4-117">Remarks</span></span>

<span data-ttu-id="d3ec4-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3ec4-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3ec4-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d3ec4-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3ec4-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d3ec4-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3ec4-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d3ec4-121">Schema name</span></span>  <br/> |<span data-ttu-id="d3ec4-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d3ec4-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d3ec4-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d3ec4-123">Validation file</span></span>  <br/> |<span data-ttu-id="d3ec4-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d3ec4-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3ec4-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d3ec4-125">Can be empty</span></span>  <br/> |<span data-ttu-id="d3ec4-126">False</span><span class="sxs-lookup"><span data-stu-id="d3ec4-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3ec4-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3ec4-127">See also</span></span>



[<span data-ttu-id="d3ec4-128">Opération EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="d3ec4-128">EmptyFolder operation</span></span>](emptyfolder-operation.md)
  
[<span data-ttu-id="d3ec4-129">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="d3ec4-129">EmptyFolder</span></span>](emptyfolder.md)


- [<span data-ttu-id="d3ec4-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d3ec4-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

