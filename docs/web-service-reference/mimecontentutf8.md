---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: L’élément MimeContentUTF8 contient le flux MIME UTF-8 d’un objet qui est représenté dans le format base64Binary et internationalisation des adresses de messagerie prend en charge et [RFC6530].
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828466"
---
# <a name="mimecontentutf8"></a><span data-ttu-id="aaac3-103">MimeContentUTF8</span><span class="sxs-lookup"><span data-stu-id="aaac3-103">MimeContentUTF8</span></span>

<span data-ttu-id="aaac3-104">L’élément **MimeContentUTF8** contient le flux MIME UTF-8 d’un objet qui est représenté dans le format base64Binary et prend en charge internationalisation des adresses de messagerie et [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span><span class="sxs-lookup"><span data-stu-id="aaac3-104">The **MimeContentUTF8** element contains the UTF-8 MIME stream of an object that is represented in base64Binary format and supports email address internationalization and [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span></span>
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 <span data-ttu-id="aaac3-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="aaac3-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaac3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aaac3-106">Attributes and elements</span></span>

<span data-ttu-id="aaac3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aaac3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaac3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aaac3-108">Attributes</span></span>

|<span data-ttu-id="aaac3-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="aaac3-109">**Attribute**</span></span>|<span data-ttu-id="aaac3-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="aaac3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aaac3-111">**Jeu de caractères**</span><span class="sxs-lookup"><span data-stu-id="aaac3-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="aaac3-112">Si la valeur, la valeur de cet attribut est ignorée par le serveur.</span><span class="sxs-lookup"><span data-stu-id="aaac3-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="aaac3-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aaac3-113">Child elements</span></span>

<span data-ttu-id="aaac3-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aaac3-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aaac3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aaac3-115">Parent elements</span></span>

<span data-ttu-id="aaac3-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [élément](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [tâche](task.md)</span><span class="sxs-lookup"><span data-stu-id="aaac3-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="aaac3-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="aaac3-117">Text value</span></span>

<span data-ttu-id="aaac3-118">Une valeur de texte qui représente un flux de données MIME base64binary est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="aaac3-118">A text value that represents a base64binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aaac3-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="aaac3-119">Remarks</span></span>

<span data-ttu-id="aaac3-120">Le contenu du message transite par les trois niveaux de codage avant d’être stocké dans la valeur **MimeContentUTF8** suivants :</span><span class="sxs-lookup"><span data-stu-id="aaac3-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContentUTF8** value:</span></span> 
  
1. <span data-ttu-id="aaac3-121">Texte du message : il s’agit de l’organisme codage, tel qu’iso-2022-jp pour les caractères japonais.</span><span class="sxs-lookup"><span data-stu-id="aaac3-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="aaac3-122">Flux de données MIME — il s’agit de l’encodage UTF-8 du texte du message pour l’élément **MimeContentUTF8** , ou le codage ASCII du texte du message pour l’élément [MimeContent](mimecontent.md) .</span><span class="sxs-lookup"><span data-stu-id="aaac3-122">MIME stream — This is the UTF8 encoding of the message text for the **MimeContentUTF8** element, or the ASCII encoding of the message text for the [MimeContent](mimecontent.md) element.</span></span> 
    
3. <span data-ttu-id="aaac3-123">Document XML — il s’agit toujours le flux ASCII codé en base64 du flux de données MIME, où caractères tels que «\<», qui sont significatif au format XML, sont masquées à partir d’analyseurs XML.</span><span class="sxs-lookup"><span data-stu-id="aaac3-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="aaac3-124">Chaque niveau est indépendante du niveau qui le précède.</span><span class="sxs-lookup"><span data-stu-id="aaac3-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="aaac3-125">L’élément **MimeContentUTF8** peut contenir les mêmes données qui contiennent des autres propriétés qui sont renvoyées avec un élément.</span><span class="sxs-lookup"><span data-stu-id="aaac3-125">The **MimeContentUTF8** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="aaac3-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aaac3-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="aaac3-127">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="aaac3-127">Version differences</span></span>

<span data-ttu-id="aaac3-128">Cet élément est disponible dans les versions d’Exchange commençant par build 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="aaac3-128">This element is available in versions of Exchange starting with build 15.00.0986.00.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aaac3-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aaac3-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaac3-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aaac3-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aaac3-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aaac3-131">Schema Name</span></span>  <br/> |<span data-ttu-id="aaac3-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="aaac3-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="aaac3-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aaac3-133">Validation File</span></span>  <br/> |<span data-ttu-id="aaac3-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aaac3-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aaac3-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aaac3-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="aaac3-136">False</span><span class="sxs-lookup"><span data-stu-id="aaac3-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aaac3-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aaac3-137">See also</span></span>



- [<span data-ttu-id="aaac3-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aaac3-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

