---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: L’élément InstallApp spécifie la demande pour installer une application.
ms.openlocfilehash: d9b7412865c003b89eccbdd92aa6ff9968048191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827949"
---
# <a name="installapp"></a><span data-ttu-id="66b07-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="66b07-103">InstallApp</span></span>

<span data-ttu-id="66b07-104">L’élément **InstallApp** spécifie la demande pour installer une application.</span><span class="sxs-lookup"><span data-stu-id="66b07-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="66b07-105">**InstallAppType**</span><span class="sxs-lookup"><span data-stu-id="66b07-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66b07-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="66b07-106">Attributes and elements</span></span>

<span data-ttu-id="66b07-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="66b07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66b07-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="66b07-108">Attributes</span></span>

<span data-ttu-id="66b07-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="66b07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66b07-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="66b07-110">Child elements</span></span>

|<span data-ttu-id="66b07-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="66b07-111">**Element**</span></span>|<span data-ttu-id="66b07-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="66b07-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66b07-113">Manifeste</span><span class="sxs-lookup"><span data-stu-id="66b07-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="66b07-114">Contient le fichier de manifeste d’application codé en base64.</span><span class="sxs-lookup"><span data-stu-id="66b07-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66b07-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="66b07-115">Parent elements</span></span>

<span data-ttu-id="66b07-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="66b07-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66b07-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="66b07-117">Remarks</span></span>

<span data-ttu-id="66b07-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="66b07-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="66b07-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="66b07-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66b07-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="66b07-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66b07-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="66b07-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66b07-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="66b07-122">Schema Name</span></span>  <br/> |<span data-ttu-id="66b07-123">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="66b07-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="66b07-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="66b07-124">Validation File</span></span>  <br/> |<span data-ttu-id="66b07-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66b07-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66b07-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="66b07-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="66b07-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="66b07-127">See also</span></span>



- [<span data-ttu-id="66b07-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="66b07-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

