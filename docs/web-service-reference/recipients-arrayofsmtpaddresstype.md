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
description: L’élément destinataires spécifie un tableau de destinataires d’un message.
ms.openlocfilehash: 8490988043b1e06fd3a8f553fcefaeb2e90e9d31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828988"
---
# <a name="recipients-arrayofsmtpaddresstype"></a><span data-ttu-id="1a56e-103">Destinataires (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="1a56e-103">Recipients (ArrayOfSmtpAddressType)</span></span>

<span data-ttu-id="1a56e-104">L’élément **destinataires** spécifie un tableau de destinataires d’un message.</span><span class="sxs-lookup"><span data-stu-id="1a56e-104">The **Recipients** element specifies an array of recipients of a message.</span></span> 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 <span data-ttu-id="1a56e-105">**ArrayOfSmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="1a56e-105">**ArrayOfSmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a56e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1a56e-106">Attributes and elements</span></span>

<span data-ttu-id="1a56e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1a56e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a56e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1a56e-108">Attributes</span></span>

<span data-ttu-id="1a56e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1a56e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a56e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1a56e-110">Child elements</span></span>

|<span data-ttu-id="1a56e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a56e-111">**Element**</span></span>|<span data-ttu-id="1a56e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a56e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a56e-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1a56e-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="1a56e-114">Représente l’adresse du destinataire d’un calendrier ou d’une demande de partage de contact SMTP Simple Mail Transfer Protocol ().</span><span class="sxs-lookup"><span data-stu-id="1a56e-114">Represents the Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a56e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1a56e-115">Parent elements</span></span>

|<span data-ttu-id="1a56e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a56e-116">**Element**</span></span>|<span data-ttu-id="1a56e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a56e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a56e-118">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="1a56e-118">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="1a56e-119">Définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="1a56e-119">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1a56e-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="1a56e-120">Remarks</span></span>

<span data-ttu-id="1a56e-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="1a56e-121">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a56e-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1a56e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a56e-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1a56e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a56e-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1a56e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1a56e-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1a56e-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1a56e-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1a56e-126">Validation File</span></span>  <br/> |<span data-ttu-id="1a56e-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1a56e-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a56e-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1a56e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a56e-129">False</span><span class="sxs-lookup"><span data-stu-id="1a56e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a56e-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1a56e-130">See also</span></span>



[<span data-ttu-id="1a56e-131">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="1a56e-131">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="1a56e-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1a56e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

