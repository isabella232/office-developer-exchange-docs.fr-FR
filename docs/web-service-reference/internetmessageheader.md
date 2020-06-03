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
description: L’élément InternetMessageHeader représente l’en-tête de message Internet d’un en-tête donné dans la collection headers. Pour obtenir la collection entière des en-têtes de message Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur EWS et les en-têtes de message Internet, obtention les en-têtes de message Internet dans EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 7b662617e0b1a1fcdcce3449b729485ba6e0956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459306"
---
# <a name="internetmessageheader"></a><span data-ttu-id="55574-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="55574-105">InternetMessageHeader</span></span>

<span data-ttu-id="55574-106">L’élément **InternetMessageHeader** représente l’en-tête de message Internet d’un en-tête donné dans la collection headers.</span><span class="sxs-lookup"><span data-stu-id="55574-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="55574-107">Pour obtenir la collection entière des en-têtes de message Internet, utilisez la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="55574-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="55574-108">Pour plus d’informations sur EWS et les en-têtes de message Internet, consultez les rubriques «obtenir des en-têtes de message Internet dans [EWS, MIME et les en-têtes de messages Internet manquants](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="55574-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="55574-109">**InternetHeaderType**</span><span class="sxs-lookup"><span data-stu-id="55574-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55574-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55574-110">Attributes and elements</span></span>

<span data-ttu-id="55574-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55574-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55574-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="55574-112">Attributes</span></span>

|<span data-ttu-id="55574-113">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="55574-113">**Attribute**</span></span>|<span data-ttu-id="55574-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="55574-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55574-115">**HeaderName**</span><span class="sxs-lookup"><span data-stu-id="55574-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="55574-116">Identifie le nom de l’en-tête.</span><span class="sxs-lookup"><span data-stu-id="55574-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="55574-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55574-117">Child elements</span></span>

<span data-ttu-id="55574-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55574-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55574-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55574-119">Parent elements</span></span>

|<span data-ttu-id="55574-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55574-120">**Element**</span></span>|<span data-ttu-id="55574-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="55574-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55574-122">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="55574-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="55574-123">Représente la collection de tous les en-têtes de message Internet contenus dans un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="55574-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55574-124">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="55574-124">Text value</span></span>

<span data-ttu-id="55574-125">La valeur de texte représente la valeur de l’en-tête.</span><span class="sxs-lookup"><span data-stu-id="55574-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55574-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="55574-126">Remarks</span></span>

<span data-ttu-id="55574-127">Voici la définition de la propriété étendue de l’API managée EWS pour la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="55574-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="55574-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="55574-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55574-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55574-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55574-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55574-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55574-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55574-131">Schema Name</span></span>  <br/> |<span data-ttu-id="55574-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="55574-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="55574-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55574-133">Validation File</span></span>  <br/> |<span data-ttu-id="55574-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55574-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55574-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55574-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="55574-136">False</span><span class="sxs-lookup"><span data-stu-id="55574-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55574-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55574-137">See also</span></span>



- [<span data-ttu-id="55574-138">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="55574-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="55574-139">EWS, MIME et les en-têtes de message Internet manquants</span><span class="sxs-lookup"><span data-stu-id="55574-139">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

