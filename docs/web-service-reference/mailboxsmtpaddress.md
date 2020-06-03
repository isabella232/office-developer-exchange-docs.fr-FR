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
description: L’élément MailboxSmtpAddress représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception doivent être récupérées ou mises à jour ; ou la date d’expiration du mot de passe à récupérer.
ms.openlocfilehash: 613e8098210257280bec47f2b22a2d29d04fa07c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530543"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="d24fc-103">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d24fc-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="d24fc-104">L’élément **MailboxSmtpAddress** représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception doivent être récupérées ou mises à jour ; ou la date d’expiration du mot de passe à récupérer.</span><span class="sxs-lookup"><span data-stu-id="d24fc-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="d24fc-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="d24fc-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d24fc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d24fc-106">Attributes and elements</span></span>

<span data-ttu-id="d24fc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d24fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d24fc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d24fc-108">Attributes</span></span>

<span data-ttu-id="d24fc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d24fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d24fc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d24fc-110">Child elements</span></span>

<span data-ttu-id="d24fc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d24fc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d24fc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d24fc-112">Parent elements</span></span>

|<span data-ttu-id="d24fc-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d24fc-113">**Element**</span></span>|<span data-ttu-id="d24fc-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d24fc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d24fc-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="d24fc-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="d24fc-116">Définit une demande pour obtenir les règles de boîte de réception sur une boîte aux lettres dans le magasin de serveurs.</span><span class="sxs-lookup"><span data-stu-id="d24fc-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="d24fc-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d24fc-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="d24fc-118">Définit une demande pour obtenir la date d’expiration du mot de passe d’un compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="d24fc-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="d24fc-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d24fc-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="d24fc-120">Définit une demande de mise à jour des règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="d24fc-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d24fc-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d24fc-121">Text value</span></span>

<span data-ttu-id="d24fc-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d24fc-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d24fc-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="d24fc-123">Remarks</span></span>

<span data-ttu-id="d24fc-124">L’élément **MailboxSmtpAddress** est un élément facultatif.</span><span class="sxs-lookup"><span data-stu-id="d24fc-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="d24fc-125">Si l’élément **MailboxSmtpAddress** est omis, l’adresse de l’utilisateur connecté est utilisée.</span><span class="sxs-lookup"><span data-stu-id="d24fc-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="d24fc-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d24fc-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d24fc-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d24fc-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d24fc-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d24fc-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d24fc-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d24fc-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d24fc-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d24fc-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d24fc-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d24fc-131">Validation File</span></span>  <br/> |<span data-ttu-id="d24fc-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d24fc-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d24fc-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d24fc-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d24fc-134">True</span><span class="sxs-lookup"><span data-stu-id="d24fc-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d24fc-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d24fc-135">See also</span></span>

- [<span data-ttu-id="d24fc-136">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="d24fc-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="d24fc-137">Opération GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d24fc-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="d24fc-138">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d24fc-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="d24fc-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d24fc-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

