---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: L’élément GetServiceConfiguration définit une demande GetServiceConfiguration.
ms.openlocfilehash: 7ff7124ff062f21a02fc69b86b7cc7367ba3fcb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827666"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="9a17a-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a17a-103">GetServiceConfiguration</span></span>

<span data-ttu-id="9a17a-104">L’élément **GetServiceConfiguration** définit une demande GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9a17a-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="9a17a-105">**GetServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="9a17a-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a17a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a17a-106">Attributes and elements</span></span>

<span data-ttu-id="9a17a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a17a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a17a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a17a-108">Attributes</span></span>

<span data-ttu-id="9a17a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a17a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a17a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a17a-110">Child elements</span></span>

|<span data-ttu-id="9a17a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a17a-111">**Element**</span></span>|<span data-ttu-id="9a17a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a17a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a17a-113">ActingAs</span><span class="sxs-lookup"><span data-stu-id="9a17a-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="9a17a-114">Identifie les personnes envoie par l’appelant.</span><span class="sxs-lookup"><span data-stu-id="9a17a-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="9a17a-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="9a17a-115">This element is optional.</span></span> <span data-ttu-id="9a17a-116">Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="9a17a-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="9a17a-117">L’élément **ActingAs** doit être inclus pour demander des conseils de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="9a17a-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="9a17a-118">Une erreur ErrorInvalidArgument peut être renvoyée dans une réponse si l’élément **ActingAs** est manquant, n’inclut pas un type de routage, n’inclut pas une adresse de messagerie, contient une adresse de messagerie non valides, ne résout pas à un utilisateur de domaine Active Directory Services (AD DS), ou résout à plusieurs utilisateurs dans AD DS.</span><span class="sxs-lookup"><span data-stu-id="9a17a-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="9a17a-119">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a17a-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="9a17a-120">Contient les configurations de service demandé.</span><span class="sxs-lookup"><span data-stu-id="9a17a-120">Contains the requested service configurations.</span></span> <span data-ttu-id="9a17a-121">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="9a17a-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a17a-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a17a-122">Parent elements</span></span>

<span data-ttu-id="9a17a-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a17a-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9a17a-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9a17a-124">Text value</span></span>

<span data-ttu-id="9a17a-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a17a-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a17a-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a17a-126">Remarks</span></span>

<span data-ttu-id="9a17a-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a17a-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a17a-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9a17a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a17a-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9a17a-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a17a-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9a17a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9a17a-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="9a17a-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9a17a-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9a17a-132">Validation File</span></span>  <br/> |<span data-ttu-id="9a17a-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9a17a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a17a-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9a17a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a17a-135">False</span><span class="sxs-lookup"><span data-stu-id="9a17a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a17a-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a17a-136">See also</span></span>



- [<span data-ttu-id="9a17a-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9a17a-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

