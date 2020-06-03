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
ms.openlocfilehash: db2bab16334b90395d29dc03353dce05b0e45357
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526745"
---
# <a name="userresponses-soap"></a><span data-ttu-id="2a09a-103">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2a09a-103">UserResponses (SOAP)</span></span>

<span data-ttu-id="2a09a-104">L’élément **UserResponses** contient les paramètres de configuration pour chaque utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="2a09a-104">The **UserResponses** element contains the configuration settings for each requested user.</span></span> 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 <span data-ttu-id="2a09a-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="2a09a-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a09a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2a09a-106">Attributes and elements</span></span>

<span data-ttu-id="2a09a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2a09a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a09a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2a09a-108">Attributes</span></span>

<span data-ttu-id="2a09a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2a09a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a09a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2a09a-110">Child elements</span></span>

|<span data-ttu-id="2a09a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2a09a-111">**Element**</span></span>|<span data-ttu-id="2a09a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2a09a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a09a-113">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2a09a-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="2a09a-114">Représente une réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) pour un utilisateur individuel.</span><span class="sxs-lookup"><span data-stu-id="2a09a-114">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a09a-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2a09a-115">Parent elements</span></span>

|<span data-ttu-id="2a09a-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2a09a-116">**Element**</span></span>|<span data-ttu-id="2a09a-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2a09a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a09a-118">Réponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2a09a-118">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="2a09a-119">Contient la réponse à une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="2a09a-119">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="2a09a-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2a09a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a09a-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2a09a-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2a09a-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2a09a-122">Schema Name</span></span>  <br/> |<span data-ttu-id="2a09a-123">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2a09a-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2a09a-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2a09a-124">Validation File</span></span>  <br/> |<span data-ttu-id="2a09a-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2a09a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2a09a-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2a09a-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a09a-127">True</span><span class="sxs-lookup"><span data-stu-id="2a09a-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a09a-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2a09a-128">See also</span></span>



[<span data-ttu-id="2a09a-129">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2a09a-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

