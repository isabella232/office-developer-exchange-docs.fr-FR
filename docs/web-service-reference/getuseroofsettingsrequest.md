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
description: L’élément GetUserOofSettingsRequest est l’élément racine qui contient les arguments utilisés pour obtenir des paramètres d’absence du bureau (OOF) de l’utilisateur une boîte aux lettres.
ms.openlocfilehash: e64818961283f90e447e2044cf7f918eccd21f06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827692"
---
# <a name="getuseroofsettingsrequest"></a><span data-ttu-id="18ce2-103">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="18ce2-103">GetUserOofSettingsRequest</span></span>

<span data-ttu-id="18ce2-104">L’élément **GetUserOofSettingsRequest** est l’élément racine qui contient les arguments utilisés pour obtenir des paramètres d’absence du bureau (OOF) de l’utilisateur une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="18ce2-104">The **GetUserOofSettingsRequest** element is the root element that contains the arguments used to get a mailbox user's Out of Office (OOF) settings.</span></span> 
  
```xml
<GetUserOofSettingsRequest>
   <Mailbox>...</Mailbox>
</GetUserOofSettingsRequest>
```

 <span data-ttu-id="18ce2-105">**GetUserOofSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="18ce2-105">**GetUserOofSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18ce2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="18ce2-106">Attributes and elements</span></span>

<span data-ttu-id="18ce2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="18ce2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18ce2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="18ce2-108">Attributes</span></span>

<span data-ttu-id="18ce2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="18ce2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18ce2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="18ce2-110">Child elements</span></span>

|<span data-ttu-id="18ce2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="18ce2-111">**Element**</span></span>|<span data-ttu-id="18ce2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="18ce2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18ce2-113">Boîte aux lettres (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="18ce2-113">Mailbox (Availability)</span></span>](mailbox-availability.md) <br/> |<span data-ttu-id="18ce2-114">Identifie l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.</span><span class="sxs-lookup"><span data-stu-id="18ce2-114">Identifies the mailbox user for a SetUserOofSettings or GetUserOofSettings request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18ce2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="18ce2-115">Parent elements</span></span>

<span data-ttu-id="18ce2-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="18ce2-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18ce2-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="18ce2-117">Remarks</span></span>

<span data-ttu-id="18ce2-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="18ce2-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="18ce2-119">Exemple</span><span class="sxs-lookup"><span data-stu-id="18ce2-119">Example</span></span>

<span data-ttu-id="18ce2-120">Voici un exemple d’une demande GetUserOofSettings qui obtient des informations d’absence du bureau d’un utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="18ce2-120">The following is an example of a GetUserOofSettings request that gets a single user's OOF information.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="18ce2-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="18ce2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18ce2-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="18ce2-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="18ce2-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="18ce2-123">Schema Name</span></span>  <br/> |<span data-ttu-id="18ce2-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="18ce2-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="18ce2-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="18ce2-125">Validation File</span></span>  <br/> |<span data-ttu-id="18ce2-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="18ce2-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="18ce2-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="18ce2-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="18ce2-128">False</span><span class="sxs-lookup"><span data-stu-id="18ce2-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18ce2-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="18ce2-129">See also</span></span>



[<span data-ttu-id="18ce2-130">Opération GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="18ce2-130">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)

