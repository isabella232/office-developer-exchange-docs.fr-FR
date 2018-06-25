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
description: L’élément UserOofSettings spécifie les paramètres d’absence du bureau (OOF).
ms.openlocfilehash: a035fd89387ece632d83f5f72a564e4896bc6753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838969"
---
# <a name="useroofsettings"></a><span data-ttu-id="7f2e2-103">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7f2e2-103">UserOofSettings</span></span>

<span data-ttu-id="7f2e2-104">L’élément **UserOofSettings** spécifie les paramètres d’absence du bureau (OOF).</span><span class="sxs-lookup"><span data-stu-id="7f2e2-104">The **UserOofSettings** element specifies the Out of Office (OOF) settings.</span></span> 
  
[<span data-ttu-id="7f2e2-105">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="7f2e2-105">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
  
[<span data-ttu-id="7f2e2-106">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7f2e2-106">UserOofSettings</span></span>](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 <span data-ttu-id="7f2e2-107">**UserOofSettings**</span><span class="sxs-lookup"><span data-stu-id="7f2e2-107">**UserOofSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f2e2-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7f2e2-108">Attributes and elements</span></span>

<span data-ttu-id="7f2e2-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f2e2-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7f2e2-110">Attributes</span></span>

<span data-ttu-id="7f2e2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f2e2-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7f2e2-112">Child elements</span></span>

|<span data-ttu-id="7f2e2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7f2e2-113">**Element**</span></span>|<span data-ttu-id="7f2e2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7f2e2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f2e2-115">OofState</span><span class="sxs-lookup"><span data-stu-id="7f2e2-115">OofState</span></span>](oofstate.md) <br/> |<span data-ttu-id="7f2e2-116">Définit l’état d’absence du bureau de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-116">Sets the user's OOF state.</span></span>  <br/> |
|[<span data-ttu-id="7f2e2-117">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="7f2e2-117">ExternalAudience</span></span>](externalaudience.md) <br/> |<span data-ttu-id="7f2e2-118">Définit ou contient une valeur qui détermine les messages d’absence du bureau externes qui sont envoyés.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-118">Sets or contains a value that determines to whom external OOF messages are sent.</span></span>  <br/> |
|[<span data-ttu-id="7f2e2-119">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="7f2e2-119">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="7f2e2-120">Spécifie la durée pour laquelle le statut d’absence du bureau est activé si l’élément [OofState](oofstate.md) est défini sur **planifiées**.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-120">Specifies the duration for which the OOF status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span> <span data-ttu-id="7f2e2-121">Si l’élément [OofState](oofstate.md) est défini sur **activé** ou **désactivé**, la valeur de cet élément est ignorée.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-121">If the [OofState](oofstate.md) element is set to **Enabled** or **Disabled**, the value of this element is ignored.</span></span>  <br/> |
|[<span data-ttu-id="7f2e2-122">InternalReply</span><span class="sxs-lookup"><span data-stu-id="7f2e2-122">InternalReply</span></span>](internalreply.md) <br/> |<span data-ttu-id="7f2e2-123">Contient la réponse d’absence du bureau envoyée à d’autres utilisateurs dans le domaine de l’utilisateur ou de domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-123">Contains the OOF response sent to other users in the user's domain or trusted domains.</span></span>  <br/> |
|[<span data-ttu-id="7f2e2-124">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="7f2e2-124">ExternalReply</span></span>](externalreply.md) <br/> |<span data-ttu-id="7f2e2-125">Contient la réponse d’absence du bureau envoyée aux adresses à l’extérieur du destinataire ou les domaines approuvés.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-125">Contains the OOF response sent to addresses outside the recipient's domain or trusted domains.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7f2e2-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7f2e2-126">Parent elements</span></span>

|<span data-ttu-id="7f2e2-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7f2e2-127">**Element**</span></span>|<span data-ttu-id="7f2e2-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="7f2e2-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f2e2-129">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="7f2e2-129">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md) <br/> |<span data-ttu-id="7f2e2-130">Contient les arguments permet de définir les paramètres d’absence du bureau et des messages d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-130">Contains the arguments used to set a mailbox user's OOF settings and messages.</span></span>  <br/> <span data-ttu-id="7f2e2-131">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="7f2e2-131">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7f2e2-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="7f2e2-132">Remarks</span></span>

<span data-ttu-id="7f2e2-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="7f2e2-134">Exemple</span><span class="sxs-lookup"><span data-stu-id="7f2e2-134">Example</span></span>

<span data-ttu-id="7f2e2-135">L’exemple suivant d’une demande SetUserOofSettings définit le OoFState sur **activé**, définit la durée d’absence du bureau pour 10 jours et définit les messages d’absence du bureau internes et externes.</span><span class="sxs-lookup"><span data-stu-id="7f2e2-135">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```xml
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

## <a name="element-information"></a><span data-ttu-id="7f2e2-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7f2e2-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f2e2-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7f2e2-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f2e2-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7f2e2-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7f2e2-139">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="7f2e2-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="7f2e2-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7f2e2-140">Validation File</span></span>  <br/> |<span data-ttu-id="7f2e2-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f2e2-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f2e2-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7f2e2-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f2e2-143">False</span><span class="sxs-lookup"><span data-stu-id="7f2e2-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f2e2-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7f2e2-144">See also</span></span>

- [<span data-ttu-id="7f2e2-145">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7f2e2-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

