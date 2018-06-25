---
title: EmailAddresses (ArrayOfEmailAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: L’élément EmailAddresses spécifie un tableau de toutes les adresses de messagerie du personnage associé.
ms.openlocfilehash: 292d4c3f12b01f25fd094b2ab6d9c2d484d37694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756118"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="37823-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="37823-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="37823-104">L’élément **EmailAddresses** spécifie un tableau de toutes les adresses de messagerie du personnage associé.</span><span class="sxs-lookup"><span data-stu-id="37823-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="37823-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="37823-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37823-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="37823-106">Attributes and elements</span></span>

<span data-ttu-id="37823-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="37823-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37823-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="37823-108">Attributes</span></span>

<span data-ttu-id="37823-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37823-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37823-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="37823-110">Child elements</span></span>

|<span data-ttu-id="37823-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37823-111">**Element**</span></span>|<span data-ttu-id="37823-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="37823-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37823-113">Adresse (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="37823-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="37823-114">Représente une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="37823-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37823-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="37823-115">Parent elements</span></span>

|<span data-ttu-id="37823-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37823-116">**Element**</span></span>|<span data-ttu-id="37823-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="37823-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37823-118">Personnage</span><span class="sxs-lookup"><span data-stu-id="37823-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="37823-119">Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="37823-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="37823-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="37823-120">Remarks</span></span>

<span data-ttu-id="37823-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="37823-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="37823-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="37823-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37823-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="37823-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37823-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="37823-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37823-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="37823-125">Schema Name</span></span>  <br/> |<span data-ttu-id="37823-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="37823-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="37823-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="37823-127">Validation File</span></span>  <br/> |<span data-ttu-id="37823-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="37823-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="37823-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="37823-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="37823-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="37823-130">See also</span></span>



- [<span data-ttu-id="37823-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="37823-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

