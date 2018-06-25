---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: L’élément ExternalAudience définit ou contient une valeur qui détermine auquel sont envoyés les messages d’absence du bureau (OOF) externes.
ms.openlocfilehash: 836b0f6a5140a37e1584f571cb8e26534fe7a25f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756310"
---
# <a name="externalaudience"></a><span data-ttu-id="e1246-103">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="e1246-103">ExternalAudience</span></span>

<span data-ttu-id="e1246-104">L’élément **ExternalAudience** définit ou contient une valeur qui détermine auquel sont envoyés les messages d’absence du bureau (OOF) externes.</span><span class="sxs-lookup"><span data-stu-id="e1246-104">The **ExternalAudience** element sets or contains a value that determines to whom external Out of Office (OOF) messages are sent.</span></span> 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 <span data-ttu-id="e1246-105">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="e1246-105">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1246-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e1246-106">Attributes and elements</span></span>

<span data-ttu-id="e1246-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e1246-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1246-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e1246-108">Attributes</span></span>

<span data-ttu-id="e1246-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e1246-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1246-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e1246-110">Child elements</span></span>

<span data-ttu-id="e1246-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e1246-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1246-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e1246-112">Parent elements</span></span>

|<span data-ttu-id="e1246-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1246-113">**Element**</span></span>|<span data-ttu-id="e1246-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1246-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1246-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e1246-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="e1246-116">Spécifie les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="e1246-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="e1246-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="e1246-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="e1246-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="e1246-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="e1246-119">Contient les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="e1246-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="e1246-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="e1246-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1246-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e1246-121">Text value</span></span>

<span data-ttu-id="e1246-122">Une valeur de texte est nécessaire pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="e1246-122">A text value is required for this element.</span></span> <span data-ttu-id="e1246-123">Le tableau suivant répertorie les valeurs possibles de cet élément.</span><span class="sxs-lookup"><span data-stu-id="e1246-123">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="e1246-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e1246-124">**Value**</span></span>|<span data-ttu-id="e1246-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1246-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1246-126">**None**</span><span class="sxs-lookup"><span data-stu-id="e1246-126">**None**</span></span> <br/> |<span data-ttu-id="e1246-127">Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur ne recevra pas une réponse de message d’absence du bureau externe.</span><span class="sxs-lookup"><span data-stu-id="e1246-127">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="e1246-128">**Connus**</span><span class="sxs-lookup"><span data-stu-id="e1246-128">**Known**</span></span> <br/> |<span data-ttu-id="e1246-129">Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur seulement reçoit une réponse de message d’absence du bureau externe si l’expéditeur se trouve dans Exchange l’utilisateur stockent la liste des contacts.</span><span class="sxs-lookup"><span data-stu-id="e1246-129">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="e1246-130">**All**</span><span class="sxs-lookup"><span data-stu-id="e1246-130">**All**</span></span> <br/> |<span data-ttu-id="e1246-131">Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur reçoit une réponse de message d’absence du bureau externe.</span><span class="sxs-lookup"><span data-stu-id="e1246-131">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1246-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="e1246-132">Remarks</span></span>

<span data-ttu-id="e1246-133">Cet élément partageant le même type que l’élément [AllowExternalOof](allowexternaloof.md) .</span><span class="sxs-lookup"><span data-stu-id="e1246-133">This element shares the same type as the [AllowExternalOof](allowexternaloof.md) element.</span></span> 
  
<span data-ttu-id="e1246-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e1246-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="e1246-135">Exemple</span><span class="sxs-lookup"><span data-stu-id="e1246-135">Example</span></span>

<span data-ttu-id="e1246-136">L’exemple suivant d’une demande SetUserOofSettings définit le OoFState sur **activé**, définit l’audience externe pour **tous les**, définit la durée d’absence du Bureau à 10 jours et définit les messages d’absence du bureau internes et externes.</span><span class="sxs-lookup"><span data-stu-id="e1246-136">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the external audience to **All**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="e1246-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e1246-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1246-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e1246-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1246-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e1246-139">Schema Name</span></span>  <br/> |<span data-ttu-id="e1246-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e1246-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1246-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e1246-141">Validation File</span></span>  <br/> |<span data-ttu-id="e1246-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1246-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1246-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e1246-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1246-144">False</span><span class="sxs-lookup"><span data-stu-id="e1246-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1246-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e1246-145">See also</span></span>



[<span data-ttu-id="e1246-146">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e1246-146">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="e1246-147">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e1246-147">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

