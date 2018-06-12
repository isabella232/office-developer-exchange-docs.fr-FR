---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: L’élément TokenType Spécifie le type de jeton.
ms.openlocfilehash: 5c8e880f035ed74776a7c77e4b4e60ca46d66d4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838743"
---
# <a name="tokentype"></a><span data-ttu-id="86d90-103">TokenType</span><span class="sxs-lookup"><span data-stu-id="86d90-103">TokenType</span></span>

<span data-ttu-id="86d90-104">L’élément **TokenType** Spécifie le type de jeton.</span><span class="sxs-lookup"><span data-stu-id="86d90-104">The **TokenType** element specifies the type of token.</span></span> 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 <span data-ttu-id="86d90-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="86d90-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86d90-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="86d90-106">Attributes and elements</span></span>

<span data-ttu-id="86d90-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="86d90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86d90-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="86d90-108">Attributes</span></span>

<span data-ttu-id="86d90-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86d90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86d90-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="86d90-110">Child elements</span></span>

<span data-ttu-id="86d90-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86d90-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86d90-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="86d90-112">Parent elements</span></span>

<span data-ttu-id="86d90-113">[TokenRequest](tokenrequest.md) | [jeton](token.md)</span><span class="sxs-lookup"><span data-stu-id="86d90-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="86d90-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="86d90-114">Text value</span></span>

<span data-ttu-id="86d90-115">La valeur de texte de l’élément **TokenType** est le type de jeton.</span><span class="sxs-lookup"><span data-stu-id="86d90-115">The text value of the **TokenType** element is the token type.</span></span> <span data-ttu-id="86d90-116">La valeur de texte de **CallerIdentity** indique que le jeton est un jeton d’identité de l’appelant.</span><span class="sxs-lookup"><span data-stu-id="86d90-116">The text value of **CallerIdentity** indicates that the token is a caller identity token.</span></span> <span data-ttu-id="86d90-117">La valeur de texte de **ExtensionCallback** indique que le jeton est un rappel d’extension.</span><span class="sxs-lookup"><span data-stu-id="86d90-117">The text value of **ExtensionCallback** indicates that the token is for an extension callback.</span></span> <span data-ttu-id="86d90-118">La valeur de texte de **ScopedToken** indique que le jeton d’accès client est un jeton de portée.</span><span class="sxs-lookup"><span data-stu-id="86d90-118">The text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="86d90-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="86d90-119">Remarks</span></span>

<span data-ttu-id="86d90-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="86d90-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="86d90-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="86d90-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86d90-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="86d90-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86d90-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="86d90-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86d90-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="86d90-124">Schema name</span></span>  <br/> |<span data-ttu-id="86d90-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="86d90-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="86d90-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="86d90-126">Validation file</span></span>  <br/> |<span data-ttu-id="86d90-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86d90-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86d90-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="86d90-128">Can be empty</span></span>  <br/> |<span data-ttu-id="86d90-129">false</span><span class="sxs-lookup"><span data-stu-id="86d90-129">false</span></span>  <br/> |
   

