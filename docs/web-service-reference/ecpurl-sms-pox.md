---
title: EcpUrl-sms (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: f5e5e589-ee16-42a8-9cd4-ae3909fc869b
description: L’élément EcpUrl-sms spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres du Service SMS (Short Message) pour un utilisateur à extension messagerie.
ms.openlocfilehash: 38471db7b7e046e43425b132b1716033c1c96afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756068"
---
# <a name="ecpurl-sms-pox"></a><span data-ttu-id="3c589-103">EcpUrl-sms (POX)</span><span class="sxs-lookup"><span data-stu-id="3c589-103">EcpUrl-sms (POX)</span></span>

<span data-ttu-id="3c589-104">L’élément **EcpUrl-sms** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres du Service SMS (Short Message) pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="3c589-104">The **EcpUrl-sms** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access Short Message Service (SMS) settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="3c589-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="3c589-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="3c589-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="3c589-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="3c589-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="3c589-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="3c589-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="3c589-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="3c589-109">EcpUrl-sms (POX)</span><span class="sxs-lookup"><span data-stu-id="3c589-109">EcpUrl-sms (POX)</span></span>](ecpurl-sms-pox.md)
  
```XML
<EcpUrl-sms/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="3c589-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3c589-110">Attributes and elements</span></span>

<span data-ttu-id="3c589-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3c589-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c589-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="3c589-112">Attributes</span></span>

<span data-ttu-id="3c589-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c589-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c589-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3c589-114">Child elements</span></span>

<span data-ttu-id="3c589-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c589-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c589-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3c589-116">Parent elements</span></span>

|<span data-ttu-id="3c589-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c589-117">**Element**</span></span>|<span data-ttu-id="3c589-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c589-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c589-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="3c589-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="3c589-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="3c589-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c589-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3c589-121">Text value</span></span>

<span data-ttu-id="3c589-122">La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de SMS pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3c589-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access SMS settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3c589-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="3c589-123">Remarks</span></span>

<span data-ttu-id="3c589-124">L’élément **EcpUrl-sms** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="3c589-124">The **EcpUrl-sms** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3c589-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3c589-125">See also</span></span>



[<span data-ttu-id="3c589-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="3c589-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

