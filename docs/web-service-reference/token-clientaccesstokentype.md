---
title: Jeton (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: L’élément jeton spécifie un jeton d’accès client.
ms.openlocfilehash: 2e1f401141aef07a57a214968f6a6bafdf71f0dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838739"
---
# <a name="token-clientaccesstokentype"></a><span data-ttu-id="180c7-103">Jeton (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="180c7-103">Token (ClientAccessTokenType)</span></span>

<span data-ttu-id="180c7-104">L’élément **jeton** spécifie un jeton d’accès client.</span><span class="sxs-lookup"><span data-stu-id="180c7-104">The **Token** element specifies a client access token.</span></span> 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 <span data-ttu-id="180c7-105">**ClientAccessTokenType**</span><span class="sxs-lookup"><span data-stu-id="180c7-105">**ClientAccessTokenType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="180c7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="180c7-106">Attributes and elements</span></span>

<span data-ttu-id="180c7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="180c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="180c7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="180c7-108">Attributes</span></span>

<span data-ttu-id="180c7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="180c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="180c7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="180c7-110">Child elements</span></span>

<span data-ttu-id="180c7-111">[ID (chaîne)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)</span><span class="sxs-lookup"><span data-stu-id="180c7-111">[ID (String)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="180c7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="180c7-112">Parent elements</span></span>

[<span data-ttu-id="180c7-113">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="180c7-113">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="180c7-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="180c7-114">Remarks</span></span>

<span data-ttu-id="180c7-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="180c7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="180c7-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="180c7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="180c7-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="180c7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="180c7-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="180c7-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="180c7-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="180c7-119">Schema name</span></span>  <br/> |<span data-ttu-id="180c7-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="180c7-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="180c7-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="180c7-121">Validation file</span></span>  <br/> |<span data-ttu-id="180c7-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="180c7-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="180c7-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="180c7-123">Can be empty</span></span>  <br/> ||
   

