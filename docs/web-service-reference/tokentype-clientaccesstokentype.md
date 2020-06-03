---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: L’élément TokenType identifie le type de jeton d’accès au client qui sera renvoyé dans la réponse GetClientAccessToken.
ms.openlocfilehash: 49ba2973967b12396e0c7f56129c89c40ccbcf97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466051"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="00b37-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="00b37-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="00b37-104">L’élément **TokenType** identifie le type de jeton d’accès au client qui sera renvoyé dans la réponse **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="00b37-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="00b37-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="00b37-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00b37-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00b37-106">Attributes and elements</span></span>

<span data-ttu-id="00b37-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00b37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00b37-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00b37-108">Attributes</span></span>

<span data-ttu-id="00b37-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00b37-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00b37-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00b37-110">Child elements</span></span>

<span data-ttu-id="00b37-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00b37-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00b37-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00b37-112">Parent elements</span></span>

<span data-ttu-id="00b37-113">[TokenRequest](tokenrequest.md)  |  [Jeton (ClientAccessTokenType)](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="00b37-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="00b37-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="00b37-114">Text value</span></span>

<span data-ttu-id="00b37-115">Une valeur de texte de **CallerIdentity** signifie qu’un jeton d’accès client d’identité de l’appelant est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="00b37-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="00b37-116">Une valeur de texte de **ExtensionCallback** indique qu’un jeton d’accès au client de rappel d’extension est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="00b37-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="00b37-117">Une valeur de texte de **ScopedToken** indique que le jeton d’accès au client est un jeton d’étendue.</span><span class="sxs-lookup"><span data-stu-id="00b37-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="00b37-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="00b37-118">Remarks</span></span>

<span data-ttu-id="00b37-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00b37-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00b37-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00b37-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00b37-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00b37-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00b37-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00b37-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00b37-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00b37-123">Schema name</span></span>  <br/> |<span data-ttu-id="00b37-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="00b37-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="00b37-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00b37-125">Validation file</span></span>  <br/> |<span data-ttu-id="00b37-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="00b37-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00b37-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00b37-127">Can be empty</span></span>  <br/> |<span data-ttu-id="00b37-128">false</span><span class="sxs-lookup"><span data-stu-id="00b37-128">false</span></span>  <br/> |
   

