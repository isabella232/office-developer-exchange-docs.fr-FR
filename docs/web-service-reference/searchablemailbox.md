---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: L’élément SearchableMailbox spécifie une boîte aux lettres renvoyée à partir d’une demande GetSearchableMailboxes.
ms.openlocfilehash: f790d9a707f10f64a776b2fc35255c233ad854b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467451"
---
# <a name="searchablemailbox"></a><span data-ttu-id="563b5-103">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="563b5-103">SearchableMailbox</span></span>

<span data-ttu-id="563b5-104">L’élément **SearchableMailbox** spécifie une boîte aux lettres renvoyée à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="563b5-104">The **SearchableMailbox** element specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 <span data-ttu-id="563b5-105">**SearchableMailboxType**</span><span class="sxs-lookup"><span data-stu-id="563b5-105">**SearchableMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="563b5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="563b5-106">Attributes and elements</span></span>

<span data-ttu-id="563b5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="563b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="563b5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="563b5-108">Attributes</span></span>

<span data-ttu-id="563b5-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="563b5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="563b5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="563b5-110">Child elements</span></span>

<span data-ttu-id="563b5-111">[GUID](guid-ex15websvcsotherref.md)  |  [PrimarySmtpAddress (String)](primarysmtpaddress-string.md)  |  [IsExternalMailbox](isexternalmailbox.md)  |  [ExternalEmailAddress](externalemailaddress.md)  |  [DisplayName (String)](displayname-string.md)  |  [IsMembershipGroup](ismembershipgroup.md)  |  [ID](referenceid.md)</span><span class="sxs-lookup"><span data-stu-id="563b5-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md) | [ReferenceId](referenceid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="563b5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="563b5-112">Parent elements</span></span>

[<span data-ttu-id="563b5-113">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="563b5-113">SearchableMailboxes</span></span>](searchablemailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="563b5-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="563b5-114">Remarks</span></span>

<span data-ttu-id="563b5-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="563b5-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="563b5-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="563b5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="563b5-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="563b5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="563b5-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="563b5-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="563b5-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="563b5-119">Schema name</span></span>  <br/> |<span data-ttu-id="563b5-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="563b5-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="563b5-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="563b5-121">Validation file</span></span>  <br/> |<span data-ttu-id="563b5-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="563b5-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="563b5-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="563b5-123">Can be empty</span></span>  <br/> ||
   

