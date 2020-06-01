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
description: L’élément InternalDomains identifie la liste des domaines SMTP internes de l’organisation.
ms.openlocfilehash: ec7ef2d72ae922c751f8f50b72ff7d6b31b212ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459965"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="44401-103">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="44401-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="44401-104">L’élément **InternalDomains** identifie la liste des domaines SMTP internes de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="44401-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="44401-105">**SmtpDomainList**</span><span class="sxs-lookup"><span data-stu-id="44401-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44401-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="44401-106">Attributes and elements</span></span>

<span data-ttu-id="44401-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="44401-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44401-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="44401-108">Attributes</span></span>

<span data-ttu-id="44401-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="44401-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44401-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="44401-110">Child elements</span></span>

|<span data-ttu-id="44401-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="44401-111">**Element**</span></span>|<span data-ttu-id="44401-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="44401-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44401-113">Domaine</span><span class="sxs-lookup"><span data-stu-id="44401-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="44401-114">Identifie un domaine SMTP unique.</span><span class="sxs-lookup"><span data-stu-id="44401-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44401-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="44401-115">Parent elements</span></span>

|<span data-ttu-id="44401-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="44401-116">**Element**</span></span>|<span data-ttu-id="44401-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="44401-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44401-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="44401-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="44401-119">Contient les informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="44401-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="44401-120">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="44401-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="44401-121">Contient des informations de configuration de service pour le service de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="44401-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="44401-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="44401-122">Text value</span></span>

<span data-ttu-id="44401-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="44401-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="44401-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="44401-124">Remarks</span></span>

<span data-ttu-id="44401-125">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="44401-125">This element is required.</span></span> 
  
<span data-ttu-id="44401-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="44401-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44401-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="44401-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44401-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="44401-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44401-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="44401-129">Schema Name</span></span>  <br/> |<span data-ttu-id="44401-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="44401-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="44401-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="44401-131">Validation File</span></span>  <br/> |<span data-ttu-id="44401-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="44401-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44401-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="44401-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="44401-134">False</span><span class="sxs-lookup"><span data-stu-id="44401-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44401-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="44401-135">See also</span></span>



- [<span data-ttu-id="44401-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="44401-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

