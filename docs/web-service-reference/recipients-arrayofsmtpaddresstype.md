---
title: Destinataires (ArrayOfSmtpAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: cf68417d-85cf-49e0-857a-f987d3675344
description: L’élément Recipients spécifie un tableau de destinataires d’un message.
ms.openlocfilehash: 4c2478a81836c2e52baad9c928d112108679b837
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465505"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="6c8a9-103">Destinataires (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="6c8a9-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="6c8a9-104">L’élément **Recipients** spécifie un tableau de destinataires d’un message.</span><span class="sxs-lookup"><span data-stu-id="6c8a9-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="6c8a9-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="6c8a9-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c8a9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6c8a9-106">Attributes and elements</span></span>

<span data-ttu-id="6c8a9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6c8a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c8a9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6c8a9-108">Attributes</span></span>

<span data-ttu-id="6c8a9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6c8a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c8a9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6c8a9-110">Child elements</span></span>

|<span data-ttu-id="6c8a9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6c8a9-111">**Element**</span></span>|<span data-ttu-id="6c8a9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6c8a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c8a9-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="6c8a9-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="6c8a9-114">Représente l’adresse de destinataire SMTP (Simple Mail Transfer Protocol) d’une demande de partage de calendrier ou de contact.</span><span class="sxs-lookup"><span data-stu-id="6c8a9-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c8a9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6c8a9-115">Parent elements</span></span>

|<span data-ttu-id="6c8a9-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6c8a9-116">**Element**</span></span>|<span data-ttu-id="6c8a9-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6c8a9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c8a9-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="6c8a9-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="6c8a9-119">Définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="6c8a9-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c8a9-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="6c8a9-120">Remarks</span></span>

<span data-ttu-id="6c8a9-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6c8a9-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c8a9-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6c8a9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c8a9-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6c8a9-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c8a9-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6c8a9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6c8a9-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6c8a9-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c8a9-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6c8a9-126">Validation File</span></span>  <br/> |<span data-ttu-id="6c8a9-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6c8a9-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c8a9-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6c8a9-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c8a9-129">False</span><span class="sxs-lookup"><span data-stu-id="6c8a9-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c8a9-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6c8a9-130">See also</span></span>



[<span data-ttu-id="6c8a9-131">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="6c8a9-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="6c8a9-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6c8a9-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

