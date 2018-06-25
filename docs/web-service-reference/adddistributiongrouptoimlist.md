---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: L’élément AddDistributionGroupToImList définit une demande pour ajouter une liste de distribution à une liste de message instantané.
ms.openlocfilehash: b63daeb8b1d60123215bfcdec307f2f948d2ec39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755164"
---
# <a name="adddistributiongrouptoimlist"></a><span data-ttu-id="57cd1-103">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="57cd1-103">AddDistributionGroupToImList</span></span>

<span data-ttu-id="57cd1-104">L’élément **AddDistributionGroupToImList** définit une demande pour ajouter une liste de distribution à une liste de message instantané.</span><span class="sxs-lookup"><span data-stu-id="57cd1-104">The **AddDistributionGroupToImList** element defines a request to add a distribution list to an instant message list.</span></span> 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 <span data-ttu-id="57cd1-105">**AddDistributionGroupToImListType**</span><span class="sxs-lookup"><span data-stu-id="57cd1-105">**AddDistributionGroupToImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57cd1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="57cd1-106">Attributes and elements</span></span>

<span data-ttu-id="57cd1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="57cd1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57cd1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="57cd1-108">Attributes</span></span>

<span data-ttu-id="57cd1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="57cd1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57cd1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="57cd1-110">Child elements</span></span>

<span data-ttu-id="57cd1-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="57cd1-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57cd1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="57cd1-112">Parent elements</span></span>

<span data-ttu-id="57cd1-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="57cd1-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57cd1-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="57cd1-114">Remarks</span></span>

<span data-ttu-id="57cd1-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="57cd1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57cd1-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="57cd1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57cd1-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="57cd1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57cd1-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="57cd1-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57cd1-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="57cd1-119">Schema name</span></span>  <br/> |<span data-ttu-id="57cd1-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="57cd1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57cd1-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="57cd1-121">Validation file</span></span>  <br/> |<span data-ttu-id="57cd1-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="57cd1-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57cd1-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="57cd1-123">Can be empty</span></span>  <br/> |<span data-ttu-id="57cd1-124">false</span><span class="sxs-lookup"><span data-stu-id="57cd1-124">false</span></span>  <br/> |
   

