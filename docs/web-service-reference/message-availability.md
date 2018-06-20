---
title: Message (disponibilité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 1eec24dd-c981-41f4-a2f0-c51d43f1d7c0
description: Le Message contient l’extérieur de la réponse du bureau (OOF).
ms.openlocfilehash: 9facd04767fdcc0fd9dfd84fc6badb1a7633d2b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828452"
---
# <a name="message-availability"></a><span data-ttu-id="fb7d8-103">Message (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="fb7d8-103">Message (Availability)</span></span>

<span data-ttu-id="fb7d8-104">Le **Message** contient l’extérieur de la réponse du bureau (OOF).</span><span class="sxs-lookup"><span data-stu-id="fb7d8-104">The **Message** element contains the out of Office (OOF) response.</span></span> 
  
```xml
<Message/> 
```

 <span data-ttu-id="fb7d8-105">**string**</span><span class="sxs-lookup"><span data-stu-id="fb7d8-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb7d8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fb7d8-106">Attributes and elements</span></span>

<span data-ttu-id="fb7d8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb7d8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fb7d8-108">Attributes</span></span>

<span data-ttu-id="fb7d8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb7d8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fb7d8-110">Child elements</span></span>

<span data-ttu-id="fb7d8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb7d8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fb7d8-112">Parent elements</span></span>

|<span data-ttu-id="fb7d8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb7d8-113">**Element**</span></span>|<span data-ttu-id="fb7d8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb7d8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb7d8-115">InternalReply</span><span class="sxs-lookup"><span data-stu-id="fb7d8-115">InternalReply</span></span>](internalreply.md) <br/> | <span data-ttu-id="fb7d8-116">Contient le message d’absence du bureau envoyé à d’autres utilisateurs dans le domaine de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-116">Contains the OOF message sent to other users in the sender's domain.</span></span> <br/> <br/>  <span data-ttu-id="fb7d8-117">Les expressions XPath possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="fb7d8-117">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/InternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/InternalReply` <br/> |
|[<span data-ttu-id="fb7d8-118">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="fb7d8-118">ExternalReply</span></span>](externalreply.md) <br/> | <span data-ttu-id="fb7d8-119">Contient le message d’absence du bureau qui est envoyé aux adresses à l’extérieur du domaine de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-119">Contains the OOF message that is sent to addresses outside the sender's domain.</span></span>  <br/> <br/> <span data-ttu-id="fb7d8-120">Les expressions XPath possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="fb7d8-120">The following are the possible XPath expressions to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/ExternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/ExternalReply` <br/> |
|[<span data-ttu-id="fb7d8-121">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="fb7d8-121">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="fb7d8-122">Contient un message d’absence du bureau et de la langue utilisée pour le message.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-122">Contains an OOF message and the language used for the message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb7d8-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fb7d8-123">Text value</span></span>

<span data-ttu-id="fb7d8-124">Une valeur de texte est nécessaire pour définir le message d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-124">A text value is required to set the OOF message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb7d8-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="fb7d8-125">Remarks</span></span>

<span data-ttu-id="fb7d8-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="fb7d8-127">Exemple</span><span class="sxs-lookup"><span data-stu-id="fb7d8-127">Example</span></span>

<span data-ttu-id="fb7d8-128">L’exemple suivant d’une demande [d’opération SetUserOofSettings](setuseroofsettings-operation.md) définit [OofState](oofstate.md) sur **activé**, définit la durée d’absence du Bureau à 10 jours et définit les messages d’absence du bureau internes et externes.</span><span class="sxs-lookup"><span data-stu-id="fb7d8-128">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="fb7d8-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fb7d8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb7d8-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fb7d8-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb7d8-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fb7d8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="fb7d8-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fb7d8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb7d8-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fb7d8-133">Validation File</span></span>  <br/> |<span data-ttu-id="fb7d8-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb7d8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb7d8-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fb7d8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb7d8-136">False</span><span class="sxs-lookup"><span data-stu-id="fb7d8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb7d8-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fb7d8-137">See also</span></span>

- [<span data-ttu-id="fb7d8-138">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="fb7d8-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="fb7d8-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fb7d8-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
