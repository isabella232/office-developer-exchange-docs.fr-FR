---
title: TokenType (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96103f15-a3e0-497c-af21-90adbf9a4b14
description: L’élément TokenType identifie le type de jeton d’accès client qui est renvoyé dans la réponse GetClientAccessToken.
ms.openlocfilehash: c9adb60acf76fefebd58e2fd3bc899332a63dbee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838749"
---
# <a name="tokentype-clientaccesstokentype"></a><span data-ttu-id="c21cf-103">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="c21cf-103">TokenType (ClientAccessTokenType)</span></span>

<span data-ttu-id="c21cf-104">L’élément **TokenType** identifie le type de jeton d’accès client qui est renvoyé dans la réponse **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="c21cf-104">The **TokenType** element identifies the type of client access token that will be returned in the **GetClientAccessToken** response.</span></span> 
  
```XML
<TokenType>CallerIdentity | ExtensionCallback | ScopedToken</TokenType>
```

 <span data-ttu-id="c21cf-105">**ClientAccessTokenTypeType**</span><span class="sxs-lookup"><span data-stu-id="c21cf-105">**ClientAccessTokenTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c21cf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c21cf-106">Attributes and elements</span></span>

<span data-ttu-id="c21cf-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c21cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c21cf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c21cf-108">Attributes</span></span>

<span data-ttu-id="c21cf-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c21cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c21cf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c21cf-110">Child elements</span></span>

<span data-ttu-id="c21cf-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c21cf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c21cf-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c21cf-112">Parent elements</span></span>

<span data-ttu-id="c21cf-113">[TokenRequest](tokenrequest.md) | [jeton (ClientAccessTokenType)](token-clientaccesstokentype.md)</span><span class="sxs-lookup"><span data-stu-id="c21cf-113">[TokenRequest](tokenrequest.md) | [Token (ClientAccessTokenType)](token-clientaccesstokentype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c21cf-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c21cf-114">Text value</span></span>

<span data-ttu-id="c21cf-115">Une valeur texte **CallerIdentity** signifie qu'un jeton d’accès client appelant identity est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="c21cf-115">A text value of **CallerIdentity** means a caller identity client access token is returned.</span></span> <span data-ttu-id="c21cf-116">Une valeur texte **ExtensionCallback** indique qu’un jeton d’accès client extension rappel est retourné.</span><span class="sxs-lookup"><span data-stu-id="c21cf-116">A text value of **ExtensionCallback** indicates that an extension callback client access token is returned.</span></span> <span data-ttu-id="c21cf-117">Valeur texte **ScopedToken** indique que le jeton d’accès client est un jeton de portée.</span><span class="sxs-lookup"><span data-stu-id="c21cf-117">A text value of **ScopedToken** indicates that the client access token is a scoped token.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c21cf-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="c21cf-118">Remarks</span></span>

<span data-ttu-id="c21cf-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c21cf-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c21cf-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c21cf-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c21cf-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c21cf-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c21cf-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c21cf-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c21cf-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c21cf-123">Schema name</span></span>  <br/> |<span data-ttu-id="c21cf-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c21cf-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="c21cf-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c21cf-125">Validation file</span></span>  <br/> |<span data-ttu-id="c21cf-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c21cf-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c21cf-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c21cf-127">Can be empty</span></span>  <br/> |<span data-ttu-id="c21cf-128">false</span><span class="sxs-lookup"><span data-stu-id="c21cf-128">false</span></span>  <br/> |
   

