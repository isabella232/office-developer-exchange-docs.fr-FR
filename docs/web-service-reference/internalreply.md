---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: L’élément InternalReply contient la réponse d’absence du Bureau envoyée aux autres utilisateurs dans le domaine ou les domaines approuvés de l’utilisateur.
ms.openlocfilehash: 24c278ebd3acf83e87fbf72650eb3d5d438d5c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465582"
---
# <a name="internalreply"></a><span data-ttu-id="daa57-103">InternalReply</span><span class="sxs-lookup"><span data-stu-id="daa57-103">InternalReply</span></span>

<span data-ttu-id="daa57-104">L’élément **InternalReply** contient la réponse d’absence du Bureau envoyée aux autres utilisateurs dans le domaine ou les domaines approuvés de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="daa57-104">The **InternalReply** element contains the out of office (OOF) response sent to other users in the user's domain or trusted domains.</span></span> 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 <span data-ttu-id="daa57-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="daa57-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="daa57-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="daa57-106">Attributes and elements</span></span>

<span data-ttu-id="daa57-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="daa57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="daa57-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="daa57-108">Attributes</span></span>

|<span data-ttu-id="daa57-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="daa57-109">**Attribute**</span></span>|<span data-ttu-id="daa57-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="daa57-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="daa57-111">XML : lang</span><span class="sxs-lookup"><span data-stu-id="daa57-111">xml:lang</span></span>  <br/> |<span data-ttu-id="daa57-112">Spécifie la langue utilisée dans le message **InternalReply** .</span><span class="sxs-lookup"><span data-stu-id="daa57-112">Specifies the language used in the **InternalReply** message.</span></span> <span data-ttu-id="daa57-113">Les valeurs possibles de cet attribut sont définies par IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="daa57-113">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="daa57-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="daa57-114">Child elements</span></span>

|<span data-ttu-id="daa57-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="daa57-115">**Element**</span></span>|<span data-ttu-id="daa57-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="daa57-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="daa57-117">Message (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="daa57-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="daa57-118">Contient la réponse OOF.</span><span class="sxs-lookup"><span data-stu-id="daa57-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="daa57-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="daa57-119">Parent elements</span></span>

|<span data-ttu-id="daa57-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="daa57-120">**Element**</span></span>|<span data-ttu-id="daa57-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="daa57-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="daa57-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="daa57-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="daa57-123">Spécifie les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="daa57-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="daa57-124">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="daa57-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="daa57-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="daa57-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="daa57-126">Contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="daa57-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="daa57-127">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="daa57-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="daa57-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="daa57-128">Remarks</span></span>

<span data-ttu-id="daa57-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="daa57-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="daa57-130">Exemple</span><span class="sxs-lookup"><span data-stu-id="daa57-130">Example</span></span>

<span data-ttu-id="daa57-131">L’exemple de requête SetUserOofSettings suivant définit le [OofState](oofstate.md) sur **activé**, définit la durée de l’absence du Bureau pour 10 jours et définit les messages OOF internes et externes.</span><span class="sxs-lookup"><span data-stu-id="daa57-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="daa57-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="daa57-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="daa57-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="daa57-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="daa57-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="daa57-134">Schema Name</span></span>  <br/> |<span data-ttu-id="daa57-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="daa57-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="daa57-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="daa57-136">Validation File</span></span>  <br/> |<span data-ttu-id="daa57-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="daa57-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="daa57-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="daa57-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="daa57-139">False</span><span class="sxs-lookup"><span data-stu-id="daa57-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="daa57-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="daa57-140">See also</span></span>



[<span data-ttu-id="daa57-141">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="daa57-141">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="daa57-142">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="daa57-142">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

