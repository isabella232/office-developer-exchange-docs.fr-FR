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
description: L’élément Internal contient la collection d’URL qu’un client peut utiliser pour se connecter à Exchange à l’intérieur du réseau de l’organisation.
ms.openlocfilehash: 8164a018a11f9bae9c3abcbfebf6cf0694ca4183
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465596"
---
# <a name="internal-pox"></a><span data-ttu-id="08cb0-103">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-103">Internal (POX)</span></span>

<span data-ttu-id="08cb0-104">L’élément **Internal** contient la collection d’URL qu’un client peut utiliser pour se connecter à Exchange à l’intérieur du réseau de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="08cb0-104">The **Internal** element contains the collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span> 
  
[<span data-ttu-id="08cb0-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="08cb0-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="08cb0-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="08cb0-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="08cb0-109">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-109">Internal (POX)</span></span>](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="08cb0-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08cb0-110">Attributes and elements</span></span>

<span data-ttu-id="08cb0-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08cb0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08cb0-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="08cb0-112">Attributes</span></span>

<span data-ttu-id="08cb0-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="08cb0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08cb0-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08cb0-114">Child elements</span></span>

|<span data-ttu-id="08cb0-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08cb0-115">**Element**</span></span>|<span data-ttu-id="08cb0-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="08cb0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08cb0-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="08cb0-118">Décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur spécifique qui exécute Microsoft Exchange Server sur lequel le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="08cb0-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="08cb0-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="08cb0-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="08cb0-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="08cb0-121">Cet élément de **protocole** n’a que deux éléments enfants : un élément de [type (POX)](type-pox.md) spécifiant le protocole de connexion et un élément [ASUrl (POX)](asurl-pox.md) , spécifiant le point de terminaison EWS pour le service Web de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="08cb0-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08cb0-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08cb0-122">Parent elements</span></span>

|<span data-ttu-id="08cb0-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08cb0-123">**Element**</span></span>|<span data-ttu-id="08cb0-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="08cb0-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08cb0-125">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="08cb0-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="08cb0-126">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="08cb0-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="08cb0-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="08cb0-127">Remarks</span></span>

<span data-ttu-id="08cb0-128">L’élément **Internal** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="08cb0-128">The **Internal** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="08cb0-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08cb0-129">See also</span></span>



[<span data-ttu-id="08cb0-130">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="08cb0-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

