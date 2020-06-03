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
description: L’élément ExcludeConflicts spécifie s’il faut renvoyer les heures suggérées pour les heures de calendrier qui sont en conflit entre les participants.
ms.openlocfilehash: d20c594ae600abf110681ea678b2d95a23bf7809
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456975"
---
# <a name="excludeconflicts"></a><span data-ttu-id="8878d-103">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="8878d-103">ExcludeConflicts</span></span>

<span data-ttu-id="8878d-104">L’élément **ExcludeConflicts** spécifie s’il faut renvoyer les heures suggérées pour les heures de calendrier qui sont en conflit entre les participants.</span><span class="sxs-lookup"><span data-stu-id="8878d-104">The **ExcludeConflicts** element specifies whether to return suggested times for calendar times that conflict among the attendees.</span></span> 
  
[<span data-ttu-id="8878d-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="8878d-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="8878d-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="8878d-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
[<span data-ttu-id="8878d-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="8878d-107">MailboxData</span></span>](mailboxdata.md)
  
[<span data-ttu-id="8878d-108">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="8878d-108">ExcludeConflicts</span></span>](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
```

 <span data-ttu-id="8878d-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8878d-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8878d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8878d-110">Attributes and elements</span></span>

<span data-ttu-id="8878d-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8878d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8878d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="8878d-112">Attributes</span></span>

<span data-ttu-id="8878d-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8878d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8878d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8878d-114">Child elements</span></span>

<span data-ttu-id="8878d-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8878d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8878d-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8878d-116">Parent elements</span></span>

|<span data-ttu-id="8878d-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8878d-117">**Element**</span></span>|<span data-ttu-id="8878d-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="8878d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8878d-119">MailboxData</span><span class="sxs-lookup"><span data-stu-id="8878d-119">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="8878d-120">Représente un utilisateur et des options de boîte aux lettres individuelle pour le type de données à renvoyer à propos de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8878d-120">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="8878d-121">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="8878d-121">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8878d-122">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8878d-122">Text value</span></span>

<span data-ttu-id="8878d-123">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="8878d-123">A text value is required.</span></span> <span data-ttu-id="8878d-124">Les valeurs possibles sont Boolean **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="8878d-124">The possible values are a Boolean **true** or **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8878d-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="8878d-125">Remarks</span></span>

<span data-ttu-id="8878d-126">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="8878d-126">This element is required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8878d-127">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8878d-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8878d-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8878d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8878d-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8878d-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8878d-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8878d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="8878d-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8878d-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8878d-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8878d-132">Validation File</span></span>  <br/> |<span data-ttu-id="8878d-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8878d-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8878d-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8878d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="8878d-135">False</span><span class="sxs-lookup"><span data-stu-id="8878d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8878d-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8878d-136">See also</span></span>



[<span data-ttu-id="8878d-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8878d-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="8878d-138">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="8878d-138">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="8878d-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8878d-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

