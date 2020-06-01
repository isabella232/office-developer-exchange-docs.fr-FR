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
description: L’élément PhoneCallInformation spécifie les informations d’État pour un appel téléphonique.
ms.openlocfilehash: 75370bccb841818a8302bdd055ad96fd16b2e8df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468844"
---
# <a name="phonecallinformation"></a><span data-ttu-id="d7417-103">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="d7417-103">PhoneCallInformation</span></span>

<span data-ttu-id="d7417-104">L’élément **PhoneCallInformation** spécifie les informations d’État pour un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="d7417-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="d7417-105">**PhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="d7417-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7417-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d7417-106">Attributes and elements</span></span>

<span data-ttu-id="d7417-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d7417-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7417-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d7417-108">Attributes</span></span>

<span data-ttu-id="d7417-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d7417-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7417-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d7417-110">Child elements</span></span>

|<span data-ttu-id="d7417-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d7417-111">**Element**</span></span>|<span data-ttu-id="d7417-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d7417-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7417-113">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="d7417-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="d7417-114">Spécifie l’état d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="d7417-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="d7417-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d7417-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d7417-116">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="d7417-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="d7417-117">Indique la cause de l’échec d’une connexion.</span><span class="sxs-lookup"><span data-stu-id="d7417-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="d7417-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d7417-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d7417-119">SIPResponseText</span><span class="sxs-lookup"><span data-stu-id="d7417-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="d7417-120">Spécifie le texte de la réponse SIP.</span><span class="sxs-lookup"><span data-stu-id="d7417-120">Specifies the SIP response text.</span></span> <span data-ttu-id="d7417-121">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d7417-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d7417-122">SIPResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7417-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="d7417-123">Spécifie le code de réponse SIP.</span><span class="sxs-lookup"><span data-stu-id="d7417-123">Specifies the SIP response code.</span></span> <span data-ttu-id="d7417-124">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d7417-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7417-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d7417-125">Parent elements</span></span>

|<span data-ttu-id="d7417-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d7417-126">**Element**</span></span>|<span data-ttu-id="d7417-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="d7417-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7417-128">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="d7417-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="d7417-129">Définit une réponse à une demande d' [opération GetPhoneCallInformation](getphonecallinformation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d7417-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7417-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="d7417-130">Remarks</span></span>

<span data-ttu-id="d7417-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7417-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7417-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d7417-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7417-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d7417-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d7417-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d7417-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d7417-135">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d7417-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d7417-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d7417-136">Validation File</span></span>  <br/> |<span data-ttu-id="d7417-137">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d7417-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7417-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d7417-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7417-139">False</span><span class="sxs-lookup"><span data-stu-id="d7417-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7417-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d7417-140">See also</span></span>



- [<span data-ttu-id="d7417-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d7417-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

