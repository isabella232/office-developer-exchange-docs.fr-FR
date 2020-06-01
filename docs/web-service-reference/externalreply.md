---
title: ExternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalReply
api_type:
- schema
ms.assetid: cbcfa469-242c-4f98-8f4f-2c9bcbe69f5a
description: L’élément ExternalReply contient la réponse d’absence du bureau qui est envoyée aux adresses en dehors du domaine du destinataire ou des domaines approuvés.
ms.openlocfilehash: c3381979e5e6aad51f9ae2bb3e661003ef793be6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458760"
---
# <a name="externalreply"></a><span data-ttu-id="980c8-103">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="980c8-103">ExternalReply</span></span>

<span data-ttu-id="980c8-104">L’élément **ExternalReply** contient la réponse d’absence du bureau qui est envoyée aux adresses en dehors du domaine du destinataire ou des domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="980c8-104">The **ExternalReply** element contains the out of office (OOF) response that is sent to addresses outside the recipient's domain or trusted domains.</span></span> 
  
```XML
<ExternalReply>
   <Message/>
</ExternalReply>
```

 <span data-ttu-id="980c8-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="980c8-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="980c8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="980c8-106">Attributes and elements</span></span>

<span data-ttu-id="980c8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="980c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="980c8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="980c8-108">Attributes</span></span>

|<span data-ttu-id="980c8-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="980c8-109">**Attribute**</span></span>|<span data-ttu-id="980c8-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="980c8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="980c8-111">XML : lang</span><span class="sxs-lookup"><span data-stu-id="980c8-111">xml:lang</span></span>  <br/> |<span data-ttu-id="980c8-112">Spécifie la langue utilisée dans le message **ExternalReply** .</span><span class="sxs-lookup"><span data-stu-id="980c8-112">Specifies the language used in the **ExternalReply** message.</span></span> <span data-ttu-id="980c8-113">Les valeurs possibles pour cet attribut sont définies par IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="980c8-113">The possible values for this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="980c8-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="980c8-114">Child elements</span></span>

|<span data-ttu-id="980c8-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="980c8-115">**Element**</span></span>|<span data-ttu-id="980c8-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="980c8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="980c8-117">Message (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="980c8-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="980c8-118">Contient la réponse OOF.</span><span class="sxs-lookup"><span data-stu-id="980c8-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="980c8-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="980c8-119">Parent elements</span></span>

|<span data-ttu-id="980c8-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="980c8-120">**Element**</span></span>|<span data-ttu-id="980c8-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="980c8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="980c8-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="980c8-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="980c8-123">Spécifie les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="980c8-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="980c8-124">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="980c8-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="980c8-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="980c8-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="980c8-126">Contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="980c8-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="980c8-127">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="980c8-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="980c8-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="980c8-128">Remarks</span></span>

<span data-ttu-id="980c8-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="980c8-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="980c8-130">Exemple</span><span class="sxs-lookup"><span data-stu-id="980c8-130">Example</span></span>

<span data-ttu-id="980c8-131">L’exemple de requête SetUserOofSettings suivant définit le [OofState](oofstate.md) sur **activé**, définit la durée du OOF sur 10 jours et définit les messages OOF internes et externes.</span><span class="sxs-lookup"><span data-stu-id="980c8-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="980c8-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="980c8-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="980c8-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="980c8-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="980c8-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="980c8-134">Schema Name</span></span>  <br/> |<span data-ttu-id="980c8-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="980c8-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="980c8-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="980c8-136">Validation File</span></span>  <br/> |<span data-ttu-id="980c8-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="980c8-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="980c8-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="980c8-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="980c8-139">False</span><span class="sxs-lookup"><span data-stu-id="980c8-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="980c8-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="980c8-140">See also</span></span>



[<span data-ttu-id="980c8-141">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="980c8-141">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

