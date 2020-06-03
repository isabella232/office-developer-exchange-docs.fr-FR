---
title: EcpUrl-MT (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: L’élément EcpUrl-MT spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi des messages électroniques pour un utilisateur à extension messagerie.
ms.openlocfilehash: 097811add5635bca14c659814652bca244a1398d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458711"
---
# <a name="ecpurl-mt-pox"></a><span data-ttu-id="43d68-103">EcpUrl-MT (POX)</span><span class="sxs-lookup"><span data-stu-id="43d68-103">EcpUrl-mt (POX)</span></span>

<span data-ttu-id="43d68-104">L’élément **EcpUrl-MT** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi des messages électroniques pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="43d68-104">The **EcpUrl-mt** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="43d68-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="43d68-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="43d68-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="43d68-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="43d68-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="43d68-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="43d68-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="43d68-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="43d68-109">EcpUrl-MT (POX)</span><span class="sxs-lookup"><span data-stu-id="43d68-109">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="43d68-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="43d68-110">Attributes and elements</span></span>

<span data-ttu-id="43d68-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="43d68-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43d68-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="43d68-112">Attributes</span></span>

<span data-ttu-id="43d68-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="43d68-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43d68-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="43d68-114">Child elements</span></span>

<span data-ttu-id="43d68-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="43d68-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="43d68-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="43d68-116">Parent elements</span></span>

|<span data-ttu-id="43d68-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="43d68-117">**Element**</span></span>|<span data-ttu-id="43d68-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="43d68-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43d68-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="43d68-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="43d68-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="43d68-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43d68-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="43d68-121">Text value</span></span>

<span data-ttu-id="43d68-122">La valeur texte représente une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de suivi du courrier électronique de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="43d68-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email tracking settings for the user.</span></span> <span data-ttu-id="43d68-123">La valeur de l’élément **EcpUrl-MT** contient les paramètres contenus dans les caractères « < » et « > » qui sont remplacés par le client, comme indiqué dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="43d68-123">The value of the **EcpUrl-mt** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="43d68-124">**Parameter**</span><span class="sxs-lookup"><span data-stu-id="43d68-124">**Parameter**</span></span>|<span data-ttu-id="43d68-125">**Remplacer par**</span><span class="sxs-lookup"><span data-stu-id="43d68-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="43d68-126">_IsOwa_</span><span class="sxs-lookup"><span data-stu-id="43d68-126">_IsOwa_</span></span> <br/> |<span data-ttu-id="43d68-127">n</span><span class="sxs-lookup"><span data-stu-id="43d68-127">n</span></span>  <br/> |
| <span data-ttu-id="43d68-128">_Identificateur_</span><span class="sxs-lookup"><span data-stu-id="43d68-128">_MsgID_</span></span> <br/> |<span data-ttu-id="43d68-129">Identificateur de message Internet du message à suivre, tel qu’il est spécifié par l’en-tête Message-ID.</span><span class="sxs-lookup"><span data-stu-id="43d68-129">Internet message identifier of the message to be tracked as specified by the Message-ID header.</span></span>  <br/> |
| <span data-ttu-id="43d68-130">_NomServeur > MBX_</span><span class="sxs-lookup"><span data-stu-id="43d68-130">_Mbx_</span></span> <br/> |<span data-ttu-id="43d68-131">Adresse SMTP du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="43d68-131">The SMTP address of the mailbox owner.</span></span>  <br/> |
| <span data-ttu-id="43d68-132">_Sender_</span><span class="sxs-lookup"><span data-stu-id="43d68-132">_Sender_</span></span> <br/> |<span data-ttu-id="43d68-133">Adresse SMTP de l’expéditeur du message.</span><span class="sxs-lookup"><span data-stu-id="43d68-133">The SMTP address of the message's sender.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="43d68-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="43d68-134">Remarks</span></span>

<span data-ttu-id="43d68-135">L’élément **EcpUrl-MT** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="43d68-135">The **EcpUrl-mt** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="43d68-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="43d68-136">See also</span></span>



[<span data-ttu-id="43d68-137">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="43d68-137">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

