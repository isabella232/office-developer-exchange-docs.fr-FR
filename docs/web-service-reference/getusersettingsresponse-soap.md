---
title: GetUserSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: L’élément GetUserSettingsResponse représente une réponse à une demande d’opération (SOAP) GetUserSettings.
ms.openlocfilehash: 24dbfb1582f628fd0130aa82ea5f1beedd31b156
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827705"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="2ccc0-103">GetUserSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ccc0-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="2ccc0-104">L’élément **GetUserSettingsResponse** représente une réponse à une demande de [l’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="2ccc0-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="2ccc0-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="2ccc0-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ccc0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ccc0-106">Attributes and elements</span></span>

<span data-ttu-id="2ccc0-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ccc0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ccc0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ccc0-108">Attributes</span></span>

<span data-ttu-id="2ccc0-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ccc0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ccc0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ccc0-110">Child elements</span></span>

|<span data-ttu-id="2ccc0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ccc0-111">**Element**</span></span>|<span data-ttu-id="2ccc0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ccc0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ccc0-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ccc0-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="2ccc0-114">Représente un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="2ccc0-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="2ccc0-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ccc0-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="2ccc0-116">Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="2ccc0-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="2ccc0-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ccc0-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="2ccc0-118">Contient les paramètres de configuration pour chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="2ccc0-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ccc0-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ccc0-119">Parent elements</span></span>

<span data-ttu-id="2ccc0-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ccc0-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2ccc0-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2ccc0-121">Text value</span></span>

<span data-ttu-id="2ccc0-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ccc0-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ccc0-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ccc0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ccc0-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ccc0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2ccc0-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ccc0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2ccc0-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2ccc0-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2ccc0-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ccc0-127">Validation File</span></span>  <br/> |<span data-ttu-id="2ccc0-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2ccc0-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ccc0-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ccc0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ccc0-130">True</span><span class="sxs-lookup"><span data-stu-id="2ccc0-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ccc0-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ccc0-131">See also</span></span>



[<span data-ttu-id="2ccc0-132">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2ccc0-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

