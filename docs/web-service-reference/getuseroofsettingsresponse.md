---
title: GetUserOofSettingsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsResponse
api_type:
- schema
ms.assetid: 011cb38b-da3c-4b1b-8836-a6b212b511f6
description: L’élément GetUserOofSettingsResponse contient le message de réponse et les paramètres d’absence du Bureau pour un utilisateur.
ms.openlocfilehash: f7f28c67fd36630ffb5294ab35c0fef2f467ba22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457815"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="40a77-103">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="40a77-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="40a77-104">L’élément **GetUserOofSettingsResponse** contient le message de réponse et les paramètres d’absence du Bureau pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="40a77-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="40a77-105">**GetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="40a77-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40a77-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="40a77-106">Attributes and elements</span></span>

<span data-ttu-id="40a77-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="40a77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40a77-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="40a77-108">Attributes</span></span>

<span data-ttu-id="40a77-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="40a77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40a77-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="40a77-110">Child elements</span></span>

|<span data-ttu-id="40a77-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="40a77-111">**Element**</span></span>|<span data-ttu-id="40a77-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="40a77-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40a77-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="40a77-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="40a77-114">Fournit des informations descriptives sur l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="40a77-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="40a77-115">OofSettings</span><span class="sxs-lookup"><span data-stu-id="40a77-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="40a77-116">Contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="40a77-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="40a77-117">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="40a77-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="40a77-118">Contient une valeur qui identifie l’expéditeur des messages OOF externes.</span><span class="sxs-lookup"><span data-stu-id="40a77-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40a77-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="40a77-119">Parent elements</span></span>

<span data-ttu-id="40a77-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="40a77-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="40a77-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="40a77-121">Remarks</span></span>

<span data-ttu-id="40a77-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="40a77-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40a77-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="40a77-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40a77-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="40a77-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="40a77-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="40a77-125">Schema Name</span></span>  <br/> |<span data-ttu-id="40a77-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="40a77-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="40a77-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="40a77-127">Validation File</span></span>  <br/> |<span data-ttu-id="40a77-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="40a77-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="40a77-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="40a77-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="40a77-130">False</span><span class="sxs-lookup"><span data-stu-id="40a77-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40a77-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40a77-131">See also</span></span>



[<span data-ttu-id="40a77-132">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="40a77-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="40a77-133">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="40a77-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

