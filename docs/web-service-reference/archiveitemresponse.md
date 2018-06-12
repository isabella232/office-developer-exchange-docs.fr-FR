---
title: ArchiveItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 68109a92-c49e-4c0e-b6ec-e90d38d4be4d
description: L’élément ArchiveItemResponse spécifie la réponse à une demande de ArchiveItem.
ms.openlocfilehash: bfd1b9d76c2b49e00a82bd8f6f57742007d0adf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755315"
---
# <a name="archiveitemresponse"></a><span data-ttu-id="ce39e-103">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="ce39e-103">ArchiveItemResponse</span></span>

<span data-ttu-id="ce39e-104">L’élément **ArchiveItemResponse** spécifie la réponse à une demande de **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="ce39e-104">The **ArchiveItemResponse** element specifies the response to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponse>
    <ResponseMessages></ResponseMessages>
</ArchiveItemResponse>
```

 <span data-ttu-id="ce39e-105">**ArchiveItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="ce39e-105">**ArchiveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce39e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ce39e-106">Attributes and elements</span></span>

<span data-ttu-id="ce39e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ce39e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce39e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ce39e-108">Attributes</span></span>

<span data-ttu-id="ce39e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ce39e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce39e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ce39e-110">Child elements</span></span>

|<span data-ttu-id="ce39e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce39e-111">**Element**</span></span>|<span data-ttu-id="ce39e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce39e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce39e-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce39e-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ce39e-114">Contient les messages de réponse à une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce39e-114">Contains the response messages to an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce39e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ce39e-115">Parent elements</span></span>

<span data-ttu-id="ce39e-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ce39e-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ce39e-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="ce39e-117">Remarks</span></span>

<span data-ttu-id="ce39e-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ce39e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ce39e-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce39e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce39e-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ce39e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce39e-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ce39e-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ce39e-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ce39e-122">Schema Name</span></span>  <br/> |<span data-ttu-id="ce39e-123">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="ce39e-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="ce39e-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ce39e-124">Validation File</span></span>  <br/> |<span data-ttu-id="ce39e-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ce39e-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce39e-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ce39e-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ce39e-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ce39e-127">See also</span></span>

- [<span data-ttu-id="ce39e-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ce39e-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

