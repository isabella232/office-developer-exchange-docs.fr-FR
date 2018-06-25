---
title: ActingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: L’élément ActingAs identifie qui envoie en tant que l’appelant.
ms.openlocfilehash: 9c007ed45f85dba265261dd79a6fd846dbd9d2f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756336"
---
# <a name="actingas"></a><span data-ttu-id="f3ff9-103">ActingAs</span><span class="sxs-lookup"><span data-stu-id="f3ff9-103">ActingAs</span></span>

<span data-ttu-id="f3ff9-104">L’élément **ActingAs** identifie qui envoie en tant que l’appelant.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-104">The **ActingAs** element identifies who the caller is sending as.</span></span> 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 <span data-ttu-id="f3ff9-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="f3ff9-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3ff9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f3ff9-106">Attributes and elements</span></span>

<span data-ttu-id="f3ff9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3ff9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f3ff9-108">Attributes</span></span>

<span data-ttu-id="f3ff9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3ff9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f3ff9-110">Child elements</span></span>

|<span data-ttu-id="f3ff9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f3ff9-111">**Element**</span></span>|<span data-ttu-id="f3ff9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f3ff9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3ff9-113">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="f3ff9-113">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="f3ff9-114">Définit l’adresse SMTP Simple Mail Transfer Protocol () d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-114">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="f3ff9-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f3ff9-116">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f3ff9-116">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="f3ff9-117">Définit le routage est utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-117">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="f3ff9-118">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-118">The default is SMTP.</span></span> <span data-ttu-id="f3ff9-119">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3ff9-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f3ff9-120">Parent elements</span></span>

|<span data-ttu-id="f3ff9-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f3ff9-121">**Element**</span></span>|<span data-ttu-id="f3ff9-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="f3ff9-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3ff9-123">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3ff9-123">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="f3ff9-124">Définit une demande **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="f3ff9-124">Defines a **GetServiceConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f3ff9-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="f3ff9-125">Remarks</span></span>

<span data-ttu-id="f3ff9-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-126">This element is optional.</span></span> <span data-ttu-id="f3ff9-127">Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-127">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="f3ff9-128">L’élément **ActingAs** doit être inclus pour demander des conseils de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-128">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="f3ff9-129">Une erreur **ErrorInvalidArgument** peut être renvoyée dans une réponse si l’élément **ActingAs** est manquant, n’inclut pas un type de routage, n’inclut pas une adresse de messagerie, contient une adresse de messagerie non valides, ne correspond pas à un utilisateur dans Active Directory Domaine Services (AD DS), ou correspond à plusieurs utilisateurs dans AD DS.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-129">An **ErrorInvalidArgument** error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span> 
  
<span data-ttu-id="f3ff9-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3ff9-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3ff9-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f3ff9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3ff9-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f3ff9-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3ff9-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f3ff9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f3ff9-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f3ff9-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3ff9-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f3ff9-135">Validation File</span></span>  <br/> |<span data-ttu-id="f3ff9-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f3ff9-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3ff9-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f3ff9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3ff9-138">False</span><span class="sxs-lookup"><span data-stu-id="f3ff9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3ff9-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f3ff9-139">See also</span></span>

- [<span data-ttu-id="f3ff9-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f3ff9-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

