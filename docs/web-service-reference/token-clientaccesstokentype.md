---
title: Jeton (ClientAccessTokenType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cddd6075-06b6-4858-9ffa-9db4d9d9b030
description: L’élément Token spécifie un jeton d’accès au client.
ms.openlocfilehash: d195e81d8d20eb2288e921c640c7b2898a5341ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467864"
---
# <a name="token-clientaccesstokentype"></a><span data-ttu-id="b6ae0-103">Jeton (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="b6ae0-103">Token (ClientAccessTokenType)</span></span>

<span data-ttu-id="b6ae0-104">L’élément **Token** spécifie un jeton d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="b6ae0-104">The **Token** element specifies a client access token.</span></span> 
  
```XML
<Token>
   <Id/>
   <TokenType/>
   <TokenValue/>
   <TTL/>
</Token>
```

 <span data-ttu-id="b6ae0-105">**ClientAccessTokenType**</span><span class="sxs-lookup"><span data-stu-id="b6ae0-105">**ClientAccessTokenType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6ae0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b6ae0-106">Attributes and elements</span></span>

<span data-ttu-id="b6ae0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b6ae0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6ae0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b6ae0-108">Attributes</span></span>

<span data-ttu-id="b6ae0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b6ae0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6ae0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b6ae0-110">Child elements</span></span>

<span data-ttu-id="b6ae0-111">[ID (chaîne)](id-string.md)  |  [TokenType](tokentype.md)  |  [TokenValue](tokenvalue.md)  |  [TTL](ttl.md)</span><span class="sxs-lookup"><span data-stu-id="b6ae0-111">[ID (String)](id-string.md) | [TokenType](tokentype.md) | [TokenValue](tokenvalue.md) | [TTL](ttl.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6ae0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b6ae0-112">Parent elements</span></span>

[<span data-ttu-id="b6ae0-113">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b6ae0-113">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="b6ae0-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="b6ae0-114">Remarks</span></span>

<span data-ttu-id="b6ae0-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b6ae0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6ae0-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6ae0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6ae0-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b6ae0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6ae0-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b6ae0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6ae0-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b6ae0-119">Schema name</span></span>  <br/> |<span data-ttu-id="b6ae0-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b6ae0-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6ae0-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b6ae0-121">Validation file</span></span>  <br/> |<span data-ttu-id="b6ae0-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b6ae0-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6ae0-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b6ae0-123">Can be empty</span></span>  <br/> ||
   

