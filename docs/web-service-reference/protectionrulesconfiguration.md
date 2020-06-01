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
description: L’élément ProtectionRulesConfiguration contient les informations de configuration de service pour le service de règles de protection.
ms.openlocfilehash: e664fba78f170c9f4c59b49b3a08c0dd2e4ed4cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456758"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="bc3f4-103">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc3f4-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="bc3f4-104">L’élément **ProtectionRulesConfiguration** contient les informations de configuration de service pour le service de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="bc3f4-105">**ProtectionRulesServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc3f4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bc3f4-106">Attributes and elements</span></span>

<span data-ttu-id="bc3f4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc3f4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bc3f4-108">Attributes</span></span>

|<span data-ttu-id="bc3f4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-109">**Attribute**</span></span>|<span data-ttu-id="bc3f4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc3f4-111">**RefreshInterval**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="bc3f4-112">Spécifie la fréquence, en heures entières, à laquelle le client doit demander des règles de protection auprès du serveur.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="bc3f4-113">Cet attribut est obligatoire et sa valeur doit être un entier supérieur ou égal à 1.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bc3f4-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bc3f4-114">Child elements</span></span>

|<span data-ttu-id="bc3f4-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-115">**Element**</span></span>|<span data-ttu-id="bc3f4-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc3f4-117">Gestion</span><span class="sxs-lookup"><span data-stu-id="bc3f4-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bc3f4-118">Tableau de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-118">An array of protection rules.</span></span> <span data-ttu-id="bc3f4-119">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="bc3f4-120">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="bc3f4-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="bc3f4-121">Identifie la liste des domaines SMTP internes de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="bc3f4-122">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc3f4-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bc3f4-123">Parent elements</span></span>

|<span data-ttu-id="bc3f4-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-124">**Element**</span></span>|<span data-ttu-id="bc3f4-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc3f4-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc3f4-126">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="bc3f4-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="bc3f4-127">Contient les paramètres de configuration du service.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc3f4-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bc3f4-128">Text value</span></span>

<span data-ttu-id="bc3f4-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc3f4-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="bc3f4-130">Remarks</span></span>

<span data-ttu-id="bc3f4-131">La configuration du service des règles de protection est constituée d’une liste de règles, de domaines internes et d’un intervalle d’actualisation.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="bc3f4-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc3f4-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc3f4-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bc3f4-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc3f4-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bc3f4-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bc3f4-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bc3f4-135">Schema Name</span></span>  <br/> |<span data-ttu-id="bc3f4-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bc3f4-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bc3f4-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bc3f4-137">Validation File</span></span>  <br/> |<span data-ttu-id="bc3f4-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc3f4-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc3f4-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bc3f4-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc3f4-140">False</span><span class="sxs-lookup"><span data-stu-id="bc3f4-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc3f4-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bc3f4-141">See also</span></span>



- [<span data-ttu-id="bc3f4-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bc3f4-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

