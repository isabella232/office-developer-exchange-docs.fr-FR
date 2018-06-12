---
title: SetUserOofSettingsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 628acf0b-3ebc-42f1-8ce2-7a02b4c8141f
description: L’élément SetUserOofSettingsRequest contient les arguments permet de définir des paramètres d’absence du bureau (OOF) de l’utilisateur une boîte aux lettres.
ms.openlocfilehash: ed54bb1d066da7b15605fb81931a6ef75dfc61bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829474"
---
# <a name="setuseroofsettingsrequest"></a><span data-ttu-id="ad644-103">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="ad644-103">SetUserOofSettingsRequest</span></span>

<span data-ttu-id="ad644-104">L’élément **SetUserOofSettingsRequest** contient les arguments permet de définir des paramètres d’absence du bureau (OOF) de l’utilisateur une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ad644-104">The **SetUserOofSettingsRequest** element contains the arguments used to set a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<SetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
   <UserOofSettings>...</UserOofSettings>
<SetUserOofSettingsRequest>
```

 <span data-ttu-id="ad644-105">**SetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="ad644-105">**SetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad644-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad644-106">Attributes and elements</span></span>

<span data-ttu-id="ad644-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad644-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad644-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad644-108">Attributes</span></span>

<span data-ttu-id="ad644-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad644-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad644-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad644-110">Child elements</span></span>

|<span data-ttu-id="ad644-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad644-111">**Element**</span></span>|<span data-ttu-id="ad644-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad644-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad644-113">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="ad644-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="ad644-114">Identifie l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="ad644-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
|[<span data-ttu-id="ad644-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ad644-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="ad644-116">Spécifie les paramètres d’absence du bureau.</span><span class="sxs-lookup"><span data-stu-id="ad644-116">Specifies the OOF settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad644-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad644-117">Parent elements</span></span>

<span data-ttu-id="ad644-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad644-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad644-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad644-119">Remarks</span></span>

<span data-ttu-id="ad644-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ad644-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="ad644-121">Exemple</span><span class="sxs-lookup"><span data-stu-id="ad644-121">Example</span></span>

<span data-ttu-id="ad644-122">L’exemple suivant d’une demande SetUserOofSettings définit un paramètre d’absence du bureau pour des dix derniers jours.</span><span class="sxs-lookup"><span data-stu-id="ad644-122">The following example of a SetUserOofSettings request sets an OOF setting for ten days.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="ad644-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad644-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad644-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad644-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ad644-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad644-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ad644-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ad644-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ad644-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad644-127">Validation File</span></span>  <br/> |<span data-ttu-id="ad644-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ad644-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad644-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad644-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad644-130">False</span><span class="sxs-lookup"><span data-stu-id="ad644-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad644-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad644-131">See also</span></span>



[<span data-ttu-id="ad644-132">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ad644-132">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

