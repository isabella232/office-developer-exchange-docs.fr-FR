---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: L’élément UserOofSettings spécifie les paramètres d’absence du bureau.
ms.openlocfilehash: 417c3d5061a6229d41eb57f72e89f03213acf460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461904"
---
# <a name="useroofsettings"></a><span data-ttu-id="38aba-103">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="38aba-103">UserOofSettings</span></span>

<span data-ttu-id="38aba-104">L’élément **UserOofSettings** spécifie les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="38aba-104">The **UserOofSettings** element specifies the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="38aba-105">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="38aba-105">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
  
[<span data-ttu-id="38aba-106">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="38aba-106">UserOofSettings</span></span>](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 <span data-ttu-id="38aba-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="38aba-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38aba-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="38aba-108">Attributes and elements</span></span>

<span data-ttu-id="38aba-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="38aba-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38aba-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="38aba-110">Attributes</span></span>

<span data-ttu-id="38aba-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="38aba-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38aba-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="38aba-112">Child elements</span></span>

|<span data-ttu-id="38aba-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38aba-113">**Element**</span></span>|<span data-ttu-id="38aba-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="38aba-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38aba-115">OofState</span><span class="sxs-lookup"><span data-stu-id="38aba-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="38aba-116">Définit l’état d’absence du Bureau de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="38aba-116">Sets the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="38aba-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="38aba-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="38aba-118">Définit ou contient une valeur qui détermine à qui les messages externes OOF sont envoyés.</span><span class="sxs-lookup"><span data-stu-id="38aba-118">Sets or contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="38aba-119">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="38aba-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="38aba-120">Spécifie la durée pendant laquelle le statut OOF est activé si l’élément [OofState](oofstate.md) est défini sur **Planifié**.</span><span class="sxs-lookup"><span data-stu-id="38aba-120">Specifies the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="38aba-121">Si l’élément [OofState](oofstate.md) est défini sur **Enabled** ou **Disabled**, la valeur de cet élément est ignorée.</span><span class="sxs-lookup"><span data-stu-id="38aba-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="38aba-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="38aba-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="38aba-123">Contient la réponse OOF envoyée aux autres utilisateurs dans le domaine de l’utilisateur ou les domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="38aba-123">Contains the OOF response sent to other users in the user's domain or trusted domains.</span></span>  <br/> |
|[<span data-ttu-id="38aba-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="38aba-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="38aba-125">Contient la réponse OOF envoyée aux adresses en dehors du domaine du destinataire ou des domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="38aba-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38aba-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="38aba-126">Parent elements</span></span>

|<span data-ttu-id="38aba-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38aba-127">**Element**</span></span>|<span data-ttu-id="38aba-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="38aba-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38aba-129">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="38aba-129">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="38aba-130">Contient les arguments utilisés pour définir les paramètres et les messages OOF d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38aba-130">Contains the arguments used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="38aba-131">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="38aba-131">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38aba-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="38aba-132">Remarks</span></span>

<span data-ttu-id="38aba-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="38aba-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="38aba-134">Exemple</span><span class="sxs-lookup"><span data-stu-id="38aba-134">Example</span></span>

<span data-ttu-id="38aba-135">L’exemple de requête SetUserOofSettings suivant définit le OoFState sur **activé**, définit la durée de l’absence du Bureau pour 10 jours et définit les messages OOF internes et externes.</span><span class="sxs-lookup"><span data-stu-id="38aba-135">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="38aba-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="38aba-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38aba-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="38aba-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38aba-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="38aba-138">Schema Name</span></span>  <br/> |<span data-ttu-id="38aba-139">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="38aba-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="38aba-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="38aba-140">Validation File</span></span>  <br/> |<span data-ttu-id="38aba-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="38aba-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38aba-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="38aba-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="38aba-143">False</span><span class="sxs-lookup"><span data-stu-id="38aba-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38aba-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38aba-144">See also</span></span>

- [<span data-ttu-id="38aba-145">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="38aba-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

