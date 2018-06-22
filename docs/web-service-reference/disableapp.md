---
title: DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 42d2a888-fa62-4970-8306-9ddde4eeb1f0
description: L’élément DisableApp spécifie une demande pour désactiver une application.
ms.openlocfilehash: d6d895d98fb368a6912f9111a4b934ba9631268e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755938"
---
# <a name="disableapp"></a><span data-ttu-id="f549f-103">DisableApp</span><span class="sxs-lookup"><span data-stu-id="f549f-103">DisableApp</span></span>

<span data-ttu-id="f549f-104">L’élément **DisableApp** spécifie une demande pour désactiver une application.</span><span class="sxs-lookup"><span data-stu-id="f549f-104">The **DisableApp** element specifies a request to disable an app.</span></span> 
  
```XML
<DisableApp>
    <ID></ID>
    <DisableReason></DisableReason>
</DisableApp>
```

 <span data-ttu-id="f549f-105">**DisableAppType**</span><span class="sxs-lookup"><span data-stu-id="f549f-105">**DisableAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f549f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f549f-106">Attributes and elements</span></span>

<span data-ttu-id="f549f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f549f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f549f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f549f-108">Attributes</span></span>

<span data-ttu-id="f549f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f549f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f549f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f549f-110">Child elements</span></span>

|<span data-ttu-id="f549f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f549f-111">**Element**</span></span>|<span data-ttu-id="f549f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f549f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f549f-113">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="f549f-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="f549f-114">Spécifie l’identificateur d’un élément.</span><span class="sxs-lookup"><span data-stu-id="f549f-114">Specifies the identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="f549f-115">DisableReason</span><span class="sxs-lookup"><span data-stu-id="f549f-115">DisableReason</span></span>](disablereason.md) <br/> |<span data-ttu-id="f549f-116">Spécifie la raison de la désactivation d’une application.</span><span class="sxs-lookup"><span data-stu-id="f549f-116">Specifies the reason for disabling an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f549f-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f549f-117">Parent elements</span></span>

<span data-ttu-id="f549f-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f549f-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f549f-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="f549f-119">Remarks</span></span>

<span data-ttu-id="f549f-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f549f-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f549f-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f549f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f549f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f549f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f549f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f549f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f549f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f549f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f549f-125">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="f549f-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="f549f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f549f-126">Validation File</span></span>  <br/> |<span data-ttu-id="f549f-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f549f-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f549f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f549f-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f549f-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f549f-129">See also</span></span>

- [<span data-ttu-id="f549f-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f549f-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

