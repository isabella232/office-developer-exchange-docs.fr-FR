---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: L’élément MimeContentUTF8 contient le flux MIME UTF-8 d’un objet représenté au format base64Binary et prend en charge l’internationalisation des adresses de messagerie et [RFC6530].
ms.openlocfilehash: a9214bda876c1aadac5b026b3adf38faea8ef17a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530428"
---
# <a name="mimecontentutf8"></a><span data-ttu-id="d4baf-103">MimeContentUTF8</span><span class="sxs-lookup"><span data-stu-id="d4baf-103">MimeContentUTF8</span></span>

<span data-ttu-id="d4baf-104">L’élément **MimeContentUTF8** contient le flux MIME UTF-8 d’un objet représenté au format base64Binary et prend en charge l’internationalisation des adresses de messagerie et [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span><span class="sxs-lookup"><span data-stu-id="d4baf-104">The **MimeContentUTF8** element contains the UTF-8 MIME stream of an object that is represented in base64Binary format and supports email address internationalization and [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span></span>
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 <span data-ttu-id="d4baf-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="d4baf-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4baf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4baf-106">Attributes and elements</span></span>

<span data-ttu-id="d4baf-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4baf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4baf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4baf-108">Attributes</span></span>

|<span data-ttu-id="d4baf-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d4baf-109">**Attribute**</span></span>|<span data-ttu-id="d4baf-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4baf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4baf-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="d4baf-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="d4baf-112">Si ce paramètre est défini, la valeur de cet attribut est ignorée par le serveur.</span><span class="sxs-lookup"><span data-stu-id="d4baf-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d4baf-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4baf-113">Child elements</span></span>

<span data-ttu-id="d4baf-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4baf-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4baf-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4baf-115">Parent elements</span></span>

<span data-ttu-id="d4baf-116">[CalendarItem](calendaritem.md)  |  [Contact](contact.md)  |  [DistributionList](distributionlist.md)  |  [Élément](item.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [MeetingMessage](meetingmessage.md)  |  [Propriété meetingrequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [Message](message-ex15websvcsotherref.md)  |  [RemoveItem](removeitem.md)  |  [Tâche](task.md)</span><span class="sxs-lookup"><span data-stu-id="d4baf-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d4baf-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d4baf-117">Text value</span></span>

<span data-ttu-id="d4baf-118">Une valeur de texte qui représente un flux MIME base64Binary est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="d4baf-118">A text value that represents a base64binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4baf-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4baf-119">Remarks</span></span>

<span data-ttu-id="d4baf-120">Le contenu du message passe par les trois niveaux d’encodage suivants avant d’être stocké dans la valeur **MimeContentUTF8** :</span><span class="sxs-lookup"><span data-stu-id="d4baf-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContentUTF8** value:</span></span> 
  
1. <span data-ttu-id="d4baf-121">Texte du message — il s’agit du codage de corps, tel que ISO-2022-JP pour les caractères japonais.</span><span class="sxs-lookup"><span data-stu-id="d4baf-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="d4baf-122">Flux MIME : il s’agit du codage UTF8 du texte du message pour l’élément **MimeContentUTF8** , ou du codage ASCII du texte du message pour l’élément [lamimecontent](mimecontent.md) .</span><span class="sxs-lookup"><span data-stu-id="d4baf-122">MIME stream — This is the UTF8 encoding of the message text for the **MimeContentUTF8** element, or the ASCII encoding of the message text for the [MimeContent](mimecontent.md) element.</span></span> 
    
3. <span data-ttu-id="d4baf-123">Document XML : il s’agit toujours du flux ASCII encodé en base64 du flux MIME, où les caractères tels que « \< », qui sont significatifs en XML, sont masqués dans les analyseurs XML.</span><span class="sxs-lookup"><span data-stu-id="d4baf-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="d4baf-124">Chaque niveau est indépendant du niveau qui le précède.</span><span class="sxs-lookup"><span data-stu-id="d4baf-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="d4baf-125">L’élément **MimeContentUTF8** peut contenir les mêmes données que d’autres propriétés renvoyées avec un élément.</span><span class="sxs-lookup"><span data-stu-id="d4baf-125">The **MimeContentUTF8** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="d4baf-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4baf-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="d4baf-127">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="d4baf-127">Version differences</span></span>

<span data-ttu-id="d4baf-128">Cet élément est disponible dans les versions d’Exchange commençant par Build 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="d4baf-128">This element is available in versions of Exchange starting with build 15.00.0986.00.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4baf-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4baf-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4baf-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4baf-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4baf-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4baf-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d4baf-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4baf-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4baf-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4baf-133">Validation File</span></span>  <br/> |<span data-ttu-id="d4baf-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4baf-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4baf-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4baf-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4baf-136">False</span><span class="sxs-lookup"><span data-stu-id="d4baf-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4baf-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4baf-137">See also</span></span>



- [<span data-ttu-id="d4baf-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4baf-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

