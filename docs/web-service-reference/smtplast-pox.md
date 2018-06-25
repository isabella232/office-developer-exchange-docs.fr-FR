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
description: L’élément SMTPLast indique si le serveur SMTP Simple Mail Transfer Protocol () nécessite que courrier électronique doit être téléchargée avant qu’il envoie un message électronique à l’aide du serveur SMTP.
ms.openlocfilehash: 5359f20b33855f4ef48566058bc46bd618e3b2ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829505"
---
# <a name="smtplast-pox"></a><span data-ttu-id="b7d82-103">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="b7d82-103">SMTPLast (POX)</span></span>

<span data-ttu-id="b7d82-104">L’élément **SMTPLast** indique si le serveur SMTP Simple Mail Transfer Protocol () nécessite que courrier électronique doit être téléchargée avant qu’il envoie un message électronique à l’aide du serveur SMTP.</span><span class="sxs-lookup"><span data-stu-id="b7d82-104">The **SMTPLast** element specifies whether the Simple Mail Transfer Protocol (SMTP) server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> 
  
- [<span data-ttu-id="b7d82-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="b7d82-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="b7d82-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="b7d82-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="b7d82-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="b7d82-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="b7d82-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="b7d82-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="b7d82-109">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="b7d82-109">SMTPLast (POX)</span></span>](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b7d82-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b7d82-110">Attributes and elements</span></span>

<span data-ttu-id="b7d82-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b7d82-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7d82-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="b7d82-112">Attributes</span></span>

<span data-ttu-id="b7d82-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7d82-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7d82-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b7d82-114">Child elements</span></span>

<span data-ttu-id="b7d82-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b7d82-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7d82-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b7d82-116">Parent elements</span></span>

|<span data-ttu-id="b7d82-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b7d82-117">**Element**</span></span>|<span data-ttu-id="b7d82-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="b7d82-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7d82-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="b7d82-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b7d82-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="b7d82-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7d82-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b7d82-121">Text value</span></span>

<span data-ttu-id="b7d82-122">La valeur texte spécifie si le serveur SMTP requiert que courrier électronique doit être téléchargée avant qu’il envoie un message électronique à l’aide du serveur SMTP.</span><span class="sxs-lookup"><span data-stu-id="b7d82-122">The text value specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> <span data-ttu-id="b7d82-123">Les valeurs possibles sont **on** et **off**.</span><span class="sxs-lookup"><span data-stu-id="b7d82-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="b7d82-124">La valeur par défaut est **désactivé**.</span><span class="sxs-lookup"><span data-stu-id="b7d82-124">The default value is **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b7d82-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b7d82-125">See also</span></span>

- [<span data-ttu-id="b7d82-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b7d82-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

