---
title: ImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7b884e-ecf1-4e58-86ec-856b13a95f2b
description: L’élément ImGroup représente un groupe de messagerie instantané.
ms.openlocfilehash: 2a444158dbc6a73b1aee7b306cc251d33d005c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827890"
---
# <a name="imgroup"></a><span data-ttu-id="593dd-103">ImGroup</span><span class="sxs-lookup"><span data-stu-id="593dd-103">ImGroup</span></span>

<span data-ttu-id="593dd-104">L’élément **ImGroup** représente un groupe de messagerie instantané.</span><span class="sxs-lookup"><span data-stu-id="593dd-104">The **ImGroup** element represents an instant messaging group.</span></span> 
  
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

 <span data-ttu-id="593dd-105">**ImGroupType**</span><span class="sxs-lookup"><span data-stu-id="593dd-105">**ImGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="593dd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="593dd-106">Attributes and elements</span></span>

<span data-ttu-id="593dd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="593dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="593dd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="593dd-108">Attributes</span></span>

<span data-ttu-id="593dd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="593dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="593dd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="593dd-110">Child elements</span></span>

<span data-ttu-id="593dd-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)  |  [ SmtpAddress](smtpaddress.md)</span><span class="sxs-lookup"><span data-stu-id="593dd-111">[DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupType](grouptype.md) | [ExchangeStoreId](exchangestoreid.md) | [MemberCorrelationKey](membercorrelationkey.md) | [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md) | [SmtpAddress](smtpaddress.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="593dd-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="593dd-112">Parent elements</span></span>

<span data-ttu-id="593dd-113">[Groupes (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span><span class="sxs-lookup"><span data-stu-id="593dd-113">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md) | [AddImGroupResponse](addimgroupresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="593dd-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="593dd-114">Remarks</span></span>

<span data-ttu-id="593dd-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="593dd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="593dd-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="593dd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="593dd-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="593dd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="593dd-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="593dd-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="593dd-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="593dd-119">Schema name</span></span>  <br/> |<span data-ttu-id="593dd-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="593dd-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="593dd-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="593dd-121">Validation file</span></span>  <br/> |<span data-ttu-id="593dd-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="593dd-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="593dd-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="593dd-123">Can be empty</span></span>  <br/> ||
   

