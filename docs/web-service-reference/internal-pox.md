---
title: Interne (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: L’élément interne contient la collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir de l’intérieur du réseau de l’organisation.
ms.openlocfilehash: 0dc5b679af98b52f15ef3b40181c2d97f102f373
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827946"
---
# <a name="internal-pox"></a><span data-ttu-id="20dda-103">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-103">Internal (POX)</span></span>

<span data-ttu-id="20dda-104">L’élément **interne** contient la collection d’URL qu’un client peut utiliser pour se connecter à Exchange à partir de l’intérieur du réseau de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="20dda-104">The **Internal** element contains the collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span> 
  
[<span data-ttu-id="20dda-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="20dda-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="20dda-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="20dda-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="20dda-109">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-109">Internal (POX)</span></span>](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="20dda-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20dda-110">Attributes and elements</span></span>

<span data-ttu-id="20dda-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20dda-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20dda-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="20dda-112">Attributes</span></span>

<span data-ttu-id="20dda-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20dda-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20dda-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20dda-114">Child elements</span></span>

|<span data-ttu-id="20dda-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20dda-115">**Element**</span></span>|<span data-ttu-id="20dda-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="20dda-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20dda-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="20dda-118">Décrit l’URL et le schéma d’authentification qui est utilisé pour accéder à un ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur Client Access installé qui héberge Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="20dda-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="20dda-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="20dda-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="20dda-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="20dda-121">Cet élément de **protocole** n'a que deux éléments enfants : un élément de [Type (POX)](type-pox.md) spécifiant le protocole de connexion et un élément [ASUrl (POX)](asurl-pox.md) , en spécifiant le point de terminaison EWS pour le service web de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="20dda-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20dda-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20dda-122">Parent elements</span></span>

|<span data-ttu-id="20dda-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20dda-123">**Element**</span></span>|<span data-ttu-id="20dda-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="20dda-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20dda-125">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="20dda-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="20dda-126">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="20dda-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="20dda-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="20dda-127">Remarks</span></span>

<span data-ttu-id="20dda-128">L’élément **interne** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="20dda-128">The **Internal** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="20dda-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20dda-129">See also</span></span>



[<span data-ttu-id="20dda-130">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="20dda-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

