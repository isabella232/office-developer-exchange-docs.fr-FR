---
title: ProtocolConnection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: L’élément ProtocolConnection représente le protocole de connexion du client Web server.
ms.openlocfilehash: 8b5396821cd959e41d24fcf7a94c519f9c634a1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828915"
---
# <a name="protocolconnection-soap"></a><span data-ttu-id="b9217-103">ProtocolConnection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9217-103">ProtocolConnection (SOAP)</span></span>

<span data-ttu-id="b9217-104">L’élément **ProtocolConnection** représente le protocole de connexion du client Web server.</span><span class="sxs-lookup"><span data-stu-id="b9217-104">The **ProtocolConnection** element represents the protocol connection of the server Web client.</span></span> 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 <span data-ttu-id="b9217-105">**ProtocolConnection**</span><span class="sxs-lookup"><span data-stu-id="b9217-105">**ProtocolConnection**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9217-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b9217-106">Attributes and elements</span></span>

<span data-ttu-id="b9217-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b9217-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9217-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b9217-108">Attributes</span></span>

<span data-ttu-id="b9217-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b9217-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9217-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b9217-110">Child elements</span></span>

|<span data-ttu-id="b9217-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b9217-111">**Element**</span></span>|<span data-ttu-id="b9217-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b9217-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9217-113">Nom d’hôte (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9217-113">Hostname (SOAP)</span></span>](hostname-soap.md) <br/> |<span data-ttu-id="b9217-114">Représente la partie de nom d’hôte du nom complet de l’ordinateur de l’ordinateur.</span><span class="sxs-lookup"><span data-stu-id="b9217-114">Represents the host name portion of the full computer name of the computer.</span></span>  <br/> |
|[<span data-ttu-id="b9217-115">Port (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9217-115">Port (SOAP)</span></span>](port-soap.md) <br/> |<span data-ttu-id="b9217-116">Représente le numéro de port à utiliser pour le protocole.</span><span class="sxs-lookup"><span data-stu-id="b9217-116">Represents the port number to use for the protocol.</span></span>  <br/> |
|[<span data-ttu-id="b9217-117">EncryptionMethod (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9217-117">EncryptionMethod (SOAP)</span></span>](encryptionmethod-soap.md) <br/> |<span data-ttu-id="b9217-118">Représente la méthode de chiffrement qui est utilisée pour les protocoles POP, IMAP et SMTP.</span><span class="sxs-lookup"><span data-stu-id="b9217-118">Represents the cryptographic method that is used for the POP, IMAP, and SMTP protocols.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9217-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b9217-119">Parent elements</span></span>

|<span data-ttu-id="b9217-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b9217-120">**Element**</span></span>|<span data-ttu-id="b9217-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="b9217-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9217-122">ProtocolConnections (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9217-122">ProtocolConnections (SOAP)</span></span>](protocolconnections-soap.md) <br/> |<span data-ttu-id="b9217-123">Contient zéro ou plusieurs connexions de protocole.</span><span class="sxs-lookup"><span data-stu-id="b9217-123">Contains zero or more protocol connections.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9217-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b9217-124">Text value</span></span>

<span data-ttu-id="b9217-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b9217-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9217-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b9217-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9217-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b9217-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b9217-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b9217-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b9217-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="b9217-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b9217-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b9217-130">Validation File</span></span>  <br/> |<span data-ttu-id="b9217-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b9217-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9217-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b9217-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9217-133">True</span><span class="sxs-lookup"><span data-stu-id="b9217-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9217-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b9217-134">See also</span></span>



[<span data-ttu-id="b9217-135">ProtocolConnectionCollectionSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b9217-135">ProtocolConnectionCollectionSetting (SOAP)</span></span>](protocolconnectioncollectionsetting-soap.md)

