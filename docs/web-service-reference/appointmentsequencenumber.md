---
title: AppointmentSequenceNumber
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentSequenceNumber
api_type:
- schema
ms.assetid: eb4c48bd-f905-48dc-ae16-53a080b9b025
description: L’élément AppointmentSequenceNumber Spécifie le numéro de séquence d’une version d’un rendez-vous.
ms.openlocfilehash: bc186170ccca06669ea7d20cea06c542f9ce274a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755304"
---
# <a name="appointmentsequencenumber"></a><span data-ttu-id="ec778-103">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="ec778-103">AppointmentSequenceNumber</span></span>

<span data-ttu-id="ec778-104">L’élément **AppointmentSequenceNumber** Spécifie le numéro de séquence d’une version d’un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="ec778-104">The **AppointmentSequenceNumber** element specifies the sequence number of a version of an appointment.</span></span> 
  
```xml
<AppointmentSequenceNumber/>
```

 <span data-ttu-id="ec778-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ec778-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec778-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ec778-106">Attributes and elements</span></span>

<span data-ttu-id="ec778-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ec778-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec778-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ec778-108">Attributes</span></span>

<span data-ttu-id="ec778-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec778-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec778-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ec778-110">Child elements</span></span>

<span data-ttu-id="ec778-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec778-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec778-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ec778-112">Parent elements</span></span>

|<span data-ttu-id="ec778-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec778-113">**Element**</span></span>|<span data-ttu-id="ec778-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec778-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec778-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ec778-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ec778-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec778-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ec778-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ec778-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ec778-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec778-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec778-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ec778-119">Text value</span></span>

<span data-ttu-id="ec778-120">La valeur de texte représente un numéro de version.</span><span class="sxs-lookup"><span data-stu-id="ec778-120">The text value represents a version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec778-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="ec778-121">Remarks</span></span>

<span data-ttu-id="ec778-122">Cette valeur est mis à jour lorsque le rendez-vous est mis à jour avec de nouvelles informations.</span><span class="sxs-lookup"><span data-stu-id="ec778-122">This value is updated when the appointment is updated with new information.</span></span> 
  
<span data-ttu-id="ec778-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ec778-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec778-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ec778-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec778-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ec778-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ec778-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ec778-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ec778-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ec778-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ec778-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ec778-128">Validation File</span></span>  <br/> |<span data-ttu-id="ec778-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ec778-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ec778-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ec778-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec778-131">False</span><span class="sxs-lookup"><span data-stu-id="ec778-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec778-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec778-132">See also</span></span>

- [<span data-ttu-id="ec778-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ec778-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

