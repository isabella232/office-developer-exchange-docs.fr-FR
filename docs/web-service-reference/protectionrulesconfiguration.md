---
title: ProtectionRulesConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProtectionRulesConfiguration
api_type:
- schema
ms.assetid: e5b4699a-476e-4053-bb52-873eb921c046
description: L’élément ProtectionRulesConfiguration contient des informations de configuration de service pour le service de règles de protection.
ms.openlocfilehash: 9c286fcf9752d591d53323f45a264f4bdd078c1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828912"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="c5516-103">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5516-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="c5516-104">L’élément **ProtectionRulesConfiguration** contient des informations de configuration de service pour le service de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="c5516-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="c5516-105">**ProtectionRulesServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="c5516-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5516-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c5516-106">Attributes and elements</span></span>

<span data-ttu-id="c5516-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c5516-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5516-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c5516-108">Attributes</span></span>

|<span data-ttu-id="c5516-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c5516-109">**Attribute**</span></span>|<span data-ttu-id="c5516-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5516-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c5516-111">**RefreshInterval**</span><span class="sxs-lookup"><span data-stu-id="c5516-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="c5516-112">Spécifie la fréquence, en heures entières, le client doit demander des règles de protection à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="c5516-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="c5516-113">Cet attribut est obligatoire et sa valeur doit être un entier qui est égale ou supérieure à 1.</span><span class="sxs-lookup"><span data-stu-id="c5516-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c5516-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c5516-114">Child elements</span></span>

|<span data-ttu-id="c5516-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5516-115">**Element**</span></span>|<span data-ttu-id="c5516-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5516-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5516-117">Règles</span><span class="sxs-lookup"><span data-stu-id="c5516-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c5516-118">Tableau des règles de protection.</span><span class="sxs-lookup"><span data-stu-id="c5516-118">An array of protection rules.</span></span> <span data-ttu-id="c5516-119">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c5516-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="c5516-120">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="c5516-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="c5516-121">Identifie la liste des domaines SMTP internes de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="c5516-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="c5516-122">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="c5516-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5516-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c5516-123">Parent elements</span></span>

|<span data-ttu-id="c5516-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5516-124">**Element**</span></span>|<span data-ttu-id="c5516-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5516-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5516-126">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="c5516-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="c5516-127">Contient les paramètres de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="c5516-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c5516-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c5516-128">Text value</span></span>

<span data-ttu-id="c5516-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c5516-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c5516-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="c5516-130">Remarks</span></span>

<span data-ttu-id="c5516-131">La configuration de service des règles de protection est constituée d’une liste de règles, les domaines internes et un intervalle d’actualisation.</span><span class="sxs-lookup"><span data-stu-id="c5516-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="c5516-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5516-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5516-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c5516-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5516-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c5516-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c5516-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c5516-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c5516-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c5516-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c5516-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c5516-137">Validation File</span></span>  <br/> |<span data-ttu-id="c5516-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c5516-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c5516-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c5516-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5516-140">False</span><span class="sxs-lookup"><span data-stu-id="c5516-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5516-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c5516-141">See also</span></span>



- [<span data-ttu-id="c5516-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c5516-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

