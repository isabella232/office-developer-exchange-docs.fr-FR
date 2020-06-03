---
title: OofState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofState
api_type:
- schema
ms.assetid: 3c486a38-06da-4382-ad20-664d067d76ac
description: L’élément OofState est utilisé pour obtenir ou définir l’État absent (e) du Bureau de l’utilisateur.
ms.openlocfilehash: 6aef7d989ee6978019a483f2673895e68a88a7c5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459734"
---
# <a name="oofstate"></a><span data-ttu-id="325c4-103">OofState</span><span class="sxs-lookup"><span data-stu-id="325c4-103">OofState</span></span>

<span data-ttu-id="325c4-104">L’élément **OofState** est utilisé pour obtenir ou définir l’État absent (e) du Bureau de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="325c4-104">The **OofState** element is used to get or set the user's Out of Office (OOF) state.</span></span> 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 <span data-ttu-id="325c4-105">**OofState**</span><span class="sxs-lookup"><span data-stu-id="325c4-105">**OofState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="325c4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="325c4-106">Attributes and elements</span></span>

<span data-ttu-id="325c4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="325c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="325c4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="325c4-108">Attributes</span></span>

<span data-ttu-id="325c4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="325c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="325c4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="325c4-110">Child elements</span></span>

<span data-ttu-id="325c4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="325c4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="325c4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="325c4-112">Parent elements</span></span>

|<span data-ttu-id="325c4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="325c4-113">**Element**</span></span>|<span data-ttu-id="325c4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="325c4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="325c4-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="325c4-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="325c4-116">Spécifie les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="325c4-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="325c4-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="325c4-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="325c4-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="325c4-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="325c4-119">Contient les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="325c4-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="325c4-120">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="325c4-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="325c4-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="325c4-121">Text value</span></span>

<span data-ttu-id="325c4-122">Une valeur de texte est requise pour l’élément **OofState** .</span><span class="sxs-lookup"><span data-stu-id="325c4-122">A text value is required for the **OofState** element.</span></span> <span data-ttu-id="325c4-123">La liste suivante contient les valeurs possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="325c4-123">The following list contains the possible values for this element:</span></span> 
  
- <span data-ttu-id="325c4-124">**Disabled**</span><span class="sxs-lookup"><span data-stu-id="325c4-124">**Disabled**</span></span>
    
- <span data-ttu-id="325c4-125">**Enabled**</span><span class="sxs-lookup"><span data-stu-id="325c4-125">**Enabled**</span></span>
    
- <span data-ttu-id="325c4-126">**Scheduled**</span><span class="sxs-lookup"><span data-stu-id="325c4-126">**Scheduled**</span></span>
    
<span data-ttu-id="325c4-127">Une valeur de **scheduled** indique que le statut OOF est défini sur **activé** pendant une période identifiée par l’élément [Duration (UserOofSettings)](duration-useroofsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="325c4-127">A value of **Scheduled** indicates that the OOF status is set to **Enabled** during a time period identified by the [Duration (UserOofSettings)](duration-useroofsettings.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="325c4-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="325c4-128">Remarks</span></span>

<span data-ttu-id="325c4-129">Cet élément est requis dans le message SetUsersOofSettingRequest et le message GetUserOofSettingResponse.</span><span class="sxs-lookup"><span data-stu-id="325c4-129">This element is required in both the SetUsersOofSettingRequest message and the GetUserOofSettingResponse message.</span></span>
  
<span data-ttu-id="325c4-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="325c4-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="325c4-131">Exemple</span><span class="sxs-lookup"><span data-stu-id="325c4-131">Example</span></span>

<span data-ttu-id="325c4-132">L’exemple de requête SetUserOofSettings suivant active l' **OofState**.</span><span class="sxs-lookup"><span data-stu-id="325c4-132">The following example of a SetUserOofSettings request enables the **OofState**.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="325c4-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="325c4-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="325c4-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="325c4-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="325c4-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="325c4-135">Schema Name</span></span>  <br/> |<span data-ttu-id="325c4-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="325c4-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="325c4-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="325c4-137">Validation File</span></span>  <br/> |<span data-ttu-id="325c4-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="325c4-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="325c4-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="325c4-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="325c4-140">False</span><span class="sxs-lookup"><span data-stu-id="325c4-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="325c4-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="325c4-141">See also</span></span>



[<span data-ttu-id="325c4-142">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="325c4-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="325c4-143">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="325c4-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

