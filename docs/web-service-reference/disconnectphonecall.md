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
ms.openlocfilehash: 8d64ecb9dce1d8b7efcebc70686db8fcbf867217
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529706"
---
# <a name="disconnectphonecall"></a><span data-ttu-id="bd984-103">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="bd984-103">DisconnectPhoneCall</span></span>

<span data-ttu-id="bd984-104">L’élément **DisconnectPhoneCall** représente une demande de déconnexion d’un appel.</span><span class="sxs-lookup"><span data-stu-id="bd984-104">The **DisconnectPhoneCall** element represents a request to disconnect a call.</span></span> 
  
```xml
<DisconnectPhoneCall>
   <PhoneCallId/>
</DisconnectPhoneCall>
```

 <span data-ttu-id="bd984-105">**DisconnectPhoneCallType**</span><span class="sxs-lookup"><span data-stu-id="bd984-105">**DisconnectPhoneCallType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd984-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bd984-106">Attributes and elements</span></span>

<span data-ttu-id="bd984-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bd984-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd984-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bd984-108">Attributes</span></span>

<span data-ttu-id="bd984-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bd984-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd984-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bd984-110">Child elements</span></span>

|<span data-ttu-id="bd984-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd984-111">**Element**</span></span>|<span data-ttu-id="bd984-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd984-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd984-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="bd984-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="bd984-114">Spécifie l’identificateur de l’appel à déconnecter.</span><span class="sxs-lookup"><span data-stu-id="bd984-114">Specifies the identifier of the call to disconnect.</span></span> <span data-ttu-id="bd984-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="bd984-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd984-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bd984-116">Parent elements</span></span>

<span data-ttu-id="bd984-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd984-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="bd984-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bd984-118">Text value</span></span>

<span data-ttu-id="bd984-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd984-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd984-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="bd984-120">Remarks</span></span>

<span data-ttu-id="bd984-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd984-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd984-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bd984-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd984-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bd984-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd984-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bd984-124">Schema Name</span></span>  <br/> |<span data-ttu-id="bd984-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bd984-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd984-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bd984-126">Validation File</span></span>  <br/> |<span data-ttu-id="bd984-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bd984-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd984-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bd984-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd984-129">False</span><span class="sxs-lookup"><span data-stu-id="bd984-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd984-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd984-130">See also</span></span>

- [<span data-ttu-id="bd984-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bd984-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

