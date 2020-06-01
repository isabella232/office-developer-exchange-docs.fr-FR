---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: L’élément RequestedVersion spécifie la version de service minimale sur laquelle le client souhaite que la demande soit traitée.
ms.openlocfilehash: ded276b3eb2c70b6edd39ca12289098de2b3faea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459166"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="5dda0-103">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5dda0-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="5dda0-104">L’élément **RequestedVersion** spécifie la version de service minimale sur laquelle le client souhaite que la demande soit traitée.</span><span class="sxs-lookup"><span data-stu-id="5dda0-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="5dda0-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="5dda0-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dda0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5dda0-106">Attributes and elements</span></span>

<span data-ttu-id="5dda0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5dda0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dda0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5dda0-108">Attributes</span></span>

<span data-ttu-id="5dda0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5dda0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dda0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5dda0-110">Child elements</span></span>

<span data-ttu-id="5dda0-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5dda0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5dda0-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5dda0-112">Parent elements</span></span>

|<span data-ttu-id="5dda0-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5dda0-113">**Element**</span></span>|<span data-ttu-id="5dda0-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5dda0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dda0-115">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5dda0-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="5dda0-116">Contient les paramètres de configuration demandés et les utilisateurs cibles.</span><span class="sxs-lookup"><span data-stu-id="5dda0-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="5dda0-117">Request (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5dda0-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="5dda0-118">Représente une demande d’obtention des paramètres de domaine.</span><span class="sxs-lookup"><span data-stu-id="5dda0-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5dda0-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5dda0-119">Text value</span></span>

<span data-ttu-id="5dda0-120">La valeur de texte de l’élément **RequestedVersion** peut être Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.</span><span class="sxs-lookup"><span data-stu-id="5dda0-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5dda0-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="5dda0-121">Remarks</span></span>

<span data-ttu-id="5dda0-122">Si cet élément n’est pas présent, la version de service la plus récente est utilisée.</span><span class="sxs-lookup"><span data-stu-id="5dda0-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5dda0-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5dda0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dda0-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5dda0-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5dda0-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5dda0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5dda0-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="5dda0-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5dda0-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5dda0-127">Validation File</span></span>  <br/> |<span data-ttu-id="5dda0-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5dda0-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5dda0-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5dda0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="5dda0-130">False</span><span class="sxs-lookup"><span data-stu-id="5dda0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5dda0-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5dda0-131">See also</span></span>



[<span data-ttu-id="5dda0-132">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5dda0-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="5dda0-133">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5dda0-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

