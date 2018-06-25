---
title: PhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: L’élément PhoneCallInformation spécifie les informations d’état pour un appel téléphonique.
ms.openlocfilehash: e64e7b38b3801c60df8a966e95d980746533d3a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828758"
---
# <a name="phonecallinformation"></a><span data-ttu-id="61ef3-103">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="61ef3-103">PhoneCallInformation</span></span>

<span data-ttu-id="61ef3-104">L’élément **PhoneCallInformation** spécifie les informations d’état pour un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="61ef3-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="61ef3-105">**PhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="61ef3-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61ef3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="61ef3-106">Attributes and elements</span></span>

<span data-ttu-id="61ef3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="61ef3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61ef3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="61ef3-108">Attributes</span></span>

<span data-ttu-id="61ef3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="61ef3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61ef3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="61ef3-110">Child elements</span></span>

|<span data-ttu-id="61ef3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="61ef3-111">**Element**</span></span>|<span data-ttu-id="61ef3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="61ef3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61ef3-113">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="61ef3-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="61ef3-114">Spécifie l’état d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="61ef3-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="61ef3-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="61ef3-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="61ef3-116">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="61ef3-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="61ef3-117">Spécifie la cause d’un échec de connexion.</span><span class="sxs-lookup"><span data-stu-id="61ef3-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="61ef3-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="61ef3-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="61ef3-119">SIPResponseText</span><span class="sxs-lookup"><span data-stu-id="61ef3-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="61ef3-120">Spécifie le texte de réponse SIP.</span><span class="sxs-lookup"><span data-stu-id="61ef3-120">Specifies the SIP response text.</span></span> <span data-ttu-id="61ef3-121">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="61ef3-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="61ef3-122">SIPResponseCode</span><span class="sxs-lookup"><span data-stu-id="61ef3-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="61ef3-123">Spécifie le code de réponse SIP.</span><span class="sxs-lookup"><span data-stu-id="61ef3-123">Specifies the SIP response code.</span></span> <span data-ttu-id="61ef3-124">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="61ef3-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="61ef3-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="61ef3-125">Parent elements</span></span>

|<span data-ttu-id="61ef3-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="61ef3-126">**Element**</span></span>|<span data-ttu-id="61ef3-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="61ef3-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61ef3-128">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="61ef3-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="61ef3-129">Définit une réponse à une demande [d’opération GetPhoneCallInformation](getphonecallinformation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="61ef3-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61ef3-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="61ef3-130">Remarks</span></span>

<span data-ttu-id="61ef3-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="61ef3-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61ef3-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="61ef3-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61ef3-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="61ef3-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="61ef3-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="61ef3-134">Schema Name</span></span>  <br/> |<span data-ttu-id="61ef3-135">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="61ef3-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="61ef3-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="61ef3-136">Validation File</span></span>  <br/> |<span data-ttu-id="61ef3-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="61ef3-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="61ef3-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="61ef3-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="61ef3-139">False</span><span class="sxs-lookup"><span data-stu-id="61ef3-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61ef3-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="61ef3-140">See also</span></span>



- [<span data-ttu-id="61ef3-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="61ef3-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

