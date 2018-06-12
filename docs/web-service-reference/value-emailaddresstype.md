---
title: Valeur (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 24eaa473-0024-47e2-b7d2-051d5dd4f53c
description: L’élément Value spécifie la valeur d’un EmailAddress associé à un tableau des attributions.
ms.openlocfilehash: 097444d90e98e73b9e83912274ecf87249008116
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838997"
---
# <a name="value-emailaddresstype"></a><span data-ttu-id="cdbfe-103">Valeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="cdbfe-103">Value (EmailAddressType)</span></span>

<span data-ttu-id="cdbfe-104">L’élément **Value** Spécifie que la valeur d’une **adresse électronique** associé à un tableau des attributions.</span><span class="sxs-lookup"><span data-stu-id="cdbfe-104">The **Value** element specifies the value of an **EmailAddress** associated with an attributions array.</span></span> 
  
```XML
<Value>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
   <OriginalDisplayName/>
</Value>
```

<span data-ttu-id="cdbfe-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="cdbfe-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cdbfe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cdbfe-106">Attributes and elements</span></span>

<span data-ttu-id="cdbfe-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cdbfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cdbfe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cdbfe-108">Attributes</span></span>

<span data-ttu-id="cdbfe-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cdbfe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cdbfe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cdbfe-110">Child elements</span></span>

<span data-ttu-id="cdbfe-111">[Name (chaîne)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span><span class="sxs-lookup"><span data-stu-id="cdbfe-111">[Name (string)](name-string.md) | [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) | [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) | [MailboxType](mailboxtype.md) | [ItemId](itemid.md) | [OriginalDisplayName](originaldisplayname.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cdbfe-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cdbfe-112">Parent elements</span></span>

[<span data-ttu-id="cdbfe-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="cdbfe-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="cdbfe-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="cdbfe-114">Remarks</span></span>

<span data-ttu-id="cdbfe-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cdbfe-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cdbfe-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cdbfe-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cdbfe-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cdbfe-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cdbfe-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cdbfe-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cdbfe-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cdbfe-119">Schema name</span></span>  <br/> |<span data-ttu-id="cdbfe-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cdbfe-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="cdbfe-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cdbfe-121">Validation file</span></span>  <br/> |<span data-ttu-id="cdbfe-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cdbfe-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cdbfe-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cdbfe-123">Can be empty</span></span>  <br/> |<span data-ttu-id="cdbfe-124">false</span><span class="sxs-lookup"><span data-stu-id="cdbfe-124">false</span></span>  <br/> |
   

