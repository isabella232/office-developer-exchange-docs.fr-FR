---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: L’élément InstallApp spécifie la demande d’installation d’une application.
ms.openlocfilehash: 003a72507813677484b2d6ee75f8ff577df169e3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468004"
---
# <a name="installapp"></a><span data-ttu-id="399e6-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="399e6-103">InstallApp</span></span>

<span data-ttu-id="399e6-104">L’élément **InstallApp** spécifie la demande d’installation d’une application.</span><span class="sxs-lookup"><span data-stu-id="399e6-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="399e6-105">**InstallAppType**</span><span class="sxs-lookup"><span data-stu-id="399e6-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="399e6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="399e6-106">Attributes and elements</span></span>

<span data-ttu-id="399e6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="399e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="399e6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="399e6-108">Attributes</span></span>

<span data-ttu-id="399e6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="399e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="399e6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="399e6-110">Child elements</span></span>

|<span data-ttu-id="399e6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="399e6-111">**Element**</span></span>|<span data-ttu-id="399e6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="399e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="399e6-113">Manifeste</span><span class="sxs-lookup"><span data-stu-id="399e6-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="399e6-114">Contient le fichier manifeste d’application encodé en base64.</span><span class="sxs-lookup"><span data-stu-id="399e6-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="399e6-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="399e6-115">Parent elements</span></span>

<span data-ttu-id="399e6-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="399e6-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="399e6-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="399e6-117">Remarks</span></span>

<span data-ttu-id="399e6-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="399e6-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="399e6-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="399e6-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="399e6-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="399e6-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="399e6-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="399e6-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="399e6-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="399e6-122">Schema Name</span></span>  <br/> |<span data-ttu-id="399e6-123">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="399e6-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="399e6-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="399e6-124">Validation File</span></span>  <br/> |<span data-ttu-id="399e6-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="399e6-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="399e6-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="399e6-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="399e6-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="399e6-127">See also</span></span>



- [<span data-ttu-id="399e6-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="399e6-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

