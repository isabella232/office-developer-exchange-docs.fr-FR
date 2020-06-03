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
description: L’élément GetUserSettingsResponse représente une réponse à une demande SOAP (GetUserSettings Operation).
ms.openlocfilehash: a41a195a003789ddaef81f844e47aad689df0937
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530147"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="130cc-103">GetUserSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="130cc-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="130cc-104">L’élément **GetUserSettingsResponse** représente une réponse à une demande [SOAP (GetUserSettings Operation)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="130cc-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="130cc-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="130cc-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="130cc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="130cc-106">Attributes and elements</span></span>

<span data-ttu-id="130cc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="130cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="130cc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="130cc-108">Attributes</span></span>

<span data-ttu-id="130cc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="130cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="130cc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="130cc-110">Child elements</span></span>

|<span data-ttu-id="130cc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="130cc-111">**Element**</span></span>|<span data-ttu-id="130cc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="130cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="130cc-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="130cc-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="130cc-114">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="130cc-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="130cc-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="130cc-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="130cc-116">Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="130cc-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="130cc-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="130cc-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="130cc-118">Contient les paramètres de configuration de chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="130cc-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="130cc-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="130cc-119">Parent elements</span></span>

<span data-ttu-id="130cc-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="130cc-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="130cc-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="130cc-121">Text value</span></span>

<span data-ttu-id="130cc-122">Aucune.</span><span class="sxs-lookup"><span data-stu-id="130cc-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="130cc-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="130cc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="130cc-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="130cc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="130cc-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="130cc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="130cc-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="130cc-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="130cc-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="130cc-127">Validation File</span></span>  <br/> |<span data-ttu-id="130cc-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="130cc-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="130cc-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="130cc-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="130cc-130">True</span><span class="sxs-lookup"><span data-stu-id="130cc-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="130cc-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="130cc-131">See also</span></span>



[<span data-ttu-id="130cc-132">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="130cc-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

