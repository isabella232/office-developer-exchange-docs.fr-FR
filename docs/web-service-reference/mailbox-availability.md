---
title: Boîte aux lettres (disponibilité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: L’élément de boîte aux lettres représente l’utilisateur de boîte aux lettres pour un SetUserOofSettings ou GetUserOofSettings demande.
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828254"
---
# <a name="mailbox-availability"></a><span data-ttu-id="cea02-103">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="cea02-103">Mailbox (Availability)</span></span>

<span data-ttu-id="cea02-104">L’élément de **boîte aux lettres** représente l’utilisateur de boîte aux lettres pour un SetUserOofSettings ou GetUserOofSettings demande.</span><span class="sxs-lookup"><span data-stu-id="cea02-104">The **Mailbox** element represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span> 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

<span data-ttu-id="cea02-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="cea02-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cea02-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cea02-106">Attributes and elements</span></span>

<span data-ttu-id="cea02-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cea02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cea02-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cea02-108">Attributes</span></span>

<span data-ttu-id="cea02-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cea02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cea02-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cea02-110">Child elements</span></span>

|<span data-ttu-id="cea02-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cea02-111">**Element**</span></span>|<span data-ttu-id="cea02-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cea02-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cea02-113">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="cea02-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="cea02-114">Représente le nom complet de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cea02-114">Represents the display name of the mailbox user.</span></span> <span data-ttu-id="cea02-115">Cet élément est facultatif dans le SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="cea02-115">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="cea02-116">Le GetUserOofSettingsRequest retournera cet élément.</span><span class="sxs-lookup"><span data-stu-id="cea02-116">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
|[<span data-ttu-id="cea02-117">Adresse (chaîne)</span><span class="sxs-lookup"><span data-stu-id="cea02-117">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="cea02-118">Représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cea02-118">Represents the e-mail address of the mailbox user.</span></span> <span data-ttu-id="cea02-119">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="cea02-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="cea02-120">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="cea02-120">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="cea02-121">Représente le protocole de routage pour le message.</span><span class="sxs-lookup"><span data-stu-id="cea02-121">Represents the routing protocol for the message.</span></span> <span data-ttu-id="cea02-122">Cet élément est facultatif dans le SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="cea02-122">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="cea02-123">Le GetUserOofSettingsRequest retournera cet élément.</span><span class="sxs-lookup"><span data-stu-id="cea02-123">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cea02-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cea02-124">Parent elements</span></span>

|<span data-ttu-id="cea02-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cea02-125">**Element**</span></span>|<span data-ttu-id="cea02-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="cea02-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cea02-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="cea02-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md) <br/> |<span data-ttu-id="cea02-128">Permet d’obtenir les paramètres d’absence du bureau (OOF) et les messages d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cea02-128">Used to get a mailbox user's Out of Office (OOF) settings and messages.</span></span>  <br/> <span data-ttu-id="cea02-129">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="cea02-129">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[<span data-ttu-id="cea02-130">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="cea02-130">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="cea02-131">Permet de définir les paramètres d’absence du bureau et des messages d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cea02-131">Used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="cea02-132">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="cea02-132">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cea02-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="cea02-133">Remarks</span></span>

<span data-ttu-id="cea02-134">L’adresse de messagerie est utilisée pour identifier le dossier calendrier qui contient les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="cea02-134">The e-mail address is used to identify the calendar folder that contains the OOF settings.</span></span> 
  
<span data-ttu-id="cea02-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cea02-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cea02-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cea02-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cea02-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cea02-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cea02-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cea02-138">Schema Name</span></span>  <br/> |<span data-ttu-id="cea02-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cea02-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="cea02-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cea02-140">Validation File</span></span>  <br/> |<span data-ttu-id="cea02-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cea02-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cea02-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cea02-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="cea02-143">False</span><span class="sxs-lookup"><span data-stu-id="cea02-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cea02-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cea02-144">See also</span></span>

- [<span data-ttu-id="cea02-145">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="cea02-145">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="cea02-146">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="cea02-146">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

