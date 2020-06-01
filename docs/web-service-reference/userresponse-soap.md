---
title: UserResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: L’élément UserResponse représente une réponse à une demande GetUserSettings pour un utilisateur individuel.
ms.openlocfilehash: 73848cb19d9c859e07216f354965ac4051d0d20c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468900"
---
# <a name="userresponse-soap"></a><span data-ttu-id="f3d89-103">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-103">UserResponse (SOAP)</span></span>

<span data-ttu-id="f3d89-104">L’élément **UserResponse** représente une réponse à une demande GetUserSettings pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="f3d89-104">The **UserResponse** element represents a response to a GetUserSettings request for an individual user.</span></span> 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 <span data-ttu-id="f3d89-105">**UserResponse**</span><span class="sxs-lookup"><span data-stu-id="f3d89-105">**UserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3d89-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f3d89-106">Attributes and elements</span></span>

<span data-ttu-id="f3d89-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f3d89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3d89-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f3d89-108">Attributes</span></span>

<span data-ttu-id="f3d89-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f3d89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3d89-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f3d89-110">Child elements</span></span>

|<span data-ttu-id="f3d89-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f3d89-111">**Element**</span></span>|<span data-ttu-id="f3d89-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f3d89-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3d89-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="f3d89-114">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f3d89-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f3d89-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="f3d89-116">Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f3d89-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f3d89-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="f3d89-118">Contient la cible de l’URL de redirection ou de l’adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="f3d89-118">Contains the target of the redirection URL or email address.</span></span>  <br/> |
|[<span data-ttu-id="f3d89-119">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-119">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="f3d89-120">Représente une collection d’informations sur les paramètres qui n’ont pas pu être renvoyés.</span><span class="sxs-lookup"><span data-stu-id="f3d89-120">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="f3d89-121">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-121">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="f3d89-122">Paramètres demandés pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f3d89-122">The requested settings for the user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3d89-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f3d89-123">Parent elements</span></span>

|<span data-ttu-id="f3d89-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f3d89-124">**Element**</span></span>|<span data-ttu-id="f3d89-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="f3d89-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3d89-126">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-126">ArrayOfUserResponse (SOAP)</span></span>](arrayofuserresponse-soap.md) <br/> |<span data-ttu-id="f3d89-127">Contient un tableau des réponses de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f3d89-127">Contains an array of user responses.</span></span>  <br/> |
|[<span data-ttu-id="f3d89-128">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f3d89-128">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="f3d89-129">Contient les paramètres de configuration de chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="f3d89-129">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="f3d89-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f3d89-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3d89-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f3d89-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f3d89-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f3d89-132">Schema Name</span></span>  <br/> |<span data-ttu-id="f3d89-133">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="f3d89-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f3d89-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f3d89-134">Validation File</span></span>  <br/> |<span data-ttu-id="f3d89-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f3d89-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3d89-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f3d89-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3d89-137">True</span><span class="sxs-lookup"><span data-stu-id="f3d89-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3d89-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f3d89-138">See also</span></span>



[<span data-ttu-id="f3d89-139">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f3d89-139">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

