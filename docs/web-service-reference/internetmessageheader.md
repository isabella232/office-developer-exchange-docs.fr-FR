---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: L’élément InternetMessageHeader représente l’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes. Pour obtenir l’ensemble des en-têtes de message Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur les en-têtes de message Internet et EWS, en-têtes de message Internet seeGetting dans EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827952"
---
# <a name="internetmessageheader"></a><span data-ttu-id="a6712-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="a6712-105">InternetMessageHeader</span></span>

<span data-ttu-id="a6712-106">L’élément **InternetMessageHeader** représente l’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes.</span><span class="sxs-lookup"><span data-stu-id="a6712-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="a6712-107">Pour obtenir l’ensemble des en-têtes de message Internet, utilisez la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="a6712-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="a6712-108">Pour plus d’informations à propos des en-têtes de message Internet et EWS, voir « en-têtes de message Internet mise en route dans [EWS, MIME et les en-têtes de message Internet manquants](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a6712-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="a6712-109">**InternetHeaderType**</span><span class="sxs-lookup"><span data-stu-id="a6712-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6712-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a6712-110">Attributes and elements</span></span>

<span data-ttu-id="a6712-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a6712-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6712-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="a6712-112">Attributes</span></span>

|<span data-ttu-id="a6712-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a6712-113">**Attribute**</span></span>|<span data-ttu-id="a6712-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a6712-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a6712-115">**HeaderName**</span><span class="sxs-lookup"><span data-stu-id="a6712-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="a6712-116">Identifie le nom d’en-tête.</span><span class="sxs-lookup"><span data-stu-id="a6712-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a6712-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a6712-117">Child elements</span></span>

<span data-ttu-id="a6712-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a6712-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6712-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a6712-119">Parent elements</span></span>

|<span data-ttu-id="a6712-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a6712-120">**Element**</span></span>|<span data-ttu-id="a6712-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="a6712-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6712-122">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="a6712-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="a6712-123">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a6712-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a6712-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a6712-124">Text value</span></span>

<span data-ttu-id="a6712-125">La valeur de texte représente la valeur de l’en-tête.</span><span class="sxs-lookup"><span data-stu-id="a6712-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a6712-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="a6712-126">Remarks</span></span>

<span data-ttu-id="a6712-127">Vous trouverez ci-dessous l’API managée EWS étendu de définition de la propriété pour la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="a6712-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="a6712-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6712-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6712-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a6712-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6712-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a6712-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6712-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a6712-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a6712-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a6712-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6712-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a6712-133">Validation File</span></span>  <br/> |<span data-ttu-id="a6712-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a6712-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6712-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a6712-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6712-136">False</span><span class="sxs-lookup"><span data-stu-id="a6712-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6712-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a6712-137">See also</span></span>



- [<span data-ttu-id="a6712-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a6712-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a6712-139">EWS, MIME et les en-têtes de message Internet manquants</span><span class="sxs-lookup"><span data-stu-id="a6712-139">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

