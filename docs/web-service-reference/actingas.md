---
title: Actionas
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
description: L’élément Actionas identifie les personnes qui envoient l’appelant.
ms.openlocfilehash: 175a03018ee3529ec595dbe9afb7dc61ad6afc35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529699"
---
# <a name="actingas"></a><span data-ttu-id="e1356-103">Actionas</span><span class="sxs-lookup"><span data-stu-id="e1356-103">ActingAs</span></span>

<span data-ttu-id="e1356-104">L’élément **actionas** identifie les personnes qui envoient l’appelant.</span><span class="sxs-lookup"><span data-stu-id="e1356-104">The **ActingAs** element identifies who the caller is sending as.</span></span> 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 <span data-ttu-id="e1356-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="e1356-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1356-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e1356-106">Attributes and elements</span></span>

<span data-ttu-id="e1356-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e1356-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1356-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e1356-108">Attributes</span></span>

<span data-ttu-id="e1356-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e1356-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1356-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e1356-110">Child elements</span></span>

|<span data-ttu-id="e1356-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1356-111">**Element**</span></span>|<span data-ttu-id="e1356-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1356-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1356-113">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="e1356-113">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="e1356-114">Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e1356-114">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="e1356-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e1356-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e1356-116">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="e1356-116">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="e1356-117">Définit le routage utilisé pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e1356-117">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="e1356-118">La valeur par défaut est SMTP.</span><span class="sxs-lookup"><span data-stu-id="e1356-118">The default is SMTP.</span></span> <span data-ttu-id="e1356-119">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e1356-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1356-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e1356-120">Parent elements</span></span>

|<span data-ttu-id="e1356-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1356-121">**Element**</span></span>|<span data-ttu-id="e1356-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1356-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1356-123">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1356-123">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="e1356-124">Définit une requête **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="e1356-124">Defines a **GetServiceConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1356-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="e1356-125">Remarks</span></span>

<span data-ttu-id="e1356-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e1356-126">This element is optional.</span></span> <span data-ttu-id="e1356-127">Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="e1356-127">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="e1356-128">L’élément **actionas** doit être inclus pour la demande d’indications de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="e1356-128">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="e1356-129">Une erreur **ErrorInvalidArgument** peut être renvoyée dans une réponse si l’élément **actionas** est manquant, qu’il n’inclut pas de type de routage, qu’il n’inclut pas d’adresse de messagerie, qu’il contient une adresse de messagerie non valide, qu’il n’est pas résolu en utilisateur dans les services de domaine Active Directory (AD DS) ou qu’il est résolu en plusieurs utilisateurs dans AD DS.</span><span class="sxs-lookup"><span data-stu-id="e1356-129">An **ErrorInvalidArgument** error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span> 
  
<span data-ttu-id="e1356-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1356-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1356-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e1356-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1356-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e1356-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e1356-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e1356-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e1356-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e1356-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e1356-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e1356-135">Validation File</span></span>  <br/> |<span data-ttu-id="e1356-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e1356-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1356-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e1356-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1356-138">False</span><span class="sxs-lookup"><span data-stu-id="e1356-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1356-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e1356-139">See also</span></span>

- [<span data-ttu-id="e1356-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e1356-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

