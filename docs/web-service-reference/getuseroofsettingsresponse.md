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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457815"
---
# <a name="getuseroofsettingsresponse"></a><span data-ttu-id="4b54b-103">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="4b54b-103">GetUserOofSettingsResponse</span></span>

<span data-ttu-id="4b54b-104">L’élément **GetUserOofSettingsResponse** contient le message de réponse et les paramètres d’absence du Bureau pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="4b54b-104">The **GetUserOofSettingsResponse** element contains the response message and the Out of Office (OOF) settings for a user.</span></span> 
  
```xml
<GetUserOofSettingsResponse>
   <ResponseMessage>...</ResponseMessage>
   <OofSettings>...</OofSettings>
   <AllowExternalOof>...</AllowExternalOof>
</GetUserOofSettingsResponse>
```

 <span data-ttu-id="4b54b-105">**GetUserOofSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="4b54b-105">**GetUserOofSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b54b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b54b-106">Attributes and elements</span></span>

<span data-ttu-id="4b54b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b54b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b54b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b54b-108">Attributes</span></span>

<span data-ttu-id="4b54b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4b54b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b54b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b54b-110">Child elements</span></span>

|<span data-ttu-id="4b54b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b54b-111">**Element**</span></span>|<span data-ttu-id="4b54b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b54b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b54b-113">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4b54b-113">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="4b54b-114">Fournit des informations descriptives sur l’état de la réponse.</span><span class="sxs-lookup"><span data-stu-id="4b54b-114">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="4b54b-115">OofSettings</span><span class="sxs-lookup"><span data-stu-id="4b54b-115">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="4b54b-116">Contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="4b54b-116">Contains the OOF settings.</span></span>  <br/> |
|[<span data-ttu-id="4b54b-117">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="4b54b-117">AllowExternalOof</span></span>](allowexternaloof.md) <br/> |<span data-ttu-id="4b54b-118">Contient une valeur qui identifie l’expéditeur des messages OOF externes.</span><span class="sxs-lookup"><span data-stu-id="4b54b-118">Contains a value that identifies to whom external OOF messages are sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b54b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b54b-119">Parent elements</span></span>

<span data-ttu-id="4b54b-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b54b-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4b54b-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b54b-121">Remarks</span></span>

<span data-ttu-id="4b54b-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4b54b-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b54b-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b54b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b54b-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b54b-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b54b-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b54b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4b54b-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4b54b-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4b54b-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b54b-127">Validation File</span></span>  <br/> |<span data-ttu-id="4b54b-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4b54b-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b54b-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b54b-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b54b-130">False</span><span class="sxs-lookup"><span data-stu-id="4b54b-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b54b-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b54b-131">See also</span></span>



[<span data-ttu-id="4b54b-132">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4b54b-132">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="4b54b-133">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4b54b-133">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

