---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: L’élément OofSettings contient les paramètres d’absence du bureau (OOF).
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828649"
---
# <a name="oofsettings"></a><span data-ttu-id="98633-103">OofSettings</span><span class="sxs-lookup"><span data-stu-id="98633-103">OofSettings</span></span>

<span data-ttu-id="98633-104">L’élément **OofSettings** contient les paramètres d’absence du bureau (OOF).</span><span class="sxs-lookup"><span data-stu-id="98633-104">The **OofSettings** element contains the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="98633-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="98633-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
[<span data-ttu-id="98633-106">OofSettings</span><span class="sxs-lookup"><span data-stu-id="98633-106">OofSettings</span></span>](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 <span data-ttu-id="98633-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="98633-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98633-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="98633-108">Attributes and elements</span></span>

<span data-ttu-id="98633-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="98633-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98633-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="98633-110">Attributes</span></span>

<span data-ttu-id="98633-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98633-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98633-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="98633-112">Child elements</span></span>

|<span data-ttu-id="98633-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="98633-113">**Element**</span></span>|<span data-ttu-id="98633-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="98633-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98633-115">OofState</span><span class="sxs-lookup"><span data-stu-id="98633-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="98633-116">Contient l’état d’absence du bureau de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="98633-116">Contains the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="98633-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="98633-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="98633-118">Contient une valeur qui détermine les messages d’absence du bureau externes qui sont envoyés.</span><span class="sxs-lookup"><span data-stu-id="98633-118">Contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="98633-119">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="98633-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="98633-120">Affiche la durée pour laquelle le statut d’absence du bureau est activé si l’élément [OofState](oofstate.md) est défini sur **planifiées**.</span><span class="sxs-lookup"><span data-stu-id="98633-120">Contains the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="98633-121">Si l’élément [OofState](oofstate.md) est défini sur **activé** ou **désactivé**, la valeur de cet élément est ignorée.</span><span class="sxs-lookup"><span data-stu-id="98633-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="98633-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="98633-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="98633-123">Contient la réponse d’absence du bureau envoyée à d’autres utilisateurs dans un domaine ou domaine approuvé de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="98633-123">Contains the OOF response sent to other users in the user's domain or trusted domain.</span></span>  <br/> |
|[<span data-ttu-id="98633-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="98633-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="98633-125">Contient la réponse d’absence du bureau envoyée aux adresses à l’extérieur du destinataire ou les domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="98633-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="98633-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="98633-126">Parent elements</span></span>

|<span data-ttu-id="98633-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="98633-127">**Element**</span></span>|<span data-ttu-id="98633-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="98633-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98633-129">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="98633-129">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="98633-130">Contient les résultats de la réponse et les paramètres d’absence du bureau pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="98633-130">Contains the response results and the OOF settings for a user.</span></span>  <br/> <span data-ttu-id="98633-131">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="98633-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="98633-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="98633-132">Remarks</span></span>

<span data-ttu-id="98633-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="98633-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98633-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="98633-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98633-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="98633-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98633-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="98633-136">Schema Name</span></span>  <br/> |<span data-ttu-id="98633-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="98633-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98633-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="98633-138">Validation File</span></span>  <br/> |<span data-ttu-id="98633-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="98633-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98633-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="98633-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="98633-141">False</span><span class="sxs-lookup"><span data-stu-id="98633-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98633-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="98633-142">See also</span></span>



[<span data-ttu-id="98633-143">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="98633-143">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="98633-144">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="98633-144">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

