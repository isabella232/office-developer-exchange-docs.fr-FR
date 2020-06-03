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
description: L’élément PhoneCallId spécifie l’identificateur d’un appel téléphonique. Cet élément est obligatoire.
ms.openlocfilehash: 3e4b9dba5e8be6e45a0c16508531fbc6cf91c170
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459699"
---
# <a name="phonecallid"></a><span data-ttu-id="3de98-104">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="3de98-104">PhoneCallId</span></span>

<span data-ttu-id="3de98-105">L’élément **PhoneCallId** spécifie l’identificateur d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="3de98-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="3de98-106">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="3de98-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="3de98-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="3de98-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3de98-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3de98-108">Attributes and elements</span></span>

<span data-ttu-id="3de98-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3de98-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3de98-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="3de98-110">Attributes</span></span>

|<span data-ttu-id="3de98-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="3de98-111">**Attribute**</span></span>|<span data-ttu-id="3de98-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3de98-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3de98-113">ID</span><span class="sxs-lookup"><span data-stu-id="3de98-113">Id</span></span>  <br/> |<span data-ttu-id="3de98-114">Identifie l’appel téléphonique à déconnecter.</span><span class="sxs-lookup"><span data-stu-id="3de98-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="3de98-115">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="3de98-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3de98-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3de98-116">Child elements</span></span>

<span data-ttu-id="3de98-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3de98-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3de98-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3de98-118">Parent elements</span></span>

|<span data-ttu-id="3de98-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3de98-119">**Element**</span></span>|<span data-ttu-id="3de98-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="3de98-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3de98-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="3de98-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="3de98-122">Représente une demande de déconnexion d’un appel.</span><span class="sxs-lookup"><span data-stu-id="3de98-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="3de98-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="3de98-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="3de98-124">Représente une demande d’obtention d’informations sur les appels téléphoniques.</span><span class="sxs-lookup"><span data-stu-id="3de98-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="3de98-125">PlayOnPhoneResponse (services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="3de98-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="3de98-126">Définit une réponse à une demande PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="3de98-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3de98-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="3de98-127">Remarks</span></span>

<span data-ttu-id="3de98-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3de98-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3de98-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3de98-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3de98-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3de98-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3de98-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3de98-131">Schema Name</span></span>  <br/> |<span data-ttu-id="3de98-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3de98-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3de98-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3de98-133">Validation File</span></span>  <br/> |<span data-ttu-id="3de98-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3de98-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3de98-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3de98-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="3de98-136">False</span><span class="sxs-lookup"><span data-stu-id="3de98-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3de98-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3de98-137">See also</span></span>



- [<span data-ttu-id="3de98-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3de98-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

