---
title: ArchiveItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 68109a92-c49e-4c0e-b6ec-e90d38d4be4d
description: L’élément ArchiveItemResponse spécifie la réponse à une demande ArchiveItem.
ms.openlocfilehash: 86360846a9a12955e7fa651d5b5027d90b5e56c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463397"
---
# <a name="archiveitemresponse"></a><span data-ttu-id="cc9e9-103">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="cc9e9-103">ArchiveItemResponse</span></span>

<span data-ttu-id="cc9e9-104">L’élément **ArchiveItemResponse** spécifie la réponse à une demande **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="cc9e9-104">The **ArchiveItemResponse** element specifies the response to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponse>
    <ResponseMessages></ResponseMessages>
</ArchiveItemResponse>
```

 <span data-ttu-id="cc9e9-105">**ArchiveItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="cc9e9-105">**ArchiveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc9e9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cc9e9-106">Attributes and elements</span></span>

<span data-ttu-id="cc9e9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cc9e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc9e9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cc9e9-108">Attributes</span></span>

<span data-ttu-id="cc9e9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cc9e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc9e9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cc9e9-110">Child elements</span></span>

|<span data-ttu-id="cc9e9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cc9e9-111">**Element**</span></span>|<span data-ttu-id="cc9e9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cc9e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc9e9-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cc9e9-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="cc9e9-114">Contient les messages de réponse à une demande de services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc9e9-114">Contains the response messages to an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc9e9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cc9e9-115">Parent elements</span></span>

<span data-ttu-id="cc9e9-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cc9e9-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cc9e9-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="cc9e9-117">Remarks</span></span>

<span data-ttu-id="cc9e9-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cc9e9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cc9e9-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc9e9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc9e9-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cc9e9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc9e9-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cc9e9-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc9e9-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cc9e9-122">Schema Name</span></span>  <br/> |<span data-ttu-id="cc9e9-123">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="cc9e9-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="cc9e9-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cc9e9-124">Validation File</span></span>  <br/> |<span data-ttu-id="cc9e9-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cc9e9-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc9e9-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cc9e9-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cc9e9-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cc9e9-127">See also</span></span>

- [<span data-ttu-id="cc9e9-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cc9e9-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

