---
title: GetClientExtensionResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4b1aba-a55d-4d64-ac80-5d4e6c4e72bd
description: L’élément GetClientExtensionResponse contient la réponse pour obtenir des informations de configuration d’une application.
ms.openlocfilehash: 523a103ec9397b0dce08aa47b074303c9e6ac897
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756542"
---
# <a name="getclientextensionresponse"></a><span data-ttu-id="7f5f3-103">GetClientExtensionResponse</span><span class="sxs-lookup"><span data-stu-id="7f5f3-103">GetClientExtensionResponse</span></span>

<span data-ttu-id="7f5f3-104">L’élément **GetClientExtensionResponse** contient la réponse pour obtenir des informations de configuration d’une application.</span><span class="sxs-lookup"><span data-stu-id="7f5f3-104">The **GetClientExtensionResponse** element contains the response to get configuration information about an app.</span></span> 
  
```XML
<GetClientExtensionResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ClientExtensions/>
   <RawMasterTableXml/>
</GetClientExtensionResponse>
```

 <span data-ttu-id="7f5f3-105">**ClientExtensionResponseType**</span><span class="sxs-lookup"><span data-stu-id="7f5f3-105">**ClientExtensionResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f5f3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7f5f3-106">Attributes and elements</span></span>

<span data-ttu-id="7f5f3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7f5f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f5f3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7f5f3-108">Attributes</span></span>

<span data-ttu-id="7f5f3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7f5f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f5f3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7f5f3-110">Child elements</span></span>

<span data-ttu-id="7f5f3-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ClientExtensions](clientextensions.md) | [RawMasterTableXml](rawmastertablexml.md)</span><span class="sxs-lookup"><span data-stu-id="7f5f3-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ClientExtensions](clientextensions.md) | [RawMasterTableXml](rawmastertablexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f5f3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7f5f3-112">Parent elements</span></span>

<span data-ttu-id="7f5f3-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7f5f3-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7f5f3-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="7f5f3-114">Remarks</span></span>

<span data-ttu-id="7f5f3-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7f5f3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7f5f3-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f5f3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f5f3-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7f5f3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f5f3-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7f5f3-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f5f3-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7f5f3-119">Schema name</span></span>  <br/> |<span data-ttu-id="7f5f3-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7f5f3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f5f3-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7f5f3-121">Validation file</span></span>  <br/> |<span data-ttu-id="7f5f3-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f5f3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f5f3-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7f5f3-123">Can be empty</span></span>  <br/> |<span data-ttu-id="7f5f3-124">false</span><span class="sxs-lookup"><span data-stu-id="7f5f3-124">false</span></span>  <br/> |
   

