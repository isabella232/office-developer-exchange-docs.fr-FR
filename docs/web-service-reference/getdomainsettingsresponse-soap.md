---
title: GetDomainSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: L’élément GetDomainSettingsResponse représente la réponse à une opération GetDomainSettings (SOAP), qui renvoie les paramètres de domaine.
ms.openlocfilehash: 94cb202948e6a0d5a34f5547132c052d1d1b6a40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461876"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="f1b10-103">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1b10-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="f1b10-104">L’élément **GetDomainSettingsResponse** représente la réponse à une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), qui renvoie les paramètres de domaine.</span><span class="sxs-lookup"><span data-stu-id="f1b10-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="f1b10-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="f1b10-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1b10-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1b10-106">Attributes and elements</span></span>

<span data-ttu-id="f1b10-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1b10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1b10-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1b10-108">Attributes</span></span>

<span data-ttu-id="f1b10-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f1b10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1b10-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1b10-110">Child elements</span></span>

|<span data-ttu-id="f1b10-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1b10-111">**Element**</span></span>|<span data-ttu-id="f1b10-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1b10-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1b10-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1b10-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="f1b10-114">Contient un tableau de réponses pour les paramètres de chaque domaine demandé.</span><span class="sxs-lookup"><span data-stu-id="f1b10-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="f1b10-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1b10-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="f1b10-116">Représente un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f1b10-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f1b10-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1b10-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="f1b10-118">Représente un message associé à un code d’erreur renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="f1b10-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1b10-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1b10-119">Parent elements</span></span>

<span data-ttu-id="f1b10-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f1b10-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f1b10-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f1b10-121">Text value</span></span>

<span data-ttu-id="f1b10-122">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f1b10-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1b10-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f1b10-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1b10-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f1b10-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f1b10-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f1b10-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f1b10-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="f1b10-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f1b10-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f1b10-127">Validation File</span></span>  <br/> |<span data-ttu-id="f1b10-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f1b10-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1b10-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f1b10-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1b10-130">True</span><span class="sxs-lookup"><span data-stu-id="f1b10-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1b10-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1b10-131">See also</span></span>



[<span data-ttu-id="f1b10-132">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f1b10-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

