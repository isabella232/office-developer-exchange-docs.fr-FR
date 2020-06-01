---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: L’élément SMTPLast spécifie si le serveur SMTP (Simple Mail Transfer Protocol) requiert le téléchargement du courrier électronique avant qu’il envoie des messages électroniques à l’aide du serveur SMTP.
ms.openlocfilehash: 7019da28ffa196a9abc8798aa75aff2756198da3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468431"
---
# <a name="smtplast-pox"></a><span data-ttu-id="cf193-103">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="cf193-103">SMTPLast (POX)</span></span>

<span data-ttu-id="cf193-104">L’élément **SMTPLast** spécifie si le serveur SMTP (Simple Mail Transfer Protocol) requiert le téléchargement du courrier électronique avant qu’il envoie des messages électroniques à l’aide du serveur SMTP.</span><span class="sxs-lookup"><span data-stu-id="cf193-104">The **SMTPLast** element specifies whether the Simple Mail Transfer Protocol (SMTP) server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> 
  
- [<span data-ttu-id="cf193-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="cf193-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="cf193-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="cf193-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="cf193-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="cf193-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="cf193-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="cf193-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="cf193-109">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="cf193-109">SMTPLast (POX)</span></span>](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cf193-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cf193-110">Attributes and elements</span></span>

<span data-ttu-id="cf193-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cf193-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf193-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="cf193-112">Attributes</span></span>

<span data-ttu-id="cf193-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cf193-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf193-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cf193-114">Child elements</span></span>

<span data-ttu-id="cf193-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cf193-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf193-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cf193-116">Parent elements</span></span>

|<span data-ttu-id="cf193-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf193-117">**Element**</span></span>|<span data-ttu-id="cf193-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf193-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf193-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="cf193-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="cf193-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cf193-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf193-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="cf193-121">Text value</span></span>

<span data-ttu-id="cf193-122">La valeur texte spécifie si le serveur SMTP requiert le téléchargement du courrier électronique avant l’envoi de courrier électronique à l’aide du serveur SMTP.</span><span class="sxs-lookup"><span data-stu-id="cf193-122">The text value specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> <span data-ttu-id="cf193-123">Les valeurs possibles sont **on** et **off**.</span><span class="sxs-lookup"><span data-stu-id="cf193-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="cf193-124">La valeur par défaut est **off**.</span><span class="sxs-lookup"><span data-stu-id="cf193-124">The default value is **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cf193-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf193-125">See also</span></span>

- [<span data-ttu-id="cf193-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="cf193-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

