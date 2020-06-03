---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: L’élément GetDomainSettingsRequest représente une demande d’opération SOAP (GetDomainSettings Operation).
ms.openlocfilehash: 400016d0817131fb70ec7ff3db7fbfdc1b51f8f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460959"
---
# <a name="getdomainsettingsrequest-soap"></a><span data-ttu-id="7b0dc-103">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7b0dc-103">GetDomainSettingsRequest (SOAP)</span></span>

<span data-ttu-id="7b0dc-104">L’élément **GetDomainSettingsRequest** représente une demande d’opération [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="7b0dc-104">The **GetDomainSettingsRequest** element represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 <span data-ttu-id="7b0dc-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="7b0dc-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b0dc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b0dc-106">Attributes and elements</span></span>

<span data-ttu-id="7b0dc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b0dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b0dc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b0dc-108">Attributes</span></span>

<span data-ttu-id="7b0dc-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b0dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b0dc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b0dc-110">Child elements</span></span>

|<span data-ttu-id="7b0dc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b0dc-111">**Element**</span></span>|<span data-ttu-id="7b0dc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b0dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b0dc-113">Domaines (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7b0dc-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="7b0dc-114">Représente une collection d’identificateurs de domaine.</span><span class="sxs-lookup"><span data-stu-id="7b0dc-114">Represents a collection of domain identifiers.</span></span>  <br/> |
|[<span data-ttu-id="7b0dc-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7b0dc-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="7b0dc-116">Contient les noms des paramètres de configuration de domaine demandés.</span><span class="sxs-lookup"><span data-stu-id="7b0dc-116">Contains the names of the requested domain configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="7b0dc-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7b0dc-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="7b0dc-118">Spécifie la version du serveur que le fournisseur doit utiliser.</span><span class="sxs-lookup"><span data-stu-id="7b0dc-118">Specifies the server version that the provider will use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b0dc-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b0dc-119">Parent elements</span></span>

<span data-ttu-id="7b0dc-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7b0dc-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7b0dc-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7b0dc-121">Text value</span></span>

<span data-ttu-id="7b0dc-122">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b0dc-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b0dc-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b0dc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b0dc-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b0dc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7b0dc-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b0dc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7b0dc-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="7b0dc-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7b0dc-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7b0dc-127">Validation File</span></span>  <br/> |<span data-ttu-id="7b0dc-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7b0dc-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7b0dc-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b0dc-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b0dc-130">True</span><span class="sxs-lookup"><span data-stu-id="7b0dc-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b0dc-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b0dc-131">See also</span></span>



[<span data-ttu-id="7b0dc-132">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7b0dc-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

