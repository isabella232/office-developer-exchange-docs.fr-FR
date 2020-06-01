---
title: GetAppManifestsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: L’élément GetAppManifestsResponse définit la réponse pour une demande d’opération GetAppManifests.
ms.openlocfilehash: a01f6265d6d534e2f7868b17acf19f0f5d52a01f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462963"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="08ae7-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="08ae7-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="08ae7-104">L’élément **GetAppManifestsResponse** définit la réponse pour une demande d’opération **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="08ae7-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
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

<span data-ttu-id="08ae7-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="08ae7-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="08ae7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08ae7-106">Attributes and elements</span></span>

<span data-ttu-id="08ae7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08ae7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08ae7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="08ae7-108">Attributes</span></span>

<span data-ttu-id="08ae7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="08ae7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08ae7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08ae7-110">Child elements</span></span>

<span data-ttu-id="08ae7-111">[ResponseCode](responsecode.md)  |  [Manifestes](manifests.md)  |  [Applications](apps.md)</span><span class="sxs-lookup"><span data-stu-id="08ae7-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08ae7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08ae7-112">Parent elements</span></span>

<span data-ttu-id="08ae7-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08ae7-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08ae7-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="08ae7-114">Remarks</span></span>

<span data-ttu-id="08ae7-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="08ae7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="08ae7-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="08ae7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08ae7-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="08ae7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08ae7-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="08ae7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="08ae7-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="08ae7-119">Schema Name</span></span>  <br/> |<span data-ttu-id="08ae7-120">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="08ae7-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="08ae7-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="08ae7-121">Validation File</span></span>  <br/> |<span data-ttu-id="08ae7-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="08ae7-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08ae7-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="08ae7-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="08ae7-124">False</span><span class="sxs-lookup"><span data-stu-id="08ae7-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08ae7-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08ae7-125">See also</span></span>

- [<span data-ttu-id="08ae7-126">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="08ae7-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

