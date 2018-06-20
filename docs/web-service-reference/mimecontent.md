---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: L’élément MimeContent contient le flux MIME ASCII d’un objet qui est représenté dans le format base64Binary et prend en charge [RFC2045].
ms.openlocfilehash: 60f2d42f09347611559137c494d93036f1192829
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828465"
---
# <a name="mimecontent"></a><span data-ttu-id="bb2ca-103">MimeContent</span><span class="sxs-lookup"><span data-stu-id="bb2ca-103">MimeContent</span></span>

<span data-ttu-id="bb2ca-104">L’élément **MimeContent** contient le flux MIME ASCII d’un objet qui est représenté dans le format base64Binary et prend en charge [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span><span class="sxs-lookup"><span data-stu-id="bb2ca-104">The **MimeContent** element contains the ASCII MIME stream of an object that is represented in base64Binary format and supports [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span></span>
  
```xml
<MimeContent CharacterSet="" />
```

 <span data-ttu-id="bb2ca-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="bb2ca-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb2ca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bb2ca-106">Attributes and elements</span></span>

<span data-ttu-id="bb2ca-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb2ca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bb2ca-108">Attributes</span></span>

|<span data-ttu-id="bb2ca-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bb2ca-109">**Attribute**</span></span>|<span data-ttu-id="bb2ca-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb2ca-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bb2ca-111">**Jeu de caractères**</span><span class="sxs-lookup"><span data-stu-id="bb2ca-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="bb2ca-112">Si la valeur, la valeur de cet attribut est ignorée par le serveur.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bb2ca-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bb2ca-113">Child elements</span></span>

<span data-ttu-id="bb2ca-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb2ca-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bb2ca-115">Parent elements</span></span>

<span data-ttu-id="bb2ca-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [élément](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [tâche](task.md)</span><span class="sxs-lookup"><span data-stu-id="bb2ca-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="bb2ca-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bb2ca-117">Text value</span></span>

<span data-ttu-id="bb2ca-118">Une valeur de texte qui représente un flux de données MIME base64Binary est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-118">A text value that represents a base64Binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb2ca-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="bb2ca-119">Remarks</span></span>

<span data-ttu-id="bb2ca-120">Le contenu du message transite par les trois niveaux de codage avant d’être stocké dans la valeur **MimeContent** suivants :</span><span class="sxs-lookup"><span data-stu-id="bb2ca-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContent** value:</span></span> 
  
1. <span data-ttu-id="bb2ca-121">Texte du message : il s’agit de l’organisme codage, tel qu’iso-2022-jp pour les caractères japonais.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="bb2ca-122">Flux de données MIME — il s’agit de l’encodage ASCII du texte du message pour l’élément **MimeContent** , ou le codage UTF-8 du texte du message pour l’élément [MimeContentUTF8](mimecontentutf8.md) .</span><span class="sxs-lookup"><span data-stu-id="bb2ca-122">MIME stream — This is the ASCII encoding of the message text for the **MimeContent** element, or the UTF8 encoding of the message text for the [MimeContentUTF8](mimecontentutf8.md) element.</span></span> 
    
3. <span data-ttu-id="bb2ca-123">Document XML — il s’agit toujours le flux ASCII codé en base64 du flux de données MIME, où caractères tels que «\<», qui sont significatif au format XML, sont masquées à partir d’analyseurs XML.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="bb2ca-124">Chaque niveau est indépendante du niveau qui le précède.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="bb2ca-125">L’élément **MimeContent** peut contenir les mêmes données qui contiennent des autres propriétés qui sont renvoyées avec un élément.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-125">The **MimeContent** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="bb2ca-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb2ca-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb2ca-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bb2ca-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb2ca-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bb2ca-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb2ca-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bb2ca-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bb2ca-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bb2ca-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb2ca-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bb2ca-131">Validation File</span></span>  <br/> |<span data-ttu-id="bb2ca-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bb2ca-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb2ca-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bb2ca-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb2ca-134">False</span><span class="sxs-lookup"><span data-stu-id="bb2ca-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb2ca-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bb2ca-135">See also</span></span>



- [<span data-ttu-id="bb2ca-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bb2ca-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

