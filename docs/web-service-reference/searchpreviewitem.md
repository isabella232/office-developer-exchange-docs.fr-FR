---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: L’élément SearchPreviewItem spécifie l’aperçu de l’élément pour une recherche de découverte.
ms.openlocfilehash: ab48353b0ffaf4bc3b9409f1a620d145bffc7a13
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466933"
---
# <a name="searchpreviewitem"></a><span data-ttu-id="9391f-103">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="9391f-103">SearchPreviewItem</span></span>

<span data-ttu-id="9391f-104">L’élément **SearchPreviewItem** spécifie l’aperçu de l’élément pour une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="9391f-104">The **SearchPreviewItem** element specifies the item preview for a discovery search.</span></span> 
  
```XML
<SearchPreviewItem>
   <Id/>
   <Mailbox/>
   <ParentId/>
   <ItemClass/>
   <UniqueHash/>
   <SortValue/>
   <OwaLink/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <CreatedTime/>
   <ReceivedTime/>
   <SentTime/>
   <Subject/>
   <Size/>
   <Preview/>
   <Importance/>
   <Read/>
   <HasAttachment/>
   <ExtendedProperties/>
</SearchPreviewItem>
```

 <span data-ttu-id="9391f-105">**SearchPreviewItemType**</span><span class="sxs-lookup"><span data-stu-id="9391f-105">**SearchPreviewItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9391f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9391f-106">Attributes and elements</span></span>

<span data-ttu-id="9391f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9391f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9391f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9391f-108">Attributes</span></span>

<span data-ttu-id="9391f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9391f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9391f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9391f-110">Child elements</span></span>

<span data-ttu-id="9391f-111">[ID (ItemIdType)](id-itemidtype.md)  |  [Boîte aux lettres (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md)  |  [ParentId](parentid.md)  |  [ItemClass](itemclass.md)  |  [UniqueHash](uniquehash.md)  |  [SortValue](sortvalue.md)  |  [OwaLink](owalink.md)  |  [Sender (chaîne)](sender-string.md)  |  [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md)  |  [CCRecipients](ccrecipients.md)  |  [BCCRecipients](bccrecipients.md)  |  [CreatedTime](createdtime.md)  |  [ReceivedTime](receivedtime.md)  |  [SentTime](senttime.md)  |  [Objet](subject.md)  |  [Taille (long)](size-long.md)  |  [Aperçu](preview-ex15websvcsotherref.md)  |  [Importance](importance.md)  |  [En lecture](read.md)  |  [HasAttachment](hasattachment.md)  |  [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span><span class="sxs-lookup"><span data-stu-id="9391f-111">[ID (ItemIdType)](id-itemidtype.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md) | [Sender (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [Subject](subject.md) | [Size (long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [Read](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9391f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9391f-112">Parent elements</span></span>

[<span data-ttu-id="9391f-113">Items (ArrayOfSearchPreviewItemsType)</span><span class="sxs-lookup"><span data-stu-id="9391f-113">Items (ArrayOfSearchPreviewItemsType)</span></span>](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a><span data-ttu-id="9391f-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="9391f-114">Remarks</span></span>

<span data-ttu-id="9391f-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9391f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9391f-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9391f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9391f-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9391f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9391f-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9391f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9391f-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9391f-119">Schema name</span></span>  <br/> |<span data-ttu-id="9391f-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9391f-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="9391f-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9391f-121">Validation file</span></span>  <br/> |<span data-ttu-id="9391f-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9391f-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9391f-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9391f-123">Can be empty</span></span>  <br/> ||
   

