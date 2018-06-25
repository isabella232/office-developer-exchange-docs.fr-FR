---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: L’élément MailboxSmtpAddress représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception sont à récupérer ou mis à jour ; ou dont la date d’expiration de mot de passe doit être récupéré.
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828303"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="7c1f7-103">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="7c1f7-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="7c1f7-104">L’élément **MailboxSmtpAddress** représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception sont à récupérer ou mis à jour ; ou dont la date d’expiration de mot de passe doit être récupéré.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="7c1f7-105">**string**</span><span class="sxs-lookup"><span data-stu-id="7c1f7-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7c1f7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7c1f7-106">Attributes and elements</span></span>

<span data-ttu-id="7c1f7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c1f7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7c1f7-108">Attributes</span></span>

<span data-ttu-id="7c1f7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c1f7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7c1f7-110">Child elements</span></span>

<span data-ttu-id="7c1f7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c1f7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7c1f7-112">Parent elements</span></span>

|<span data-ttu-id="7c1f7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7c1f7-113">**Element**</span></span>|<span data-ttu-id="7c1f7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7c1f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c1f7-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="7c1f7-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="7c1f7-116">Définit une requête pour obtenir les règles de boîte de réception sur une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="7c1f7-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="7c1f7-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="7c1f7-118">Définit une demande pour obtenir la date d’expiration de mot de passe d’un compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="7c1f7-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7c1f7-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="7c1f7-120">Définit une demande pour mettre à jour les règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c1f7-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7c1f7-121">Text value</span></span>

<span data-ttu-id="7c1f7-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c1f7-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="7c1f7-123">Remarks</span></span>

<span data-ttu-id="7c1f7-124">L’élément **MailboxSmtpAddress** est un élément facultatif.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="7c1f7-125">Si l’élément **MailboxSmtpAddress** est omis, l’adresse de l’utilisateur connecté est utilisé.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="7c1f7-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c1f7-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c1f7-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7c1f7-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c1f7-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7c1f7-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c1f7-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7c1f7-129">Schema Name</span></span>  <br/> |<span data-ttu-id="7c1f7-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7c1f7-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c1f7-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7c1f7-131">Validation File</span></span>  <br/> |<span data-ttu-id="7c1f7-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c1f7-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c1f7-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7c1f7-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c1f7-134">True</span><span class="sxs-lookup"><span data-stu-id="7c1f7-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c1f7-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7c1f7-135">See also</span></span>

- [<span data-ttu-id="7c1f7-136">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="7c1f7-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="7c1f7-137">Opération GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="7c1f7-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="7c1f7-138">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="7c1f7-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="7c1f7-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7c1f7-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

