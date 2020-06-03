---
title: TokenType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 83c650eb-7ab8-480c-a7c9-df60072ee042
description: L’élément TokenType spécifie le type de jeton.
ms.openlocfilehash: a42849dce9ed0253c3c5d4d4e899367b8e105594
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459881"
---
# <a name="tokentype"></a><span data-ttu-id="55629-103">TokenType</span><span class="sxs-lookup"><span data-stu-id="55629-103">TokenType</span></span>

<span data-ttu-id="55629-104">L’élément **TokenType** spécifie le type de jeton.</span><span class="sxs-lookup"><span data-stu-id="55629-104">The **TokenType** element specifies the type of token.</span></span> 
  
```XML
<TokenType> CallerIdentity | ExtensionCallback | ScopedToken </TokenType>
```

 <span data-ttu-id="55629-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="55629-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55629-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55629-106">Attributes and elements</span></span>

<span data-ttu-id="55629-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55629-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55629-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="55629-108">Attributes</span></span>

<span data-ttu-id="55629-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="55629-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55629-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55629-110">Child elements</span></span>

<span data-ttu-id="55629-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55629-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55629-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55629-112">Parent elements</span></span>

<span data-ttu-id="55629-113">[TokenRequest](tokenrequest.md)  |  [Jeton (Token](token.md) )</span><span class="sxs-lookup"><span data-stu-id="55629-113">[TokenRequest](tokenrequest.md) | [Token](token.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="55629-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="55629-114">Text value</span></span>

<span data-ttu-id="55629-115">La valeur de texte de l’élément **TokenType** est le type de jeton.</span><span class="sxs-lookup"><span data-stu-id="55629-115">The text value of the **TokenType** element is the token type.</span></span> <span data-ttu-id="55629-116">La valeur de texte **CallerIdentity** indique que le jeton est un jeton d’identité de l’appelant.</span><span class="sxs-lookup"><span data-stu-id="55629-116">The text value of **CallerIdentity** indicates that the token is a caller identity token.</span></span> <span data-ttu-id="55629-117">La valeur de texte **ExtensionCallback** indique que le jeton est destiné à un rappel d’extension.</span><span class="sxs-lookup"><span data-stu-id="55629-117">The text value of **ExtensionCallback** indicates that the token is for an extension callback.</span></span> <span data-ttu-id="55629-118">La valeur de texte **ScopedToken** indique que le jeton d’accès au client est un jeton d’étendue.</span><span class="sxs-lookup"><span data-stu-id="55629-118">The text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="55629-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="55629-119">Remarks</span></span>

<span data-ttu-id="55629-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="55629-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="55629-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="55629-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55629-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55629-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55629-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55629-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55629-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55629-124">Schema name</span></span>  <br/> |<span data-ttu-id="55629-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="55629-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="55629-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55629-126">Validation file</span></span>  <br/> |<span data-ttu-id="55629-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55629-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55629-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55629-128">Can be empty</span></span>  <br/> |<span data-ttu-id="55629-129">false</span><span class="sxs-lookup"><span data-stu-id="55629-129">false</span></span>  <br/> |
   

