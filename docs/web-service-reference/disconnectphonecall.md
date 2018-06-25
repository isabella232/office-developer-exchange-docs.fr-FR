---
title: DisconnectPhoneCall
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCall
api_type:
- schema
ms.assetid: f9252536-9852-4dd9-9ebc-91f5cf281171
description: L’élément DisconnectPhoneCall représente une demande de déconnexion d’un appel.
ms.openlocfilehash: 56947ea9ba56c76bb02d6a425ff43b3b846a2f60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755963"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="848b5-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="848b5-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="848b5-104">L’élément **DisconnectPhoneCall** représente une demande de déconnexion d’un appel.</span><span class="sxs-lookup"><span data-stu-id="848b5-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="848b5-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="848b5-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="848b5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="848b5-106">Attributes and elements</span></span>

<span data-ttu-id="848b5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="848b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="848b5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="848b5-108">Attributes</span></span>

<span data-ttu-id="848b5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="848b5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="848b5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="848b5-110">Child elements</span></span>

|<span data-ttu-id="848b5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="848b5-111">**Element**</span></span>|<span data-ttu-id="848b5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="848b5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="848b5-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="848b5-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="848b5-114">Spécifie l’identificateur de l’appel pour déconnecter la session.</span><span class="sxs-lookup"><span data-stu-id="848b5-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="848b5-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="848b5-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="848b5-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="848b5-116">Parent elements</span></span>

<span data-ttu-id="848b5-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="848b5-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="848b5-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="848b5-118">Text value</span></span>

<span data-ttu-id="848b5-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="848b5-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="848b5-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="848b5-120">Remarks</span></span>

<span data-ttu-id="848b5-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="848b5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="848b5-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="848b5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="848b5-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="848b5-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="848b5-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="848b5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="848b5-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="848b5-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="848b5-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="848b5-126">Validation File</span></span>  <br/> |<span data-ttu-id="848b5-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="848b5-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="848b5-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="848b5-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="848b5-129">False</span><span class="sxs-lookup"><span data-stu-id="848b5-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="848b5-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="848b5-130">See also</span></span>

- [<span data-ttu-id="848b5-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="848b5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

