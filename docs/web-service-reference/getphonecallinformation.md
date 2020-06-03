---
title: GetPhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 5f4ee71c-bde0-4b0d-b426-0c24dfe67585
description: L’élément GetPhoneCallInformation spécifie une demande d’obtention d’informations sur les appels téléphoniques.
ms.openlocfilehash: b835cd301b1c243e88034d1057026ef1305b9038
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530196"
---
# <a name="getphonecallinformation"></a><span data-ttu-id="b0986-103">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="b0986-103">GetPhoneCallInformation</span></span>

<span data-ttu-id="b0986-104">L’élément **GetPhoneCallInformation** spécifie une demande d’obtention d’informations sur les appels téléphoniques.</span><span class="sxs-lookup"><span data-stu-id="b0986-104">The **GetPhoneCallInformation** element specifies a request to get telephone call information.</span></span> 
  
```xml
<GetPhoneCallInformation>
   <PhoneCallId/>
</GetPhoneCallInformation>
```

 <span data-ttu-id="b0986-105">**GetPhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="b0986-105">**GetPhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0986-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b0986-106">Attributes and elements</span></span>

<span data-ttu-id="b0986-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b0986-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0986-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b0986-108">Attributes</span></span>

<span data-ttu-id="b0986-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b0986-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0986-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b0986-110">Child elements</span></span>

|<span data-ttu-id="b0986-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b0986-111">**Element**</span></span>|<span data-ttu-id="b0986-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0986-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0986-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="b0986-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="b0986-114">Spécifie l’identificateur d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="b0986-114">Specifies the identifier of a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0986-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b0986-115">Parent elements</span></span>

<span data-ttu-id="b0986-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b0986-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b0986-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b0986-117">Text value</span></span>

<span data-ttu-id="b0986-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b0986-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0986-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="b0986-119">Remarks</span></span>

<span data-ttu-id="b0986-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0986-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0986-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b0986-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0986-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b0986-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0986-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b0986-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b0986-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b0986-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0986-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b0986-125">Validation File</span></span>  <br/> |<span data-ttu-id="b0986-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b0986-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0986-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b0986-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0986-128">False</span><span class="sxs-lookup"><span data-stu-id="b0986-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0986-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b0986-129">See also</span></span>



- [<span data-ttu-id="b0986-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b0986-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

