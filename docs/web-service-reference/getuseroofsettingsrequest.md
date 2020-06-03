---
title: GetUserOofSettingsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettingsRequest
api_type:
- schema
ms.assetid: 15dea99c-7f5d-4af1-82ff-4255127fe567
description: L’élément GetUserOofSettingsRequest est l’élément racine qui contient les arguments utilisés pour obtenir les paramètres d’absence du Bureau d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: f515e8cf016d3aff6c652ae92a0da71a8f0a5f6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457829"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="ebb73-103">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="ebb73-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="ebb73-104">L’élément **GetUserOofSettingsRequest** est l’élément racine qui contient les arguments utilisés pour obtenir les paramètres d’absence du Bureau d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ebb73-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="ebb73-105">**GetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="ebb73-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebb73-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ebb73-106">Attributes and elements</span></span>

<span data-ttu-id="ebb73-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ebb73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebb73-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ebb73-108">Attributes</span></span>

<span data-ttu-id="ebb73-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ebb73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebb73-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ebb73-110">Child elements</span></span>

|<span data-ttu-id="ebb73-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ebb73-111">**Element**</span></span>|<span data-ttu-id="ebb73-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ebb73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebb73-113">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="ebb73-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="ebb73-114">Identifie l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="ebb73-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ebb73-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ebb73-115">Parent elements</span></span>

<span data-ttu-id="ebb73-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebb73-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ebb73-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="ebb73-117">Remarks</span></span>

<span data-ttu-id="ebb73-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ebb73-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="ebb73-119">Exemple</span><span class="sxs-lookup"><span data-stu-id="ebb73-119">Example</span></span>

<span data-ttu-id="ebb73-120">Voici un exemple de requête GetUserOofSettings qui récupère les informations du Bureau d’veille d’un utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="ebb73-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="ebb73-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ebb73-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebb73-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ebb73-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ebb73-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ebb73-123">Schema Name</span></span>  <br/> |<span data-ttu-id="ebb73-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ebb73-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ebb73-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ebb73-125">Validation File</span></span>  <br/> |<span data-ttu-id="ebb73-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ebb73-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ebb73-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ebb73-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="ebb73-128">False</span><span class="sxs-lookup"><span data-stu-id="ebb73-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebb73-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ebb73-129">See also</span></span>



[<span data-ttu-id="ebb73-130">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="ebb73-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

