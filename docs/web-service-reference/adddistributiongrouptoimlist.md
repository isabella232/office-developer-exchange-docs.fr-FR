---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: L’élément AddDistributionGroupToImList définit une demande d’ajout d’une liste de distribution à une liste de messages instantanés.
ms.openlocfilehash: 90a84b23678fb0740158f601967905a8847286fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460378"
---
# <a name="adddistributiongrouptoimlist"></a><span data-ttu-id="9565d-103">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="9565d-103">AddDistributionGroupToImList</span></span>

<span data-ttu-id="9565d-104">L’élément **AddDistributionGroupToImList** définit une demande d’ajout d’une liste de distribution à une liste de messages instantanés.</span><span class="sxs-lookup"><span data-stu-id="9565d-104">The **AddDistributionGroupToImList** element defines a request to add a distribution list to an instant message list.</span></span> 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 <span data-ttu-id="9565d-105">**AddDistributionGroupToImListType**</span><span class="sxs-lookup"><span data-stu-id="9565d-105">**AddDistributionGroupToImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9565d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9565d-106">Attributes and elements</span></span>

<span data-ttu-id="9565d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9565d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9565d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9565d-108">Attributes</span></span>

<span data-ttu-id="9565d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9565d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9565d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9565d-110">Child elements</span></span>

<span data-ttu-id="9565d-111">[SmtpAddress](smtpaddress.md)  |  [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="9565d-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9565d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9565d-112">Parent elements</span></span>

<span data-ttu-id="9565d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9565d-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9565d-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="9565d-114">Remarks</span></span>

<span data-ttu-id="9565d-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9565d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9565d-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9565d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9565d-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9565d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9565d-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9565d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9565d-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9565d-119">Schema name</span></span>  <br/> |<span data-ttu-id="9565d-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9565d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9565d-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9565d-121">Validation file</span></span>  <br/> |<span data-ttu-id="9565d-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9565d-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9565d-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9565d-123">Can be empty</span></span>  <br/> |<span data-ttu-id="9565d-124">false</span><span class="sxs-lookup"><span data-stu-id="9565d-124">false</span></span>  <br/> |
   

