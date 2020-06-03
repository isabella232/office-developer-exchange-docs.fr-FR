---
title: Externe (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: L’élément External contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange depuis l’extérieur du réseau de l’organisation.
ms.openlocfilehash: 45d7e72c5a43c5c468c1edd303a5e5ea8c2cb62e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457969"
---
# <a name="external-pox"></a><span data-ttu-id="6f4a6-103">Externe (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-103">External (POX)</span></span>

<span data-ttu-id="6f4a6-104">L’élément **External** contient une collection d’URL qu’un client peut utiliser pour se connecter à Exchange depuis l’extérieur du réseau de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="6f4a6-104">The **External** element contains a collection of URLs that a client can use to connect to Exchange from outside of the organization's network.</span></span> 
  
[<span data-ttu-id="6f4a6-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6f4a6-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6f4a6-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6f4a6-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="6f4a6-109">Externe (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-109">External (POX)</span></span>](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

```

## <a name="attributes-and-elements"></a><span data-ttu-id="6f4a6-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6f4a6-110">Attributes and elements</span></span>

<span data-ttu-id="6f4a6-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6f4a6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f4a6-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="6f4a6-112">Attributes</span></span>

<span data-ttu-id="6f4a6-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6f4a6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f4a6-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6f4a6-114">Child elements</span></span>

|<span data-ttu-id="6f4a6-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6f4a6-115">**Element**</span></span>|<span data-ttu-id="6f4a6-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="6f4a6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f4a6-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="6f4a6-118">Décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur spécifique qui exécute Microsoft Exchange Server sur lequel le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="6f4a6-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="6f4a6-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6f4a6-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6f4a6-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="6f4a6-121">Cet élément de **protocole** n’a que deux éléments enfants : un élément de [type (POX)](type-pox.md) spécifiant le protocole de connexion et un élément [ASUrl (POX)](asurl-pox.md) , spécifiant le point de terminaison EWS pour le service Web de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="6f4a6-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f4a6-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6f4a6-122">Parent elements</span></span>

|<span data-ttu-id="6f4a6-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6f4a6-123">**Element**</span></span>|<span data-ttu-id="6f4a6-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="6f4a6-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f4a6-125">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="6f4a6-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6f4a6-126">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6f4a6-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f4a6-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="6f4a6-127">Remarks</span></span>

<span data-ttu-id="6f4a6-128">L’élément **External** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="6f4a6-128">The **External** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6f4a6-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6f4a6-129">See also</span></span>



[<span data-ttu-id="6f4a6-130">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="6f4a6-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

