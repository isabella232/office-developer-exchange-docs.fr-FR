---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: L’élément GetSharingMetadata définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage. Cet élément est l’élément de base pour l’opération GetSharingMetadata.
ms.openlocfilehash: 406908e566d6d4249003b1a19a9ce79b8b328c4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530845"
---
# <a name="getsharingmetadata"></a><span data-ttu-id="b5d2d-104">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="b5d2d-104">GetSharingMetadata</span></span>

<span data-ttu-id="b5d2d-105">L’élément **GetSharingMetadata** définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-105">The **GetSharingMetadata** element defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span> <span data-ttu-id="b5d2d-106">Cet élément est l’élément de base pour l' [opération GetSharingMetadata](getsharingmetadata-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b5d2d-106">This element is the base element for the [GetSharingMetadata operation](getsharingmetadata-operation.md).</span></span>
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 <span data-ttu-id="b5d2d-107">**GetSharingMetadataType**</span><span class="sxs-lookup"><span data-stu-id="b5d2d-107">**GetSharingMetadataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5d2d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b5d2d-108">Attributes and elements</span></span>

<span data-ttu-id="b5d2d-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5d2d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="b5d2d-110">Attributes</span></span>

<span data-ttu-id="b5d2d-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5d2d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b5d2d-112">Child elements</span></span>

|<span data-ttu-id="b5d2d-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b5d2d-113">**Element**</span></span>|<span data-ttu-id="b5d2d-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b5d2d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5d2d-115">IdOfFolderToShare</span><span class="sxs-lookup"><span data-stu-id="b5d2d-115">IdOfFolderToShare</span></span>](idoffoldertoshare.md) <br/> |<span data-ttu-id="b5d2d-116">Représente l’identificateur du dossier sur le serveur qui sera partagé.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-116">Represents the identifier of the folder on the server that will be shared.</span></span> <span data-ttu-id="b5d2d-117">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="b5d2d-118">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="b5d2d-118">SenderSmtpAddress</span></span>](sendersmtpaddress.md) <br/> |<span data-ttu-id="b5d2d-119">Représente l’adresse de messagerie SMTP qui correspond à la boîte aux lettres qui contient le dossier identifié par l’élément [IdOfFolderToShare](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="b5d2d-119">Represents the SMTP email address that corresponds to the mailbox that contains the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="b5d2d-120">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="b5d2d-121">Destinataires (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="b5d2d-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="b5d2d-122">Représente les adresses de messagerie SMTP d’une ou plusieurs entités qui seront autorisées à accéder aux données dans le dossier identifié par l’élément [IdOfFolderToShare](idoffoldertoshare.md) .</span><span class="sxs-lookup"><span data-stu-id="b5d2d-122">Represents the SMTP email addresses of one or more entities that will be granted access to the data in the folder that is identified by the [IdOfFolderToShare](idoffoldertoshare.md) element.</span></span> <span data-ttu-id="b5d2d-123">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-123">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b5d2d-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b5d2d-124">Parent elements</span></span>

<span data-ttu-id="b5d2d-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b5d2d-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5d2d-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b5d2d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5d2d-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b5d2d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b5d2d-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b5d2d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b5d2d-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b5d2d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b5d2d-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b5d2d-130">Validation File</span></span>  <br/> |<span data-ttu-id="b5d2d-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b5d2d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b5d2d-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b5d2d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b5d2d-133">False</span><span class="sxs-lookup"><span data-stu-id="b5d2d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5d2d-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b5d2d-134">See also</span></span>



[<span data-ttu-id="b5d2d-135">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="b5d2d-135">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="b5d2d-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b5d2d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

