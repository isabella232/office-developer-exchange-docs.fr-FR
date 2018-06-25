---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: L’élément SearchPreviewItem Spécifie l’aperçu de l’élément pour une recherche de découverte.
ms.openlocfilehash: 46b9d6049f856ce6e93b9e49e07516ec4b52d932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829308"
---
# <a name="searchpreviewitem"></a><span data-ttu-id="70678-103">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="70678-103">SearchPreviewItem</span></span>

<span data-ttu-id="70678-104">L’élément **SearchPreviewItem** Spécifie l’aperçu de l’élément pour une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="70678-104">The **SearchPreviewItem** element specifies the item preview for a discovery search.</span></span> 
  
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

 <span data-ttu-id="70678-105">**SearchPreviewItemType**</span><span class="sxs-lookup"><span data-stu-id="70678-105">**SearchPreviewItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70678-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="70678-106">Attributes and elements</span></span>

<span data-ttu-id="70678-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="70678-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70678-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="70678-108">Attributes</span></span>

<span data-ttu-id="70678-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="70678-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70678-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="70678-110">Child elements</span></span>

<span data-ttu-id="70678-111">[ID (ItemIdType)](id-itemidtype.md) | [boîte aux lettres (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md)  |  [ L’expéditeur (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md)  |  [Heure d’envoi](senttime.md)  |  [Objet](subject.md) | [taille (longue)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [en lecture](read.md) | [HasAttachment](hasattachment.md) | [(ExtendedProperties NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span><span class="sxs-lookup"><span data-stu-id="70678-111">[ID (ItemIdType)](id-itemidtype.md) | [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md) | [ParentId](parentid.md) | [ItemClass](itemclass.md) | [UniqueHash](uniquehash.md) | [SortValue](sortvalue.md) | [OwaLink](owalink.md) | [Sender (string)](sender-string.md) | [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md) | [CcRecipients](ccrecipients.md) | [BccRecipients](bccrecipients.md) | [CreatedTime](createdtime.md) | [ReceivedTime](receivedtime.md) | [SentTime](senttime.md) | [Subject](subject.md) | [Size (long)](size-long.md) | [Preview](preview-ex15websvcsotherref.md) | [Importance](importance.md) | [Read](read.md) | [HasAttachment](hasattachment.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70678-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="70678-112">Parent elements</span></span>

[<span data-ttu-id="70678-113">Éléments (ArrayOfSearchPreviewItemsType)</span><span class="sxs-lookup"><span data-stu-id="70678-113">Items (ArrayOfSearchPreviewItemsType)</span></span>](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a><span data-ttu-id="70678-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="70678-114">Remarks</span></span>

<span data-ttu-id="70678-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="70678-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="70678-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="70678-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70678-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="70678-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70678-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="70678-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70678-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="70678-119">Schema name</span></span>  <br/> |<span data-ttu-id="70678-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="70678-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="70678-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="70678-121">Validation file</span></span>  <br/> |<span data-ttu-id="70678-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="70678-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70678-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="70678-123">Can be empty</span></span>  <br/> ||
   

