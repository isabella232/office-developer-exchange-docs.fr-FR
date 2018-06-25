---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: L’élément AllowExternalOof contient une valeur qui identifie auquel sont envoyés les messages d’absence du bureau (OOF) externes.
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755200"
---
# <a name="allowexternaloof"></a><span data-ttu-id="1b7cc-103">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="1b7cc-103">AllowExternalOof</span></span>

<span data-ttu-id="1b7cc-104">L’élément **AllowExternalOof** contient une valeur qui identifie auquel sont envoyés les messages d’absence du bureau (OOF) externes.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="1b7cc-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="1b7cc-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="1b7cc-106">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="1b7cc-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="1b7cc-107">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b7cc-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1b7cc-108">Attributes and elements</span></span>

<span data-ttu-id="1b7cc-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b7cc-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="1b7cc-110">Attributes</span></span>

<span data-ttu-id="1b7cc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b7cc-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1b7cc-112">Child elements</span></span>

<span data-ttu-id="1b7cc-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b7cc-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1b7cc-114">Parent elements</span></span>

|<span data-ttu-id="1b7cc-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-115">**Element**</span></span>|<span data-ttu-id="1b7cc-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b7cc-117">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="1b7cc-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="1b7cc-118">Contient les résultats de la réponse et les paramètres d’absence du bureau pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b7cc-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1b7cc-119">Text value</span></span>

<span data-ttu-id="1b7cc-120">Une valeur de texte est nécessaire pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-120">A text value is required for this element.</span></span> <span data-ttu-id="1b7cc-121">Le tableau suivant répertorie les valeurs possibles de cet élément.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-121">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="1b7cc-122">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-122">**Value**</span></span>|<span data-ttu-id="1b7cc-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b7cc-124">**None**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-124">**None**</span></span> <br/> |<span data-ttu-id="1b7cc-125">Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur ne recevra pas une réponse de message d’absence du bureau externe.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="1b7cc-126">**Connus**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-126">**Known**</span></span> <br/> |<span data-ttu-id="1b7cc-127">Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur seulement reçoit une réponse de message d’absence du bureau externe si l’expéditeur se trouve dans Exchange l’utilisateur stockent la liste des contacts.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="1b7cc-128">**All**</span><span class="sxs-lookup"><span data-stu-id="1b7cc-128">**All**</span></span> <br/> |<span data-ttu-id="1b7cc-129">Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur reçoit une réponse de message d’absence du bureau externe.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b7cc-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="1b7cc-130">Remarks</span></span>

<span data-ttu-id="1b7cc-131">Cet élément partageant le même type que l’élément [ExternalAudience](externalaudience.md) .</span><span class="sxs-lookup"><span data-stu-id="1b7cc-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="1b7cc-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1b7cc-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b7cc-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1b7cc-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b7cc-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1b7cc-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b7cc-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1b7cc-135">Schema Name</span></span>  <br/> |<span data-ttu-id="1b7cc-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1b7cc-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b7cc-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1b7cc-137">Validation File</span></span>  <br/> |<span data-ttu-id="1b7cc-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b7cc-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b7cc-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1b7cc-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b7cc-140">False</span><span class="sxs-lookup"><span data-stu-id="1b7cc-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b7cc-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1b7cc-141">See also</span></span>

- [<span data-ttu-id="1b7cc-142">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="1b7cc-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="1b7cc-143">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="1b7cc-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

