---
title: UserResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a48766df-4cc8-47c2-a8c1-826daec94e5a
description: L’élément UserResponses contient les paramètres de configuration pour chaque utilisateur demandé.
ms.openlocfilehash: bee7f3c9a95c1facfe0adc990516dfa323d9c8cf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838971"
---
# <a name="userresponses-soap"></a><span data-ttu-id="857ef-103">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="857ef-103">UserResponses (SOAP)</span></span>

<span data-ttu-id="857ef-104">L’élément **UserResponses** contient les paramètres de configuration pour chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="857ef-104">The **UserResponses** element contains the configuration settings for each requested user.</span></span> 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 <span data-ttu-id="857ef-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="857ef-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="857ef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="857ef-106">Attributes and elements</span></span>

<span data-ttu-id="857ef-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="857ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="857ef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="857ef-108">Attributes</span></span>

<span data-ttu-id="857ef-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="857ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="857ef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="857ef-110">Child elements</span></span>

|<span data-ttu-id="857ef-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="857ef-111">**Element**</span></span>|<span data-ttu-id="857ef-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="857ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="857ef-113">Réponse de l’utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="857ef-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="857ef-114">Représente une réponse à une demande de [l’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="857ef-114">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="857ef-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="857ef-115">Parent elements</span></span>

|<span data-ttu-id="857ef-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="857ef-116">**Element**</span></span>|<span data-ttu-id="857ef-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="857ef-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="857ef-118">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="857ef-118">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="857ef-119">Contient la réponse à une demande [d’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="857ef-119">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="857ef-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="857ef-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="857ef-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="857ef-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="857ef-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="857ef-122">Schema Name</span></span>  <br/> |<span data-ttu-id="857ef-123">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="857ef-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="857ef-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="857ef-124">Validation File</span></span>  <br/> |<span data-ttu-id="857ef-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="857ef-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="857ef-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="857ef-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="857ef-127">True</span><span class="sxs-lookup"><span data-stu-id="857ef-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="857ef-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="857ef-128">See also</span></span>



[<span data-ttu-id="857ef-129">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="857ef-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

