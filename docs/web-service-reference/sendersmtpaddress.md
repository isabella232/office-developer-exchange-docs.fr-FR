---
title: SenderSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderSmtpAddress
api_type:
- schema
ms.assetid: e39c7df7-4bfa-455f-b4bb-1f1d05398eec
description: L’élément SenderSmtpAddress représente l’adresse de messagerie SMTP correspondant à la boîte aux lettres qui contient le dossier qui sera partagé.
ms.openlocfilehash: 70905dd1ae2c3df18224aceeea246b542d1338e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829334"
---
# <a name="sendersmtpaddress"></a><span data-ttu-id="1741f-103">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1741f-103">SenderSmtpAddress</span></span>

<span data-ttu-id="1741f-104">L’élément **SenderSmtpAddress** représente l’adresse de messagerie SMTP correspondant à la boîte aux lettres qui contient le dossier qui sera partagé.</span><span class="sxs-lookup"><span data-stu-id="1741f-104">The **SenderSmtpAddress** element represents the SMTP e-mail address corresponding to the mailbox that contains the folder that will be shared.</span></span> 
  
```xml
<SenderSmtpAddress/>
```

 <span data-ttu-id="1741f-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="1741f-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1741f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1741f-106">Attributes and elements</span></span>

<span data-ttu-id="1741f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1741f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1741f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1741f-108">Attributes</span></span>

<span data-ttu-id="1741f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1741f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1741f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1741f-110">Child elements</span></span>

<span data-ttu-id="1741f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1741f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1741f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1741f-112">Parent elements</span></span>

|<span data-ttu-id="1741f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1741f-113">**Element**</span></span>|<span data-ttu-id="1741f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1741f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1741f-115">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="1741f-115">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="1741f-116">Définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="1741f-116">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1741f-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1741f-117">Text value</span></span>

<span data-ttu-id="1741f-118">Une valeur de texte qui représente une adresse SMTP est requise.</span><span class="sxs-lookup"><span data-stu-id="1741f-118">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1741f-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="1741f-119">Remarks</span></span>

<span data-ttu-id="1741f-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="1741f-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1741f-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1741f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1741f-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1741f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1741f-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1741f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="1741f-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1741f-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1741f-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1741f-125">Validation File</span></span>  <br/> |<span data-ttu-id="1741f-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1741f-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1741f-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1741f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="1741f-128">False</span><span class="sxs-lookup"><span data-stu-id="1741f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1741f-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1741f-129">See also</span></span>



[<span data-ttu-id="1741f-130">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="1741f-130">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="1741f-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1741f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

