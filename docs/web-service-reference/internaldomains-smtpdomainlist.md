---
title: InternalDomains (SmtpDomainList)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalDomains
api_type:
- schema
ms.assetid: 0f2cbb05-338d-4302-8871-a06e78b33f98
description: L’élément InternalDomains identifie la liste des domaines SMTP internes de votre organisation.
ms.openlocfilehash: f37a31f4348a7eb0024656489f249dec349bc67b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827953"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="1c621-103">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="1c621-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="1c621-104">L’élément **InternalDomains** identifie la liste des domaines SMTP internes de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="1c621-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="1c621-105">**SmtpDomainList**</span><span class="sxs-lookup"><span data-stu-id="1c621-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c621-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1c621-106">Attributes and elements</span></span>

<span data-ttu-id="1c621-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1c621-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c621-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1c621-108">Attributes</span></span>

<span data-ttu-id="1c621-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1c621-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c621-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1c621-110">Child elements</span></span>

|<span data-ttu-id="1c621-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c621-111">**Element**</span></span>|<span data-ttu-id="1c621-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c621-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c621-113">Domain</span><span class="sxs-lookup"><span data-stu-id="1c621-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="1c621-114">Identifie un domaine SMTP unique.</span><span class="sxs-lookup"><span data-stu-id="1c621-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c621-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1c621-115">Parent elements</span></span>

|<span data-ttu-id="1c621-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c621-116">**Element**</span></span>|<span data-ttu-id="1c621-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c621-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c621-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="1c621-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="1c621-119">Contient des informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="1c621-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="1c621-120">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c621-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="1c621-121">Contient des informations de configuration de service pour le service de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="1c621-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1c621-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1c621-122">Text value</span></span>

<span data-ttu-id="1c621-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1c621-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1c621-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="1c621-124">Remarks</span></span>

<span data-ttu-id="1c621-125">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="1c621-125">This element is required.</span></span> 
  
<span data-ttu-id="1c621-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c621-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c621-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1c621-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c621-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1c621-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c621-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1c621-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1c621-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1c621-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="1c621-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1c621-131">Validation File</span></span>  <br/> |<span data-ttu-id="1c621-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1c621-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c621-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1c621-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c621-134">False</span><span class="sxs-lookup"><span data-stu-id="1c621-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c621-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1c621-135">See also</span></span>



- [<span data-ttu-id="1c621-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1c621-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

