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
ms.openlocfilehash: 73047dcecfbccb55d74e373891c3154bc7baeeba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464895"
---
# <a name="sendersmtpaddress"></a><span data-ttu-id="a76db-103">SenderSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a76db-103">SenderSmtpAddress</span></span>

<span data-ttu-id="a76db-104">L’élément **SenderSmtpAddress** représente l’adresse de messagerie SMTP correspondant à la boîte aux lettres qui contient le dossier qui sera partagé.</span><span class="sxs-lookup"><span data-stu-id="a76db-104">The **SenderSmtpAddress** element represents the SMTP e-mail address corresponding to the mailbox that contains the folder that will be shared.</span></span> 
  
```xml
<SenderSmtpAddress/>
```

 <span data-ttu-id="a76db-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="a76db-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a76db-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a76db-106">Attributes and elements</span></span>

<span data-ttu-id="a76db-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a76db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a76db-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a76db-108">Attributes</span></span>

<span data-ttu-id="a76db-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a76db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a76db-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a76db-110">Child elements</span></span>

<span data-ttu-id="a76db-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a76db-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a76db-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a76db-112">Parent elements</span></span>

|<span data-ttu-id="a76db-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a76db-113">**Element**</span></span>|<span data-ttu-id="a76db-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a76db-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a76db-115">GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="a76db-115">GetSharingMetadata</span></span>](getsharingmetadata.md) <br/> |<span data-ttu-id="a76db-116">Définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.</span><span class="sxs-lookup"><span data-stu-id="a76db-116">Defines a request to get an opaque authentication token that identifies the sharing invitation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a76db-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a76db-117">Text value</span></span>

<span data-ttu-id="a76db-118">Une valeur de texte qui représente une adresse SMTP est requise.</span><span class="sxs-lookup"><span data-stu-id="a76db-118">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a76db-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="a76db-119">Remarks</span></span>

<span data-ttu-id="a76db-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a76db-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a76db-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a76db-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a76db-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a76db-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a76db-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a76db-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a76db-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a76db-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a76db-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a76db-125">Validation File</span></span>  <br/> |<span data-ttu-id="a76db-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a76db-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a76db-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a76db-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a76db-128">False</span><span class="sxs-lookup"><span data-stu-id="a76db-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a76db-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a76db-129">See also</span></span>



[<span data-ttu-id="a76db-130">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="a76db-130">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="a76db-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a76db-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

