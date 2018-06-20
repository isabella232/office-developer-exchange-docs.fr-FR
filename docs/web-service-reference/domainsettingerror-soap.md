---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: L’élément DomainSettingError représente une erreur s’est produite lors de la récupération d’un paramètre du domaine. Cela représente une erreur à partir d’une demande GetDomainSettings.
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756042"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="2b745-104">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2b745-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="2b745-105">L’élément **DomainSettingError** représente une erreur s’est produite lors de la récupération d’un paramètre du domaine.</span><span class="sxs-lookup"><span data-stu-id="2b745-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="2b745-106">Cela représente une erreur à partir d’une demande **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="2b745-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="2b745-107">**DomainSettingError**</span><span class="sxs-lookup"><span data-stu-id="2b745-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b745-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2b745-108">Attributes and elements</span></span>

<span data-ttu-id="2b745-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2b745-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b745-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2b745-110">Attributes</span></span>

<span data-ttu-id="2b745-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b745-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b745-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2b745-112">Child elements</span></span>

|<span data-ttu-id="2b745-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b745-113">**Element**</span></span>|<span data-ttu-id="2b745-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b745-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b745-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2b745-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="2b745-116">Identifie le code d’erreur qui est associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="2b745-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="2b745-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2b745-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="2b745-118">Contient le message d’erreur qui est associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="2b745-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="2b745-119">Nom du paramètre (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2b745-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="2b745-120">Représente le nom du paramètre.</span><span class="sxs-lookup"><span data-stu-id="2b745-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b745-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2b745-121">Parent elements</span></span>

|<span data-ttu-id="2b745-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b745-122">**Element**</span></span>|<span data-ttu-id="2b745-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b745-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b745-124">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2b745-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="2b745-125">Contient des informations d’erreur pour les paramètres qui ne peut pas être retourné.</span><span class="sxs-lookup"><span data-stu-id="2b745-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b745-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2b745-126">Text value</span></span>

<span data-ttu-id="2b745-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b745-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b745-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2b745-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b745-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2b745-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2b745-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2b745-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2b745-131">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2b745-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2b745-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2b745-132">Validation File</span></span>  <br/> |<span data-ttu-id="2b745-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2b745-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2b745-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2b745-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b745-135">True</span><span class="sxs-lookup"><span data-stu-id="2b745-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b745-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2b745-136">See also</span></span>

- [<span data-ttu-id="2b745-137">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2b745-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

