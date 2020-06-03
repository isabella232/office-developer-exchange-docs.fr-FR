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
description: L’élément ExternalAudience définit ou contient une valeur qui détermine à qui les messages externes d’absence du Bureau (OOF) sont envoyés.
ms.openlocfilehash: b3fcebd9042b07bb9a8294196799ef2a13d78bdd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530599"
---
# <a name="externalaudience"></a><span data-ttu-id="91b27-103">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="91b27-103">ExternalAudience</span></span>

<span data-ttu-id="91b27-104">L’élément **ExternalAudience** définit ou contient une valeur qui détermine à qui les messages externes d’absence du Bureau (OOF) sont envoyés.</span><span class="sxs-lookup"><span data-stu-id="91b27-104">The **ExternalAudience** element sets or contains a value that determines to whom external Out of Office (OOF) messages are sent.</span></span> 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 <span data-ttu-id="91b27-105">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="91b27-105">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91b27-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="91b27-106">Attributes and elements</span></span>

<span data-ttu-id="91b27-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="91b27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91b27-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="91b27-108">Attributes</span></span>

<span data-ttu-id="91b27-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="91b27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91b27-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="91b27-110">Child elements</span></span>

<span data-ttu-id="91b27-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91b27-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91b27-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="91b27-112">Parent elements</span></span>

|<span data-ttu-id="91b27-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91b27-113">**Element**</span></span>|<span data-ttu-id="91b27-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="91b27-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91b27-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="91b27-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="91b27-116">Spécifie les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="91b27-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="91b27-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="91b27-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="91b27-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="91b27-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="91b27-119">Contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="91b27-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="91b27-120">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="91b27-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91b27-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="91b27-121">Text value</span></span>

<span data-ttu-id="91b27-122">Une valeur de texte est requise pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="91b27-122">A text value is required for this element.</span></span> <span data-ttu-id="91b27-123">Le tableau suivant répertorie les valeurs possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="91b27-123">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="91b27-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="91b27-124">**Value**</span></span>|<span data-ttu-id="91b27-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="91b27-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91b27-126">**Aucun**</span><span class="sxs-lookup"><span data-stu-id="91b27-126">**None**</span></span> <br/> |<span data-ttu-id="91b27-127">Les expéditeurs de messages électroniques situés en dehors de l’organisation de l’utilisateur de la boîte aux lettres qui envoient des messages à l’utilisateur ne reçoivent pas de réponse externe aux messages OOF.</span><span class="sxs-lookup"><span data-stu-id="91b27-127">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="91b27-128">**Connus**</span><span class="sxs-lookup"><span data-stu-id="91b27-128">**Known**</span></span> <br/> |<span data-ttu-id="91b27-129">Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront uniquement une réponse externe aux messages OOF si l’expéditeur se trouve dans la liste des contacts de la banque Exchange de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="91b27-129">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="91b27-130">**All**</span><span class="sxs-lookup"><span data-stu-id="91b27-130">**All**</span></span> <br/> |<span data-ttu-id="91b27-131">Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront une réponse externe aux messages OOF.</span><span class="sxs-lookup"><span data-stu-id="91b27-131">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="91b27-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="91b27-132">Remarks</span></span>

<span data-ttu-id="91b27-133">Cet élément partage le même type que l’élément [AllowExternalOof](allowexternaloof.md) .</span><span class="sxs-lookup"><span data-stu-id="91b27-133">This element shares the same type as the [AllowExternalOof](allowexternaloof.md) element.</span></span> 
  
<span data-ttu-id="91b27-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="91b27-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="91b27-135">Exemple</span><span class="sxs-lookup"><span data-stu-id="91b27-135">Example</span></span>

<span data-ttu-id="91b27-136">L’exemple de requête SetUserOofSettings suivant définit le OoFState sur **activé**, définit l’audience externe sur **tous**, définit la durée du OOF sur 10 jours et définit les messages OOF internes et externes.</span><span class="sxs-lookup"><span data-stu-id="91b27-136">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the external audience to **All**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="91b27-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="91b27-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91b27-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="91b27-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91b27-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="91b27-139">Schema Name</span></span>  <br/> |<span data-ttu-id="91b27-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="91b27-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="91b27-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="91b27-141">Validation File</span></span>  <br/> |<span data-ttu-id="91b27-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91b27-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91b27-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="91b27-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="91b27-144">False</span><span class="sxs-lookup"><span data-stu-id="91b27-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91b27-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="91b27-145">See also</span></span>



[<span data-ttu-id="91b27-146">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="91b27-146">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="91b27-147">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="91b27-147">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

