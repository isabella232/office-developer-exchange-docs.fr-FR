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
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457871"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="2aaea-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2aaea-103">GetServiceConfiguration</span></span>

<span data-ttu-id="2aaea-104">L’élément **GetServiceConfiguration** définit une demande GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2aaea-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="2aaea-105">**GetServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="2aaea-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2aaea-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2aaea-106">Attributes and elements</span></span>

<span data-ttu-id="2aaea-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2aaea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2aaea-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2aaea-108">Attributes</span></span>

<span data-ttu-id="2aaea-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2aaea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2aaea-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2aaea-110">Child elements</span></span>

|<span data-ttu-id="2aaea-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2aaea-111">**Element**</span></span>|<span data-ttu-id="2aaea-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2aaea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2aaea-113">Actionas</span><span class="sxs-lookup"><span data-stu-id="2aaea-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="2aaea-114">Identifie les personnes qui envoient l’appelant.</span><span class="sxs-lookup"><span data-stu-id="2aaea-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="2aaea-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="2aaea-115">This element is optional.</span></span> <span data-ttu-id="2aaea-116">Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="2aaea-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="2aaea-117">L’élément **actionas** doit être inclus pour la demande d’indications de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="2aaea-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="2aaea-118">Une erreur ErrorInvalidArgument peut être renvoyée dans une réponse si l’élément **actionas** est manquant, qu’il n’inclut pas de type de routage, qu’il n’inclut pas d’adresse de messagerie, qu’il contient une adresse de messagerie non valide, qu’il n’est pas résolu en utilisateur dans les services de domaine Active Directory (AD DS) ou qu’il est résolu en plusieurs utilisateurs dans AD DS.</span><span class="sxs-lookup"><span data-stu-id="2aaea-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="2aaea-119">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="2aaea-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="2aaea-120">Contient les configurations de service demandées.</span><span class="sxs-lookup"><span data-stu-id="2aaea-120">Contains the requested service configurations.</span></span> <span data-ttu-id="2aaea-121">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="2aaea-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2aaea-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2aaea-122">Parent elements</span></span>

<span data-ttu-id="2aaea-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2aaea-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2aaea-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2aaea-124">Text value</span></span>

<span data-ttu-id="2aaea-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2aaea-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2aaea-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="2aaea-126">Remarks</span></span>

<span data-ttu-id="2aaea-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2aaea-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2aaea-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2aaea-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2aaea-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2aaea-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2aaea-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2aaea-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2aaea-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2aaea-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2aaea-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2aaea-132">Validation File</span></span>  <br/> |<span data-ttu-id="2aaea-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2aaea-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2aaea-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2aaea-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2aaea-135">False</span><span class="sxs-lookup"><span data-stu-id="2aaea-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2aaea-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2aaea-136">See also</span></span>



- [<span data-ttu-id="2aaea-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2aaea-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

