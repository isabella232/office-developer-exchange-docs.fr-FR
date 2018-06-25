---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: L’élément GetPasswordExpirationDate définit une demande pour obtenir la date d’expiration de mot de passe pour un compte de messagerie. Cet élément est l’élément de base pour l’opération GetPasswordExpirationDate.
ms.openlocfilehash: a9e0955566372f7b99c48c56e62ce2c5025f9f95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756703"
---
# <a name="getpasswordexpirationdate"></a><span data-ttu-id="6e54a-104">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="6e54a-104">GetPasswordExpirationDate</span></span>

<span data-ttu-id="6e54a-105">L’élément **GetPasswordExpirationDate** définit une demande pour obtenir la date d’expiration de mot de passe pour un compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="6e54a-105">The **GetPasswordExpirationDate** element defines a request to get the password expiration date for an email account.</span></span> <span data-ttu-id="6e54a-106">Cet élément est l’élément de base pour l’opération [GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6e54a-106">This element is the base element for the [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation.</span></span> 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 <span data-ttu-id="6e54a-107">**GetPasswordExpirationDateType**</span><span class="sxs-lookup"><span data-stu-id="6e54a-107">**GetPasswordExpirationDateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e54a-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6e54a-108">Attributes and elements</span></span>

<span data-ttu-id="6e54a-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6e54a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e54a-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="6e54a-110">Attributes</span></span>

<span data-ttu-id="6e54a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e54a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e54a-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6e54a-112">Child elements</span></span>

|<span data-ttu-id="6e54a-113">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="6e54a-113">**Element name**</span></span>|<span data-ttu-id="6e54a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6e54a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e54a-115">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="6e54a-115">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="6e54a-116">Représente l’adresse de messagerie du compte de messagerie pour lequel la date d’expiration de mot de passe doit être retourné.</span><span class="sxs-lookup"><span data-stu-id="6e54a-116">Represents the email address of the email account for which the password expiration date is to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e54a-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6e54a-117">Parent elements</span></span>

<span data-ttu-id="6e54a-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6e54a-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e54a-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="6e54a-119">Remarks</span></span>

<span data-ttu-id="6e54a-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e54a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="6e54a-121">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="6e54a-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e54a-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6e54a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e54a-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6e54a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e54a-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6e54a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6e54a-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6e54a-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e54a-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6e54a-126">Validation File</span></span>  <br/> |<span data-ttu-id="6e54a-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e54a-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e54a-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6e54a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e54a-129">False</span><span class="sxs-lookup"><span data-stu-id="6e54a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e54a-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6e54a-130">See also</span></span>



[<span data-ttu-id="6e54a-131">Opération GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="6e54a-131">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)


- [<span data-ttu-id="6e54a-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6e54a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

