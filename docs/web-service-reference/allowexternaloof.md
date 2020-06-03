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
description: L’élément AllowExternalOof contient une valeur qui identifie l’expéditeur des messages d’absence du Bureau externes.
ms.openlocfilehash: e4934bc4bc86e1f9f764279a13ecaeca073d9e5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464811"
---
# <a name="allowexternaloof"></a><span data-ttu-id="a267b-103">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="a267b-103">AllowExternalOof</span></span>

<span data-ttu-id="a267b-104">L’élément **AllowExternalOof** contient une valeur qui identifie l’expéditeur des messages d’absence du Bureau externes.</span><span class="sxs-lookup"><span data-stu-id="a267b-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="a267b-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="a267b-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="a267b-106">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="a267b-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="a267b-107">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="a267b-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a267b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a267b-108">Attributes and elements</span></span>

<span data-ttu-id="a267b-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a267b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a267b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a267b-110">Attributes</span></span>

<span data-ttu-id="a267b-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a267b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a267b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a267b-112">Child elements</span></span>

<span data-ttu-id="a267b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a267b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a267b-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a267b-114">Parent elements</span></span>

|<span data-ttu-id="a267b-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a267b-115">**Element**</span></span>|<span data-ttu-id="a267b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="a267b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a267b-117">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="a267b-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="a267b-118">Contient les résultats de la réponse et les paramètres OOF d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a267b-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a267b-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a267b-119">Text value</span></span>

<span data-ttu-id="a267b-120">Une valeur de texte est requise pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="a267b-120">A text value is required for this element.</span></span> <span data-ttu-id="a267b-121">Le tableau suivant répertorie les valeurs possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="a267b-121">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="a267b-122">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="a267b-122">**Value**</span></span>|<span data-ttu-id="a267b-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="a267b-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a267b-124">**Aucun**</span><span class="sxs-lookup"><span data-stu-id="a267b-124">**None**</span></span> <br/> |<span data-ttu-id="a267b-125">Les expéditeurs de messages électroniques situés en dehors de l’organisation de l’utilisateur de la boîte aux lettres qui envoient des messages à l’utilisateur ne reçoivent pas de réponse externe aux messages OOF.</span><span class="sxs-lookup"><span data-stu-id="a267b-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="a267b-126">**Connus**</span><span class="sxs-lookup"><span data-stu-id="a267b-126">**Known**</span></span> <br/> |<span data-ttu-id="a267b-127">Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront uniquement une réponse externe aux messages OOF si l’expéditeur se trouve dans la liste des contacts de la banque Exchange de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a267b-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="a267b-128">**All**</span><span class="sxs-lookup"><span data-stu-id="a267b-128">**All**</span></span> <br/> |<span data-ttu-id="a267b-129">Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront une réponse externe aux messages OOF.</span><span class="sxs-lookup"><span data-stu-id="a267b-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a267b-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="a267b-130">Remarks</span></span>

<span data-ttu-id="a267b-131">Cet élément partage le même type que l’élément [ExternalAudience](externalaudience.md) .</span><span class="sxs-lookup"><span data-stu-id="a267b-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="a267b-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a267b-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a267b-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a267b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a267b-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a267b-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a267b-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a267b-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a267b-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a267b-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a267b-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a267b-137">Validation File</span></span>  <br/> |<span data-ttu-id="a267b-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a267b-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a267b-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a267b-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a267b-140">False</span><span class="sxs-lookup"><span data-stu-id="a267b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a267b-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a267b-141">See also</span></span>

- [<span data-ttu-id="a267b-142">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="a267b-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="a267b-143">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="a267b-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

