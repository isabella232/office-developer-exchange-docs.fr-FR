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
description: L’élément GetServerTimeZones est l’élément racine dans une requête pour récupérer les définitions de fuseau horaire à partir du serveur Exchange.
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756746"
---
# <a name="getservertimezones"></a><span data-ttu-id="4008d-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="4008d-103">GetServerTimeZones</span></span>

<span data-ttu-id="4008d-104">L’élément **GetServerTimeZones** est l’élément racine dans une requête pour récupérer les définitions de fuseau horaire à partir du serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4008d-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="4008d-105">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="4008d-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4008d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4008d-106">Attributes and elements</span></span>

<span data-ttu-id="4008d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4008d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4008d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4008d-108">Attributes</span></span>

|<span data-ttu-id="4008d-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4008d-109">**Attribute**</span></span>|<span data-ttu-id="4008d-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="4008d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4008d-111">**ReturnFullTimeZoneData**</span><span class="sxs-lookup"><span data-stu-id="4008d-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="4008d-112">Spécifie si l' [opération GetServerTimeZones](getservertimezones-operation.md) renvoie la définition complète ou uniquement le nom et l’identificateur pour chaque fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="4008d-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="4008d-113">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="4008d-113">This attribute is optional.</span></span> <span data-ttu-id="4008d-114">La valeur par défaut est **true**.</span><span class="sxs-lookup"><span data-stu-id="4008d-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="4008d-115">Attribut ReturnFullTimeZoneData</span><span class="sxs-lookup"><span data-stu-id="4008d-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="4008d-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4008d-116">**Value**</span></span>|<span data-ttu-id="4008d-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4008d-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4008d-118">**valeur True**</span><span class="sxs-lookup"><span data-stu-id="4008d-118">**true**</span></span> <br/> |<span data-ttu-id="4008d-119">Renvoyer les définitions complètes pour chaque fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="4008d-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="4008d-120">**False**</span><span class="sxs-lookup"><span data-stu-id="4008d-120">**false**</span></span> <br/> |<span data-ttu-id="4008d-121">Retourner uniquement le nom et l’identificateur de chaque fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="4008d-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4008d-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4008d-122">Child elements</span></span>

|<span data-ttu-id="4008d-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4008d-123">**Element**</span></span>|<span data-ttu-id="4008d-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="4008d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4008d-125">ID</span><span class="sxs-lookup"><span data-stu-id="4008d-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="4008d-126">Contient un tableau d’identificateurs de définition de fuseau horaire qui spécifie les définitions de fuseau horaire demandé.</span><span class="sxs-lookup"><span data-stu-id="4008d-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="4008d-127">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="4008d-127">This element is optional.</span></span> <span data-ttu-id="4008d-128">Si cet élément n’est pas inclus dans la requête [d’opération GetServerTimeZones](getservertimezones-operation.md) , toutes les définitions de fuseau horaire sont disponibles sur le serveur sont renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="4008d-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4008d-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4008d-129">Parent elements</span></span>

<span data-ttu-id="4008d-130">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4008d-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4008d-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="4008d-131">Remarks</span></span>

<span data-ttu-id="4008d-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4008d-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4008d-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4008d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4008d-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4008d-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4008d-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4008d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="4008d-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4008d-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4008d-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4008d-137">Validation File</span></span>  <br/> |<span data-ttu-id="4008d-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4008d-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4008d-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4008d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="4008d-140">False</span><span class="sxs-lookup"><span data-stu-id="4008d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4008d-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4008d-141">See also</span></span>



[<span data-ttu-id="4008d-142">Opération GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="4008d-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="4008d-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="4008d-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="4008d-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4008d-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

