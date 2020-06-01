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
description: L’élément OofSettings contient les paramètres absent (absent (e) du bureau.
ms.openlocfilehash: c1b214fd8bfab5b7a82d41a5187cf6e0fc4ba79c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467192"
---
# <a name="oofsettings"></a><span data-ttu-id="8ea2b-103">OofSettings</span><span class="sxs-lookup"><span data-stu-id="8ea2b-103">OofSettings</span></span>

<span data-ttu-id="8ea2b-104">L’élément **OofSettings** contient les paramètres absent (absent (e) du bureau.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-104">The **OofSettings** element contains the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="8ea2b-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="8ea2b-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
[<span data-ttu-id="8ea2b-106">OofSettings</span><span class="sxs-lookup"><span data-stu-id="8ea2b-106">OofSettings</span></span>](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 <span data-ttu-id="8ea2b-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="8ea2b-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ea2b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8ea2b-108">Attributes and elements</span></span>

<span data-ttu-id="8ea2b-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ea2b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="8ea2b-110">Attributes</span></span>

<span data-ttu-id="8ea2b-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ea2b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8ea2b-112">Child elements</span></span>

|<span data-ttu-id="8ea2b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8ea2b-113">**Element**</span></span>|<span data-ttu-id="8ea2b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ea2b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ea2b-115">OofState</span><span class="sxs-lookup"><span data-stu-id="8ea2b-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="8ea2b-116">Contient l’état d’absence du Bureau de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-116">Contains the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="8ea2b-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="8ea2b-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="8ea2b-118">Contient une valeur qui détermine à qui les messages externes OOF sont envoyés.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-118">Contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="8ea2b-119">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="8ea2b-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="8ea2b-120">Contient la durée pendant laquelle l’état du Bureau d’absence est activé si l’élément [OofState](oofstate.md) est défini sur **Planifié**.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-120">Contains the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="8ea2b-121">Si l’élément [OofState](oofstate.md) est défini sur **Enabled** ou **Disabled**, la valeur de cet élément est ignorée.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="8ea2b-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="8ea2b-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="8ea2b-123">Contient la réponse OOF envoyée aux autres utilisateurs du domaine de l’utilisateur ou du domaine approuvé.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-123">Contains the OOF response sent to other users in the user's domain or trusted domain.</span></span>  <br/> |
|[<span data-ttu-id="8ea2b-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="8ea2b-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="8ea2b-125">Contient la réponse OOF envoyée aux adresses en dehors du domaine du destinataire ou des domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8ea2b-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8ea2b-126">Parent elements</span></span>

|<span data-ttu-id="8ea2b-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8ea2b-127">**Element**</span></span>|<span data-ttu-id="8ea2b-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ea2b-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ea2b-129">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="8ea2b-129">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="8ea2b-130">Contient les résultats de la réponse et les paramètres OOF d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-130">Contains the response results and the OOF settings for a user.</span></span>  <br/> <span data-ttu-id="8ea2b-131">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="8ea2b-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8ea2b-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="8ea2b-132">Remarks</span></span>

<span data-ttu-id="8ea2b-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8ea2b-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ea2b-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8ea2b-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ea2b-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8ea2b-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ea2b-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8ea2b-136">Schema Name</span></span>  <br/> |<span data-ttu-id="8ea2b-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8ea2b-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8ea2b-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8ea2b-138">Validation File</span></span>  <br/> |<span data-ttu-id="8ea2b-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8ea2b-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ea2b-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8ea2b-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ea2b-141">False</span><span class="sxs-lookup"><span data-stu-id="8ea2b-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ea2b-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8ea2b-142">See also</span></span>



[<span data-ttu-id="8ea2b-143">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8ea2b-143">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="8ea2b-144">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8ea2b-144">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

