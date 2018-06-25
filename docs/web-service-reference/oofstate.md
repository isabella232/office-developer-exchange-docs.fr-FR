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
description: L’élément OofState est utilisé pour obtenir ou définir l’état d’absence du bureau (OOF) de l’utilisateur.
ms.openlocfilehash: f97c050aec102b384fa4d98e6dee43befd4dc9ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828651"
---
# <a name="oofstate"></a><span data-ttu-id="7f57a-103">OofState</span><span class="sxs-lookup"><span data-stu-id="7f57a-103">OofState</span></span>

<span data-ttu-id="7f57a-104">L’élément **OofState** est utilisé pour obtenir ou définir l’état d’absence du bureau (OOF) de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7f57a-104">The **OofState** element is used to get or set the user's Out of Office (OOF) state.</span></span> 
  
```xml
<OofState>Disabled or Enabled or Scheduled</OofState>
```

 <span data-ttu-id="7f57a-105">**OofState**</span><span class="sxs-lookup"><span data-stu-id="7f57a-105">**OofState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f57a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7f57a-106">Attributes and elements</span></span>

<span data-ttu-id="7f57a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7f57a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f57a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7f57a-108">Attributes</span></span>

<span data-ttu-id="7f57a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7f57a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f57a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7f57a-110">Child elements</span></span>

<span data-ttu-id="7f57a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7f57a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f57a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7f57a-112">Parent elements</span></span>

|<span data-ttu-id="7f57a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7f57a-113">**Element**</span></span>|<span data-ttu-id="7f57a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7f57a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f57a-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7f57a-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="7f57a-116">Spécifie les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="7f57a-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="7f57a-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="7f57a-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="7f57a-118">OofSettings</span><span class="sxs-lookup"><span data-stu-id="7f57a-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="7f57a-119">Contient les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="7f57a-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="7f57a-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="7f57a-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7f57a-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7f57a-121">Text value</span></span>

<span data-ttu-id="7f57a-122">Une valeur de texte est requise pour l’élément **OofState** .</span><span class="sxs-lookup"><span data-stu-id="7f57a-122">A text value is required for the **OofState** element.</span></span> <span data-ttu-id="7f57a-123">La liste suivante contient les valeurs possibles de cet élément :</span><span class="sxs-lookup"><span data-stu-id="7f57a-123">The following list contains the possible values for this element:</span></span> 
  
- <span data-ttu-id="7f57a-124">**Désactivé**</span><span class="sxs-lookup"><span data-stu-id="7f57a-124">**Disabled**</span></span>
    
- <span data-ttu-id="7f57a-125">**Enabled**</span><span class="sxs-lookup"><span data-stu-id="7f57a-125">**Enabled**</span></span>
    
- <span data-ttu-id="7f57a-126">**Planifiée**</span><span class="sxs-lookup"><span data-stu-id="7f57a-126">**Scheduled**</span></span>
    
<span data-ttu-id="7f57a-127">Une valeur **planifiée** indique que le statut d’absence du bureau est défini sur **activé** durant une période identifiée par l’élément [durée (UserOofSettings)](duration-useroofsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="7f57a-127">A value of **Scheduled** indicates that the OOF status is set to **Enabled** during a time period identified by the [Duration (UserOofSettings)](duration-useroofsettings.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7f57a-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="7f57a-128">Remarks</span></span>

<span data-ttu-id="7f57a-129">Cet élément est requis dans le message SetUsersOofSettingRequest et le message GetUserOofSettingResponse.</span><span class="sxs-lookup"><span data-stu-id="7f57a-129">This element is required in both the SetUsersOofSettingRequest message and the GetUserOofSettingResponse message.</span></span>
  
<span data-ttu-id="7f57a-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7f57a-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="7f57a-131">Exemple</span><span class="sxs-lookup"><span data-stu-id="7f57a-131">Example</span></span>

<span data-ttu-id="7f57a-132">L’exemple suivant d’une demande SetUserOofSettings permet **OofState**.</span><span class="sxs-lookup"><span data-stu-id="7f57a-132">The following example of a SetUserOofSettings request enables the **OofState**.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="7f57a-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7f57a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f57a-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7f57a-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f57a-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7f57a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="7f57a-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7f57a-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f57a-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7f57a-137">Validation File</span></span>  <br/> |<span data-ttu-id="7f57a-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7f57a-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f57a-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7f57a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f57a-140">False</span><span class="sxs-lookup"><span data-stu-id="7f57a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f57a-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7f57a-141">See also</span></span>



[<span data-ttu-id="7f57a-142">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7f57a-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="7f57a-143">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7f57a-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

