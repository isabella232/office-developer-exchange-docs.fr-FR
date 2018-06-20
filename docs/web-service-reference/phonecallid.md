---
title: PhoneCallId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallId
api_type:
- schema
ms.assetid: 79e31a4c-fc84-4802-8761-470df8d63694
description: L’élément PhoneCallId Spécifie l’identificateur d’un appel téléphonique. Cet élément est obligatoire.
ms.openlocfilehash: 1886d9510fe254c016779166efccc9882fd77d2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828757"
---
# <a name="phonecallid"></a><span data-ttu-id="fdcf5-104">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="fdcf5-104">PhoneCallId</span></span>

<span data-ttu-id="fdcf5-105">L’élément **PhoneCallId** Spécifie l’identificateur d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="fdcf5-106">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="fdcf5-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="fdcf5-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdcf5-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fdcf5-108">Attributes and elements</span></span>

<span data-ttu-id="fdcf5-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdcf5-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="fdcf5-110">Attributes</span></span>

|<span data-ttu-id="fdcf5-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="fdcf5-111">**Attribute**</span></span>|<span data-ttu-id="fdcf5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fdcf5-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fdcf5-113">ID</span><span class="sxs-lookup"><span data-stu-id="fdcf5-113">Id</span></span>  <br/> |<span data-ttu-id="fdcf5-114">Identifie l’appel téléphonique pour déconnecter la session.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="fdcf5-115">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fdcf5-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fdcf5-116">Child elements</span></span>

<span data-ttu-id="fdcf5-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fdcf5-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fdcf5-118">Parent elements</span></span>

|<span data-ttu-id="fdcf5-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fdcf5-119">**Element**</span></span>|<span data-ttu-id="fdcf5-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="fdcf5-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdcf5-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="fdcf5-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="fdcf5-122">Représente une demande de déconnexion d’un appel.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="fdcf5-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="fdcf5-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="fdcf5-124">Représente une demande pour obtenir des informations d’appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="fdcf5-125">PlayOnPhoneResponse (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="fdcf5-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="fdcf5-126">Définit une réponse à une demande de PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fdcf5-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="fdcf5-127">Remarks</span></span>

<span data-ttu-id="fdcf5-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="fdcf5-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdcf5-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fdcf5-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdcf5-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fdcf5-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fdcf5-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fdcf5-131">Schema Name</span></span>  <br/> |<span data-ttu-id="fdcf5-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fdcf5-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fdcf5-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fdcf5-133">Validation File</span></span>  <br/> |<span data-ttu-id="fdcf5-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fdcf5-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fdcf5-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fdcf5-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="fdcf5-136">False</span><span class="sxs-lookup"><span data-stu-id="fdcf5-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fdcf5-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fdcf5-137">See also</span></span>



- [<span data-ttu-id="fdcf5-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fdcf5-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

