---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: L’élément DomainSetting contient les paramètres de domaine qui sont renvoyés par la demande d’opération SOAP (GetDomainSettings Operation).
ms.openlocfilehash: 54441dd7cfcf7372807a1e6bfd8ea5d26805bffc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526297"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="2927f-103">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2927f-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="2927f-104">L’élément **DomainSetting** contient les paramètres de domaine qui sont renvoyés par la demande d’opération [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="2927f-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="2927f-105">**DomainSetting**</span><span class="sxs-lookup"><span data-stu-id="2927f-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2927f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2927f-106">Attributes and elements</span></span>

<span data-ttu-id="2927f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2927f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2927f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2927f-108">Attributes</span></span>

<span data-ttu-id="2927f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2927f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2927f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2927f-110">Child elements</span></span>

|<span data-ttu-id="2927f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2927f-111">**Element**</span></span>|<span data-ttu-id="2927f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2927f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2927f-113">Nom (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2927f-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="2927f-114">Représente le nom d’un paramètre.</span><span class="sxs-lookup"><span data-stu-id="2927f-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2927f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2927f-115">Parent elements</span></span>

|<span data-ttu-id="2927f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2927f-116">**Element**</span></span>|<span data-ttu-id="2927f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2927f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2927f-118">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2927f-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="2927f-119">Représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="2927f-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2927f-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2927f-120">Text value</span></span>

<span data-ttu-id="2927f-121">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2927f-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2927f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2927f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2927f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2927f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2927f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2927f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2927f-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2927f-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2927f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2927f-126">Validation File</span></span>  <br/> |<span data-ttu-id="2927f-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2927f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2927f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2927f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2927f-129">True</span><span class="sxs-lookup"><span data-stu-id="2927f-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2927f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2927f-130">See also</span></span>

- [<span data-ttu-id="2927f-131">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2927f-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

