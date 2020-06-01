---
title: Durée (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: L’élément Duration spécifie la durée pendant laquelle l’État absent (absent du bureau) est activé si l’élément OofState est défini sur planifié.
ms.openlocfilehash: 0ba0f1ea7498781c0cccb072c7ea0fa05414764c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457297"
---
# <a name="duration-useroofsettings"></a><span data-ttu-id="2bee3-103">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="2bee3-103">Duration (UserOofSettings)</span></span>

<span data-ttu-id="2bee3-104">L’élément **Duration** spécifie la durée pendant laquelle l’État absent (absent du bureau) est activé si l’élément [OofState](oofstate.md) est défini sur **planifié**.</span><span class="sxs-lookup"><span data-stu-id="2bee3-104">The **Duration** element specifies the duration that the out of office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 <span data-ttu-id="2bee3-105">**Duration**</span><span class="sxs-lookup"><span data-stu-id="2bee3-105">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bee3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2bee3-106">Attributes and elements</span></span>

<span data-ttu-id="2bee3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2bee3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bee3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2bee3-108">Attributes</span></span>

<span data-ttu-id="2bee3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2bee3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bee3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2bee3-110">Child elements</span></span>

|<span data-ttu-id="2bee3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2bee3-111">**Element**</span></span>|<span data-ttu-id="2bee3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2bee3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bee3-113">StartTime</span><span class="sxs-lookup"><span data-stu-id="2bee3-113">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="2bee3-114">Représente le début de l’intervalle de temps défini avec un statut OOF.</span><span class="sxs-lookup"><span data-stu-id="2bee3-114">Represents the start of the time span set with an OOF status.</span></span> <span data-ttu-id="2bee3-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="2bee3-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2bee3-116">EndTime</span><span class="sxs-lookup"><span data-stu-id="2bee3-116">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="2bee3-117">Représente la fin de l’intervalle de temps défini avec un statut OOF.</span><span class="sxs-lookup"><span data-stu-id="2bee3-117">Represents the end of the time span set with an OOF status.</span></span> <span data-ttu-id="2bee3-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="2bee3-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2bee3-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2bee3-119">Parent elements</span></span>

|<span data-ttu-id="2bee3-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2bee3-120">**Element**</span></span>|<span data-ttu-id="2bee3-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2bee3-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bee3-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="2bee3-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="2bee3-123">Spécifie les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="2bee3-123">Specifies the OOF settings.</span></span>  <br/><br/><span data-ttu-id="2bee3-124">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2bee3-124">The following is the XPath expression to this element:</span></span><br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="2bee3-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="2bee3-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="2bee3-126">Contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="2bee3-126">Contains the OOF settings.</span></span><br/><br/><span data-ttu-id="2bee3-127">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2bee3-127">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[<span data-ttu-id="2bee3-128">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="2bee3-128">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="2bee3-129">Définit le message de réponse d’absence du bureau et une durée d’envoi du message de réponse pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2bee3-129">Defines the Out of Office (OOF) response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2bee3-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="2bee3-130">Remarks</span></span>

<span data-ttu-id="2bee3-131">Le type de **durée** est également le type des éléments [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [TimeWindow](timewindow.md)et [OutOfOffice](outofoffice.md) .</span><span class="sxs-lookup"><span data-stu-id="2bee3-131">The **Duration** type is also the type for the [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [TimeWindow](timewindow.md), and [OutOfOffice](outofoffice.md) elements.</span></span> 
  
<span data-ttu-id="2bee3-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2bee3-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="2bee3-133">Exemple</span><span class="sxs-lookup"><span data-stu-id="2bee3-133">Example</span></span>

<span data-ttu-id="2bee3-134">L’exemple suivant de demande d' [opération SetUserOofSettings](setuseroofsettings-operation.md) définit le [OofState](oofstate.md) sur **Enabled**, les messages OOF internes et externes, et définit la durée du OOF pendant 10 jours.</span><span class="sxs-lookup"><span data-stu-id="2bee3-134">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, the internal and external OOF messages, and sets the duration of OOF for 10 days.</span></span>
  
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
        <SetByLegacyClient>false</SetByLegacyClient>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="2bee3-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2bee3-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bee3-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2bee3-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2bee3-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2bee3-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2bee3-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2bee3-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="2bee3-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2bee3-139">Validation File</span></span>  <br/> |<span data-ttu-id="2bee3-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2bee3-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2bee3-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2bee3-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bee3-142">False</span><span class="sxs-lookup"><span data-stu-id="2bee3-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bee3-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2bee3-143">See also</span></span>

- [<span data-ttu-id="2bee3-144">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="2bee3-144">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)  
- [<span data-ttu-id="2bee3-145">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="2bee3-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

