---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: L’élément SmtpAddress représente l’adresse SMTP Simple Mail Transfer Protocol () d’un compte à utiliser pour l’emprunt d’identité ou une adresse de destinataire SMTP Simple Mail Transfer Protocol () d’un calendrier ou d’une demande de partage de contact.
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829511"
---
# <a name="smtpaddress"></a><span data-ttu-id="7590a-103">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="7590a-103">SmtpAddress</span></span>

<span data-ttu-id="7590a-104">L’élément **SmtpAddress** représente l’adresse SMTP Simple Mail Transfer Protocol () d’un compte à utiliser pour l’emprunt d’identité ou une adresse de destinataire SMTP Simple Mail Transfer Protocol () d’un calendrier ou d’une demande de partage de contact.</span><span class="sxs-lookup"><span data-stu-id="7590a-104">The **SmtpAddress** element represents the Simple Mail Transfer Protocol (SMTP) address of an account to be used for impersonation or a Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span> 
  
```xml
<SmtpAddress/>
```

<span data-ttu-id="7590a-105">**SmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="7590a-105">**SmtpAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7590a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7590a-106">Attributes and elements</span></span>

<span data-ttu-id="7590a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7590a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7590a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7590a-108">Attributes</span></span>

<span data-ttu-id="7590a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7590a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7590a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7590a-110">Child elements</span></span>

<span data-ttu-id="7590a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7590a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7590a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7590a-112">Parent elements</span></span>

|<span data-ttu-id="7590a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7590a-113">**Element**</span></span>|<span data-ttu-id="7590a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7590a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7590a-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="7590a-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="7590a-116">Représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.</span><span class="sxs-lookup"><span data-stu-id="7590a-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="7590a-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="7590a-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="7590a-118">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="7590a-118">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="7590a-119">Représente un destinataire non valide pour un partage de calendrier ou un message de partage de contact.</span><span class="sxs-lookup"><span data-stu-id="7590a-119">Represents an invalid recipient for a calendar sharing or contact sharing message.</span></span>  <br/> |
|[<span data-ttu-id="7590a-120">Destinataires (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="7590a-120">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="7590a-121">Représente une collection de destinataires qui auront accès au dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="7590a-121">Represents a collection of recipients that will be granted access to the shared folder.</span></span>  <br/> |
|[<span data-ttu-id="7590a-122">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="7590a-122">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="7590a-123">Définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.</span><span class="sxs-lookup"><span data-stu-id="7590a-123">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7590a-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7590a-124">Text value</span></span>

<span data-ttu-id="7590a-125">Une valeur de texte qui représente une adresse SMTP est requise.</span><span class="sxs-lookup"><span data-stu-id="7590a-125">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7590a-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="7590a-126">Remarks</span></span>

<span data-ttu-id="7590a-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="7590a-127">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7590a-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7590a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7590a-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7590a-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7590a-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7590a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7590a-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7590a-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7590a-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7590a-132">Validation File</span></span>  <br/> |<span data-ttu-id="7590a-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7590a-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7590a-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7590a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7590a-135">False</span><span class="sxs-lookup"><span data-stu-id="7590a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7590a-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7590a-136">See also</span></span>

- [<span data-ttu-id="7590a-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7590a-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

