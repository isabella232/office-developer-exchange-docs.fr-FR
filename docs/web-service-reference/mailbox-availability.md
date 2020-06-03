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
description: L’élément Mailbox représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.
ms.openlocfilehash: 1bda6e8b90551b86b4e1c2711ac25693a65e5410
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458074"
---
# <a name="mailbox-availability"></a><span data-ttu-id="e9dbc-103">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="e9dbc-103">Mailbox (Availability)</span></span>

<span data-ttu-id="e9dbc-104">L’élément **Mailbox** représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-104">The **Mailbox** element represents the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span> 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

<span data-ttu-id="e9dbc-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e9dbc-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e9dbc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e9dbc-106">Attributes and elements</span></span>

<span data-ttu-id="e9dbc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9dbc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e9dbc-108">Attributes</span></span>

<span data-ttu-id="e9dbc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9dbc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e9dbc-110">Child elements</span></span>

|<span data-ttu-id="e9dbc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9dbc-111">**Element**</span></span>|<span data-ttu-id="e9dbc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9dbc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9dbc-113">Nom (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e9dbc-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="e9dbc-114">Représente le nom complet de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-114">Represents the display name of the mailbox user.</span></span> <span data-ttu-id="e9dbc-115">Cet élément est facultatif dans le SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-115">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="e9dbc-116">L’GetUserOofSettingsRequest renverra cet élément.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-116">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
|[<span data-ttu-id="e9dbc-117">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="e9dbc-117">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="e9dbc-118">Représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-118">Represents the e-mail address of the mailbox user.</span></span> <span data-ttu-id="e9dbc-119">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="e9dbc-120">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e9dbc-120">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e9dbc-121">Représente le protocole de routage du message.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-121">Represents the routing protocol for the message.</span></span> <span data-ttu-id="e9dbc-122">Cet élément est facultatif dans le SetUserOofSettingsRequest.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-122">This element is optional in the SetUserOofSettingsRequest.</span></span> <span data-ttu-id="e9dbc-123">L’GetUserOofSettingsRequest renverra cet élément.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-123">The GetUserOofSettingsRequest will return this element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9dbc-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e9dbc-124">Parent elements</span></span>

|<span data-ttu-id="e9dbc-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9dbc-125">**Element**</span></span>|<span data-ttu-id="e9dbc-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9dbc-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9dbc-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="e9dbc-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md) <br/> |<span data-ttu-id="e9dbc-128">Utilisé pour obtenir les paramètres et les messages d’absence du Bureau d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-128">Used to get a mailbox user's Out of Office (OOF) settings and messages.</span></span>  <br/> <span data-ttu-id="e9dbc-129">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="e9dbc-129">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[<span data-ttu-id="e9dbc-130">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="e9dbc-130">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="e9dbc-131">Permet de définir les paramètres et les messages OOF d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-131">Used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="e9dbc-132">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="e9dbc-132">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9dbc-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="e9dbc-133">Remarks</span></span>

<span data-ttu-id="e9dbc-134">L’adresse de messagerie est utilisée pour identifier le dossier de calendrier qui contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-134">The e-mail address is used to identify the calendar folder that contains the OOF settings.</span></span> 
  
<span data-ttu-id="e9dbc-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e9dbc-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9dbc-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e9dbc-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9dbc-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e9dbc-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9dbc-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e9dbc-138">Schema Name</span></span>  <br/> |<span data-ttu-id="e9dbc-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e9dbc-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9dbc-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e9dbc-140">Validation File</span></span>  <br/> |<span data-ttu-id="e9dbc-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9dbc-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9dbc-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e9dbc-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9dbc-143">False</span><span class="sxs-lookup"><span data-stu-id="e9dbc-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9dbc-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e9dbc-144">See also</span></span>

- [<span data-ttu-id="e9dbc-145">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e9dbc-145">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="e9dbc-146">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e9dbc-146">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

