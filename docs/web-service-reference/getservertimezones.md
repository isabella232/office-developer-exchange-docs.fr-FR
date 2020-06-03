---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: L’élément GetServerTimeZones est l’élément racine dans une demande pour récupérer des définitions de fuseau horaire à partir du serveur Exchange.
ms.openlocfilehash: 797e4543c94b0628242bcf544fe9a735ebaa5a63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460938"
---
# <a name="getservertimezones"></a><span data-ttu-id="b243f-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="b243f-103">GetServerTimeZones</span></span>

<span data-ttu-id="b243f-104">L’élément **GetServerTimeZones** est l’élément racine dans une demande pour récupérer des définitions de fuseau horaire à partir du serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b243f-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="b243f-105">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="b243f-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b243f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b243f-106">Attributes and elements</span></span>

<span data-ttu-id="b243f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b243f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b243f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b243f-108">Attributes</span></span>

|<span data-ttu-id="b243f-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b243f-109">**Attribute**</span></span>|<span data-ttu-id="b243f-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b243f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b243f-111">**ReturnFullTimeZoneData**</span><span class="sxs-lookup"><span data-stu-id="b243f-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="b243f-112">Indique si l' [opération GetServerTimeZones](getservertimezones-operation.md) renvoie la définition complète ou uniquement le nom et l’identificateur de chaque fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="b243f-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="b243f-113">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="b243f-113">This attribute is optional.</span></span> <span data-ttu-id="b243f-114">La valeur par défaut est **true**.</span><span class="sxs-lookup"><span data-stu-id="b243f-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="b243f-115">Attribut ReturnFullTimeZoneData</span><span class="sxs-lookup"><span data-stu-id="b243f-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="b243f-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b243f-116">**Value**</span></span>|<span data-ttu-id="b243f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b243f-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b243f-118">**a**</span><span class="sxs-lookup"><span data-stu-id="b243f-118">**true**</span></span> <br/> |<span data-ttu-id="b243f-119">Renvoyer les définitions complètes de chaque fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="b243f-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="b243f-120">**true**</span><span class="sxs-lookup"><span data-stu-id="b243f-120">**false**</span></span> <br/> |<span data-ttu-id="b243f-121">Ne renvoyer que le nom et l’identificateur de chaque fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="b243f-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b243f-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b243f-122">Child elements</span></span>

|<span data-ttu-id="b243f-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b243f-123">**Element**</span></span>|<span data-ttu-id="b243f-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="b243f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b243f-125">Codes</span><span class="sxs-lookup"><span data-stu-id="b243f-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="b243f-126">Contient un tableau d’identificateurs de définition de fuseau horaire qui spécifie les définitions de fuseau horaire demandées.</span><span class="sxs-lookup"><span data-stu-id="b243f-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="b243f-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="b243f-127">This element is optional.</span></span> <span data-ttu-id="b243f-128">Si cet élément n’est pas inclus dans la demande d' [opération GetServerTimeZones](getservertimezones-operation.md) , toutes les définitions de fuseau horaire qui sont disponibles sur le serveur sont renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b243f-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b243f-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b243f-129">Parent elements</span></span>

<span data-ttu-id="b243f-130">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b243f-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b243f-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="b243f-131">Remarks</span></span>

<span data-ttu-id="b243f-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b243f-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b243f-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b243f-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b243f-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b243f-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b243f-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b243f-135">Schema Name</span></span>  <br/> |<span data-ttu-id="b243f-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b243f-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b243f-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b243f-137">Validation File</span></span>  <br/> |<span data-ttu-id="b243f-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b243f-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b243f-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b243f-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="b243f-140">False</span><span class="sxs-lookup"><span data-stu-id="b243f-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b243f-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b243f-141">See also</span></span>



[<span data-ttu-id="b243f-142">Opération GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="b243f-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="b243f-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="b243f-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="b243f-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b243f-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

