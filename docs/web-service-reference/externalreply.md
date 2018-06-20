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
description: L’élément ExternalReply contient à l’extérieur de la réponse de bureau (OOF) qui est envoyé à une adresse hors du destinataire ou les domaines approuvés.
ms.openlocfilehash: f318b34c98dd42487b8ca3791ba915fb91d629a5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756339"
---
# <a name="externalreply"></a><span data-ttu-id="a0573-103">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="a0573-103">ExternalReply</span></span>

<span data-ttu-id="a0573-104">L’élément **ExternalReply** contient à l’extérieur de la réponse de bureau (OOF) qui est envoyé à une adresse hors du destinataire ou les domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="a0573-104">The **ExternalReply** element contains the out of office (OOF) response that is sent to addresses outside the recipient's domain or trusted domains.</span></span> 
  
```XML
<ExternalReply>
   <Message/>
</ExternalReply>
```

 <span data-ttu-id="a0573-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="a0573-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0573-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0573-106">Attributes and elements</span></span>

<span data-ttu-id="a0573-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0573-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0573-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0573-108">Attributes</span></span>

|<span data-ttu-id="a0573-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a0573-109">**Attribute**</span></span>|<span data-ttu-id="a0573-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0573-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0573-111">XML : lang</span><span class="sxs-lookup"><span data-stu-id="a0573-111">xml:lang</span></span>  <br/> |<span data-ttu-id="a0573-112">Spécifie la langue utilisée dans le message **ExternalReply** .</span><span class="sxs-lookup"><span data-stu-id="a0573-112">Specifies the language used in the **ExternalReply** message.</span></span> <span data-ttu-id="a0573-113">Les valeurs possibles de cet attribut sont définies par la norme IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="a0573-113">The possible values for this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a0573-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0573-114">Child elements</span></span>

|<span data-ttu-id="a0573-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0573-115">**Element**</span></span>|<span data-ttu-id="a0573-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0573-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0573-117">Message (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="a0573-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="a0573-118">Contient la réponse d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="a0573-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0573-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0573-119">Parent elements</span></span>

|<span data-ttu-id="a0573-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0573-120">**Element**</span></span>|<span data-ttu-id="a0573-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0573-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0573-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="a0573-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="a0573-123">Spécifie les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="a0573-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="a0573-124">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a0573-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="a0573-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="a0573-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="a0573-126">Contient les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="a0573-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="a0573-127">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a0573-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0573-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0573-128">Remarks</span></span>

<span data-ttu-id="a0573-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0573-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="a0573-130">Exemple</span><span class="sxs-lookup"><span data-stu-id="a0573-130">Example</span></span>

<span data-ttu-id="a0573-131">L’exemple suivant d’une demande SetUserOofSettings définit [OofState](oofstate.md) sur **activé**, définit la durée d’absence du Bureau à 10 jours et définit les messages d’absence du bureau internes et externes.</span><span class="sxs-lookup"><span data-stu-id="a0573-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="a0573-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0573-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0573-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0573-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0573-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0573-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a0573-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a0573-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0573-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0573-136">Validation File</span></span>  <br/> |<span data-ttu-id="a0573-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a0573-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0573-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0573-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0573-139">False</span><span class="sxs-lookup"><span data-stu-id="a0573-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0573-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0573-140">See also</span></span>



[<span data-ttu-id="a0573-141">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="a0573-141">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

