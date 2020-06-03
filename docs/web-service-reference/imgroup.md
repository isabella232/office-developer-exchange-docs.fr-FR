---
title: Imgroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: L’élément imgroup représente un groupe de messagerie instantanée.
ms.openlocfilehash: a0ff3fcb82e7f18837af5a6f5daa16e90043034d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460686"
---
# <a name="imgroup"></a><span data-ttu-id="50a6b-103">Imgroup</span><span class="sxs-lookup"><span data-stu-id="50a6b-103">ImGroup</span></span>

<span data-ttu-id="50a6b-104">L’élément **imgroup** représente un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="50a6b-104">The **ImGroup** element represents an instant messaging group.</span></span> 
  
```XML
<ImGroup>
   <DisplayName/>
   <GroupType/>
   <ExchangeStoreId/>
   <MemberCorrelationKey/>
   <ExtendedProperties/>
   <SmtpAddress/>
</ImGroup>
```

 <span data-ttu-id="50a6b-105">**ImGroupType**</span><span class="sxs-lookup"><span data-stu-id="50a6b-105">**ImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50a6b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="50a6b-106">Attributes and elements</span></span>

<span data-ttu-id="50a6b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="50a6b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50a6b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="50a6b-108">Attributes</span></span>

<span data-ttu-id="50a6b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="50a6b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50a6b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="50a6b-110">Child elements</span></span>

<span data-ttu-id="50a6b-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)  |  [GroupType](grouptype.md)  |  [ExchangeStoreId](exchangestoreid.md)  |  [MemberCorrelationKey](membercorrelationkey.md)  |  [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  |  [SmtpAddress](smtpaddress.md)</span><span class="sxs-lookup"><span data-stu-id="50a6b-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="50a6b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="50a6b-112">Parent elements</span></span>

<span data-ttu-id="50a6b-113">[Groupes (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)  |  [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)  |  [AddImGroupResponse](addimgroupresponse.md)</span><span class="sxs-lookup"><span data-stu-id="50a6b-113">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="50a6b-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="50a6b-114">Remarks</span></span>

<span data-ttu-id="50a6b-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="50a6b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="50a6b-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="50a6b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50a6b-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="50a6b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50a6b-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="50a6b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50a6b-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="50a6b-119">Schema name</span></span>  <br/> |<span data-ttu-id="50a6b-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="50a6b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="50a6b-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="50a6b-121">Validation file</span></span>  <br/> |<span data-ttu-id="50a6b-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="50a6b-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50a6b-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="50a6b-123">Can be empty</span></span>  <br/> ||
   

