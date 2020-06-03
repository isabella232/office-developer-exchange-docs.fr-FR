---
title: DomainSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: L’élément DomainSettingsErrors contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés.
ms.openlocfilehash: 4e7ee29c2bc680a1938b75189c2ac3c214f7d2b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530704"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="cc673-103">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cc673-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="cc673-104">L’élément **DomainSettingsErrors** contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés.</span><span class="sxs-lookup"><span data-stu-id="cc673-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="cc673-105">**DomainSettingsErrors**</span><span class="sxs-lookup"><span data-stu-id="cc673-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc673-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cc673-106">Attributes and elements</span></span>

<span data-ttu-id="cc673-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cc673-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc673-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cc673-108">Attributes</span></span>

<span data-ttu-id="cc673-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cc673-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc673-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cc673-110">Child elements</span></span>

|<span data-ttu-id="cc673-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cc673-111">**Element**</span></span>|<span data-ttu-id="cc673-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cc673-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc673-113">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cc673-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="cc673-114">Représente une erreur qui s’est produite lors de la récupération d’un paramètre de domaine.</span><span class="sxs-lookup"><span data-stu-id="cc673-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="cc673-115">Cela représente une erreur à partir d’une demande d’opération [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="cc673-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc673-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cc673-116">Parent elements</span></span>

|<span data-ttu-id="cc673-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cc673-117">**Element**</span></span>|<span data-ttu-id="cc673-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="cc673-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc673-119">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cc673-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="cc673-120">Contient les paramètres demandés pour le domaine spécifié.</span><span class="sxs-lookup"><span data-stu-id="cc673-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cc673-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cc673-121">Text value</span></span>

<span data-ttu-id="cc673-122">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cc673-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc673-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cc673-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc673-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cc673-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cc673-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cc673-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cc673-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="cc673-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cc673-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cc673-127">Validation File</span></span>  <br/> |<span data-ttu-id="cc673-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cc673-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc673-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cc673-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc673-130">True</span><span class="sxs-lookup"><span data-stu-id="cc673-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc673-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cc673-131">See also</span></span>

- [<span data-ttu-id="cc673-132">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cc673-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

