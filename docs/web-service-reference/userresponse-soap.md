---
title: Réponse de l’utilisateur (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: L’élément de réponse utilisateur représente une réponse à une demande de GetUserSettings pour un utilisateur individuel.
ms.openlocfilehash: 6fcd82e06916df5acdd317cb44161c1b69e58574
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19838972"
---
# <a name="userresponse-soap"></a><span data-ttu-id="8f662-103">Réponse de l’utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-103">UserResponse (SOAP)</span></span>

<span data-ttu-id="8f662-104">L’élément de **réponse utilisateur** représente une réponse à une demande de GetUserSettings pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="8f662-104">The **UserResponse** element represents a response to a GetUserSettings request for an individual user.</span></span> 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 <span data-ttu-id="8f662-105">**Réponse utilisateur**</span><span class="sxs-lookup"><span data-stu-id="8f662-105">**UserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f662-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8f662-106">Attributes and elements</span></span>

<span data-ttu-id="8f662-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8f662-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f662-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8f662-108">Attributes</span></span>

<span data-ttu-id="8f662-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8f662-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f662-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8f662-110">Child elements</span></span>

|<span data-ttu-id="8f662-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8f662-111">**Element**</span></span>|<span data-ttu-id="8f662-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8f662-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f662-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="8f662-114">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="8f662-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="8f662-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="8f662-116">Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="8f662-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="8f662-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="8f662-118">Contient la cible de la redirection URL ou l’adresse électronique.</span><span class="sxs-lookup"><span data-stu-id="8f662-118">Contains the target of the redirection URL or email address.</span></span>  <br/> |
|[<span data-ttu-id="8f662-119">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-119">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="8f662-120">Représente une collection d’informations sur les paramètres qui ne peut pas être retourné.</span><span class="sxs-lookup"><span data-stu-id="8f662-120">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="8f662-121">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-121">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="8f662-122">Les paramètres requis pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8f662-122">The requested settings for the user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f662-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8f662-123">Parent elements</span></span>

|<span data-ttu-id="8f662-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8f662-124">**Element**</span></span>|<span data-ttu-id="8f662-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="8f662-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f662-126">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-126">ArrayOfUserResponse (SOAP)</span></span>](arrayofuserresponse-soap.md) <br/> |<span data-ttu-id="8f662-127">Contient un tableau des réponses de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8f662-127">Contains an array of user responses.</span></span>  <br/> |
|[<span data-ttu-id="8f662-128">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8f662-128">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="8f662-129">Contient les paramètres de configuration pour chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="8f662-129">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="8f662-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8f662-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f662-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8f662-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8f662-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8f662-132">Schema Name</span></span>  <br/> |<span data-ttu-id="8f662-133">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="8f662-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8f662-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8f662-134">Validation File</span></span>  <br/> |<span data-ttu-id="8f662-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8f662-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8f662-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8f662-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f662-137">True</span><span class="sxs-lookup"><span data-stu-id="8f662-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f662-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8f662-138">See also</span></span>



[<span data-ttu-id="8f662-139">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8f662-139">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

