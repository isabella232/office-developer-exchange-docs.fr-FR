---
title: ExcludeConflicts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExcludeConflicts
api_type:
- schema
ms.assetid: ec33ef23-8537-41eb-8d89-7eb906a1fad7
description: L’élément ExcludeConflicts Spécifie s’il faut renvoyer suggérées heures de temps de calendrier en conflit entre les participants.
ms.openlocfilehash: 66b69d57246942e551de2f683949870823e2e4e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756244"
---
# <a name="excludeconflicts"></a><span data-ttu-id="bb4ca-103">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="bb4ca-103">ExcludeConflicts</span></span>

<span data-ttu-id="bb4ca-104">L’élément **ExcludeConflicts** Spécifie s’il faut renvoyer suggérées heures de temps de calendrier en conflit entre les participants.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="bb4ca-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="bb4ca-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="bb4ca-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="bb4ca-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="bb4ca-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="bb4ca-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="bb4ca-108">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="bb4ca-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="bb4ca-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bb4ca-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb4ca-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bb4ca-110">Attributes and elements</span></span>

<span data-ttu-id="bb4ca-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb4ca-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="bb4ca-112">Attributes</span></span>

<span data-ttu-id="bb4ca-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb4ca-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bb4ca-114">Child elements</span></span>

<span data-ttu-id="bb4ca-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb4ca-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bb4ca-116">Parent elements</span></span>

|<span data-ttu-id="bb4ca-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb4ca-117">**Element**</span></span>|<span data-ttu-id="bb4ca-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb4ca-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb4ca-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="bb4ca-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="bb4ca-120">Représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="bb4ca-121">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="bb4ca-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bb4ca-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bb4ca-122">Text value</span></span>

<span data-ttu-id="bb4ca-123">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-123">A text value is required.</span></span> <span data-ttu-id="bb4ca-124">Les valeurs possibles sont une valeur booléenne **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb4ca-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="bb4ca-125">Remarks</span></span>

<span data-ttu-id="bb4ca-126">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="bb4ca-127">Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="bb4ca-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="bb4ca-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bb4ca-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb4ca-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bb4ca-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb4ca-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bb4ca-130">Schema Name</span></span>  <br/> |<span data-ttu-id="bb4ca-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bb4ca-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb4ca-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bb4ca-132">Validation File</span></span>  <br/> |<span data-ttu-id="bb4ca-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bb4ca-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb4ca-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bb4ca-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb4ca-135">False</span><span class="sxs-lookup"><span data-stu-id="bb4ca-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb4ca-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bb4ca-136">See also</span></span>



[<span data-ttu-id="bb4ca-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="bb4ca-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="bb4ca-138">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="bb4ca-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="bb4ca-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="bb4ca-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

