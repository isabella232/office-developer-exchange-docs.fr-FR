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
description: L’élément SetUserOofSettingsRequest contient les arguments utilisés pour définir les paramètres d’absence du Bureau (OOF) d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: 10edc9809fd72f80c316de1c6688eaedec4f93df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466149"
---
# <a name="setuseroofsettingsrequest"></a><span data-ttu-id="4b088-103">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="4b088-103">SetUserOofSettingsRequest</span></span>

<span data-ttu-id="4b088-104">L’élément **SetUserOofSettingsRequest** contient les arguments utilisés pour définir les paramètres d’absence du Bureau (OOF) d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4b088-104">The **SetUserOofSettingsRequest** element contains the arguments used to set a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<SetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
   <UserOofSettings>...</UserOofSettings>
<SetUserOofSettingsRequest>
```

 <span data-ttu-id="4b088-105">**SetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="4b088-105">**SetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b088-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b088-106">Attributes and elements</span></span>

<span data-ttu-id="4b088-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b088-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b088-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b088-108">Attributes</span></span>

<span data-ttu-id="4b088-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4b088-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b088-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b088-110">Child elements</span></span>

|<span data-ttu-id="4b088-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b088-111">**Element**</span></span>|<span data-ttu-id="4b088-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b088-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b088-113">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="4b088-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="4b088-114">Identifie l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="4b088-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
|[<span data-ttu-id="4b088-115">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4b088-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="4b088-116">Spécifie les paramètres OOF.</span><span class="sxs-lookup"><span data-stu-id="4b088-116">Specifies the OOF settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b088-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b088-117">Parent elements</span></span>

<span data-ttu-id="4b088-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b088-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4b088-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b088-119">Remarks</span></span>

<span data-ttu-id="4b088-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4b088-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="4b088-121">Exemple</span><span class="sxs-lookup"><span data-stu-id="4b088-121">Example</span></span>

<span data-ttu-id="4b088-122">L’exemple de requête SetUserOofSettings suivant définit un paramètre OOF sur 10 jours.</span><span class="sxs-lookup"><span data-stu-id="4b088-122">The following example of a SetUserOofSettings request sets an OOF setting for ten days.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="4b088-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b088-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b088-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b088-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b088-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b088-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4b088-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4b088-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4b088-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b088-127">Validation File</span></span>  <br/> |<span data-ttu-id="4b088-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4b088-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b088-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b088-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b088-130">False</span><span class="sxs-lookup"><span data-stu-id="4b088-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b088-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b088-131">See also</span></span>



[<span data-ttu-id="4b088-132">Opération SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="4b088-132">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

