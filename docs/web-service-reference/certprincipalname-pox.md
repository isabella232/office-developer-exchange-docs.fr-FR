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
description: L’élément CertPrincipalName Spécifie le nom principal du certificat Secure Sockets Layer (SSL) qui est nécessaire pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL.
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755502"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="30cff-103">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="30cff-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="30cff-104">L’élément **CertPrincipalName** Spécifie le nom principal du certificat Secure Sockets Layer (SSL) qui est nécessaire pour se connecter à l’organisation Microsoft Exchange Server 2007 à l’aide de SSL.</span><span class="sxs-lookup"><span data-stu-id="30cff-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="30cff-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="30cff-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="30cff-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="30cff-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="30cff-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="30cff-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="30cff-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="30cff-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="30cff-109">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="30cff-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="30cff-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="30cff-110">Attributes and elements</span></span>

<span data-ttu-id="30cff-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="30cff-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30cff-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="30cff-112">Attributes</span></span>

<span data-ttu-id="30cff-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30cff-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30cff-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="30cff-114">Child elements</span></span>

<span data-ttu-id="30cff-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30cff-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30cff-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="30cff-116">Parent elements</span></span>

|<span data-ttu-id="30cff-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="30cff-117">**Element**</span></span>|<span data-ttu-id="30cff-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="30cff-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30cff-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="30cff-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="30cff-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Exchange 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="30cff-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30cff-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="30cff-121">Text value</span></span>

<span data-ttu-id="30cff-122">La valeur texte spécifie le nom principal du certificat SSL qui est requise pour se connecter à l’organisation Microsoft Exchange à l’aide de SSL.</span><span class="sxs-lookup"><span data-stu-id="30cff-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30cff-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="30cff-123">Remarks</span></span>

<span data-ttu-id="30cff-124">Si l’élément **CertPrincipalName** n’est pas spécifié, la valeur par défaut est définie à msstd:SERVER, où serveur est la valeur qui est spécifiée dans l’élément [Serveur (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="30cff-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="30cff-125">Par exemple, si le serveur est spécifié en tant qu’exemple.com et **CertPrincipalName** avec [SSL (POX)](ssl-pox.md) activée est vide, la valeur par défaut **CertPrincipalName** serait msstd:example.com.</span><span class="sxs-lookup"><span data-stu-id="30cff-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="30cff-126">Si **aucun** n’est spécifié, Windows valide le nom principal du certificat en fonction des informations figurant dans la rubrique [Noms principaux](http://go.microsoft.com/fwlink/?LinkId=93417) sur MSDN.</span><span class="sxs-lookup"><span data-stu-id="30cff-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](http://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="30cff-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="30cff-127">See also</span></span>



[<span data-ttu-id="30cff-128">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="30cff-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

