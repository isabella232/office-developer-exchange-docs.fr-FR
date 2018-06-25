---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: L’élément EcpUrl-mt spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’un utilisateur à extension messagerie de suivi des messages électroniques.
ms.openlocfilehash: 13954a4dab8e81f4ba75b3578e6ba7f67f4b8b96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756060"
---
# <a name="ecpurl-mt-pox"></a><span data-ttu-id="a5c61-103">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="a5c61-103">EcpUrl-mt (POX)</span></span>

<span data-ttu-id="a5c61-104">L’élément **EcpUrl-mt** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’un utilisateur à extension messagerie de suivi des messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="a5c61-104">The **EcpUrl-mt** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="a5c61-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="a5c61-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a5c61-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="a5c61-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a5c61-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="a5c61-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a5c61-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="a5c61-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a5c61-109">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="a5c61-109">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a5c61-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a5c61-110">Attributes and elements</span></span>

<span data-ttu-id="a5c61-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a5c61-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5c61-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="a5c61-112">Attributes</span></span>

<span data-ttu-id="a5c61-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5c61-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5c61-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a5c61-114">Child elements</span></span>

<span data-ttu-id="a5c61-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5c61-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5c61-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a5c61-116">Parent elements</span></span>

|<span data-ttu-id="a5c61-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a5c61-117">**Element**</span></span>|<span data-ttu-id="a5c61-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="a5c61-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5c61-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="a5c61-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a5c61-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="a5c61-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5c61-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a5c61-121">Text value</span></span>

<span data-ttu-id="a5c61-122">La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut servir à accéder à leur messagerie suivi des paramètres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a5c61-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email tracking settings for the user.</span></span> <span data-ttu-id="a5c61-123">La valeur de l’élément **EcpUrl-mt** contient des paramètres contenus dans « < » et « > » caractères sont remplacés par le client, comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="a5c61-123">The value of the **EcpUrl-mt** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="a5c61-124">**Paramètre**</span><span class="sxs-lookup"><span data-stu-id="a5c61-124">**Parameter**</span></span>|<span data-ttu-id="a5c61-125">**Remplacer par**</span><span class="sxs-lookup"><span data-stu-id="a5c61-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="a5c61-126">_IsOwa_</span><span class="sxs-lookup"><span data-stu-id="a5c61-126">_IsOwa_</span></span> <br/> |<span data-ttu-id="a5c61-127">n</span><span class="sxs-lookup"><span data-stu-id="a5c61-127">n</span></span>  <br/> |
| <span data-ttu-id="a5c61-128">_Identificateur de message_</span><span class="sxs-lookup"><span data-stu-id="a5c61-128">_MsgID_</span></span> <br/> |<span data-ttu-id="a5c61-129">Identificateur de message Internet du message suivi comme spécifié par l’en-tête de Message-ID.</span><span class="sxs-lookup"><span data-stu-id="a5c61-129">Internet message identifier of the message to be tracked as specified by the Message-ID header.</span></span>  <br/> |
| <span data-ttu-id="a5c61-130">_Mbx_</span><span class="sxs-lookup"><span data-stu-id="a5c61-130">_Mbx_</span></span> <br/> |<span data-ttu-id="a5c61-131">L’adresse SMTP du propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a5c61-131">The SMTP address of the mailbox owner.</span></span>  <br/> |
| <span data-ttu-id="a5c61-132">_Sender_</span><span class="sxs-lookup"><span data-stu-id="a5c61-132">_Sender_</span></span> <br/> |<span data-ttu-id="a5c61-133">L’adresse SMTP de l’expéditeur du message.</span><span class="sxs-lookup"><span data-stu-id="a5c61-133">The SMTP address of the message's sender.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a5c61-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="a5c61-134">Remarks</span></span>

<span data-ttu-id="a5c61-135">L’élément **EcpUrl-mt** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="a5c61-135">The **EcpUrl-mt** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a5c61-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a5c61-136">See also</span></span>



[<span data-ttu-id="a5c61-137">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="a5c61-137">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

