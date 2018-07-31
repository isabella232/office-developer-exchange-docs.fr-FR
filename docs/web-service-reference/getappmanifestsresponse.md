---
title: GetAppManifestsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: L’élément GetAppManifestsResponse définit la réponse à une demande d’opération GetAppManifests.
ms.openlocfilehash: ae9d1d853023a5b42db2e8fee2ed57f585433f69
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354147"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="fe64c-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="fe64c-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="fe64c-104">L’élément **GetAppManifestsResponse** définit la réponse à une demande d’opération **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="fe64c-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Manifests/>
</GetAppManifestsResponse>
```

```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Apps/>
</GetAppManifestsResponse>
```

<span data-ttu-id="fe64c-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="fe64c-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fe64c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fe64c-106">Attributes and elements</span></span>

<span data-ttu-id="fe64c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fe64c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe64c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fe64c-108">Attributes</span></span>

<span data-ttu-id="fe64c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe64c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe64c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fe64c-110">Child elements</span></span>

<span data-ttu-id="fe64c-111">[ResponseCode](responsecode.md) | [manifestes](manifests.md) | [applications](apps.md)</span><span class="sxs-lookup"><span data-stu-id="fe64c-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe64c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fe64c-112">Parent elements</span></span>

<span data-ttu-id="fe64c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe64c-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fe64c-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="fe64c-114">Remarks</span></span>

<span data-ttu-id="fe64c-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fe64c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fe64c-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe64c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe64c-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fe64c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe64c-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fe64c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fe64c-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fe64c-119">Schema Name</span></span>  <br/> |<span data-ttu-id="fe64c-120">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="fe64c-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="fe64c-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fe64c-121">Validation File</span></span>  <br/> |<span data-ttu-id="fe64c-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fe64c-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fe64c-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fe64c-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="fe64c-124">False</span><span class="sxs-lookup"><span data-stu-id="fe64c-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe64c-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe64c-125">See also</span></span>

- [<span data-ttu-id="fe64c-126">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fe64c-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

