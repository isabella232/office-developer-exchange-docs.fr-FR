---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: L’élément CertPrincipalName spécifie le nom de principal du certificat SSL (Secure Sockets Layer) qui est requis pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL.
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463341"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="0cc46-103">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="0cc46-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="0cc46-104">L’élément **CertPrincipalName** spécifie le nom de principal du certificat SSL (Secure Sockets Layer) qui est requis pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL.</span><span class="sxs-lookup"><span data-stu-id="0cc46-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="0cc46-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="0cc46-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0cc46-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="0cc46-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0cc46-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="0cc46-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0cc46-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0cc46-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="0cc46-109">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="0cc46-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0cc46-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0cc46-110">Attributes and elements</span></span>

<span data-ttu-id="0cc46-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0cc46-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cc46-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="0cc46-112">Attributes</span></span>

<span data-ttu-id="0cc46-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0cc46-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cc46-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0cc46-114">Child elements</span></span>

<span data-ttu-id="0cc46-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0cc46-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0cc46-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0cc46-116">Parent elements</span></span>

|<span data-ttu-id="0cc46-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0cc46-117">**Element**</span></span>|<span data-ttu-id="0cc46-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0cc46-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cc46-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0cc46-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="0cc46-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Exchange 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0cc46-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0cc46-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0cc46-121">Text value</span></span>

<span data-ttu-id="0cc46-122">La valeur texte spécifie le nom de principal du certificat SSL qui est requis pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.</span><span class="sxs-lookup"><span data-stu-id="0cc46-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0cc46-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="0cc46-123">Remarks</span></span>

<span data-ttu-id="0cc46-124">Si l’élément **CertPrincipalName** n’est pas spécifié, la valeur par défaut est définie sur msstd : serveur, où serveur est la valeur spécifiée dans l’élément [serveur (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="0cc46-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="0cc46-125">Par exemple, si le serveur est spécifié en tant que example.com et que la valeur de **CertPrincipalName** est laissée vide avec le [protocole SSL (POX)](ssl-pox.md) activé, la valeur par défaut de **CertPrincipalName** serait msstd :example. com.</span><span class="sxs-lookup"><span data-stu-id="0cc46-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="0cc46-126">Si **aucune** valeur n’est spécifiée, Windows valide le nom de principal du certificat en fonction des informations figurant dans la rubrique [noms principaux](https://go.microsoft.com/fwlink/?LinkId=93417) sur MSDN.</span><span class="sxs-lookup"><span data-stu-id="0cc46-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](https://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0cc46-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0cc46-127">See also</span></span>



[<span data-ttu-id="0cc46-128">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0cc46-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

