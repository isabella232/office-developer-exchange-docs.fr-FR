---
title: TokenRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45f8e-c02b-4ead-b15a-38b30872c362
description: L’élément TokenRequest spécifie une seule demande d’émission de jeton.
ms.openlocfilehash: b7e814cbcf34912f79bded57874dbc8e4ce28176
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838747"
---
# <a name="tokenrequest"></a><span data-ttu-id="2a187-103">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="2a187-103">TokenRequest</span></span>

<span data-ttu-id="2a187-104">L’élément **TokenRequest** spécifie une seule demande d’émission de jeton.</span><span class="sxs-lookup"><span data-stu-id="2a187-104">The **TokenRequest** element specifies a single token request.</span></span> 
  
```XML
<TokenRequest>
   <Id/>
   <TokenType/>
</TokenRequest>
```

 <span data-ttu-id="2a187-105">**ClientAccessTokenRequestType**</span><span class="sxs-lookup"><span data-stu-id="2a187-105">**ClientAccessTokenRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a187-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2a187-106">Attributes and elements</span></span>

<span data-ttu-id="2a187-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2a187-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a187-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2a187-108">Attributes</span></span>

<span data-ttu-id="2a187-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2a187-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a187-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2a187-110">Child elements</span></span>

<span data-ttu-id="2a187-111">[ID (chaîne)](id-string.md) | [TokenType (ClientAccessTokenType)](tokentype-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="2a187-111">[ID (String)](id-string.md) | [TokenType (ClientAccessTokenType)](tokentype-clientaccesstokentype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a187-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2a187-112">Parent elements</span></span>

[<span data-ttu-id="2a187-113">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="2a187-113">TokenRequests</span></span>](tokenrequests.md)
  
## <a name="remarks"></a><span data-ttu-id="2a187-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="2a187-114">Remarks</span></span>

<span data-ttu-id="2a187-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2a187-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2a187-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2a187-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a187-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2a187-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a187-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2a187-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a187-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2a187-119">Schema name</span></span>  <br/> |<span data-ttu-id="2a187-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2a187-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="2a187-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2a187-121">Validation file</span></span>  <br/> |<span data-ttu-id="2a187-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2a187-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a187-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2a187-123">Can be empty</span></span>  <br/> |<span data-ttu-id="2a187-124">false</span><span class="sxs-lookup"><span data-stu-id="2a187-124">false</span></span>  <br/> |
   

