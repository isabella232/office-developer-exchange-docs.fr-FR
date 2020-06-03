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
description: L’élément DomainSettingError représente une erreur qui s’est produite lors de la récupération d’un paramètre de domaine. Cela représente une erreur à partir d’une demande GetDomainSettings.
ms.openlocfilehash: 189a614e7629033c8db2f60b8fd3679835a696ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530711"
---
# <a name="domainsettingerror-soap"></a><span data-ttu-id="4a031-104">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a031-104">DomainSettingError (SOAP)</span></span>

<span data-ttu-id="4a031-105">L’élément **DomainSettingError** représente une erreur qui s’est produite lors de la récupération d’un paramètre de domaine.</span><span class="sxs-lookup"><span data-stu-id="4a031-105">The **DomainSettingError** element represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="4a031-106">Cela représente une erreur à partir d’une demande **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="4a031-106">This represents an error from a **GetDomainSettings** request.</span></span> 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 <span data-ttu-id="4a031-107">**DomainSettingError**</span><span class="sxs-lookup"><span data-stu-id="4a031-107">**DomainSettingError**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a031-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a031-108">Attributes and elements</span></span>

<span data-ttu-id="4a031-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a031-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a031-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a031-110">Attributes</span></span>

<span data-ttu-id="4a031-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4a031-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a031-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a031-112">Child elements</span></span>

|<span data-ttu-id="4a031-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a031-113">**Element**</span></span>|<span data-ttu-id="4a031-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a031-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a031-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a031-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="4a031-116">Identifie le code d’erreur associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="4a031-116">Identifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="4a031-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a031-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="4a031-118">Contient le message d’erreur associé à la demande spécifique.</span><span class="sxs-lookup"><span data-stu-id="4a031-118">Contains the error message that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="4a031-119">Propriétés SettingName (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a031-119">SettingName (SOAP)</span></span>](settingname-soap.md) <br/> |<span data-ttu-id="4a031-120">Représente le nom du paramètre.</span><span class="sxs-lookup"><span data-stu-id="4a031-120">Represents the name of the setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a031-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a031-121">Parent elements</span></span>

|<span data-ttu-id="4a031-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a031-122">**Element**</span></span>|<span data-ttu-id="4a031-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a031-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a031-124">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a031-124">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="4a031-125">Contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés.</span><span class="sxs-lookup"><span data-stu-id="4a031-125">Contains error information for settings that could not be returned.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a031-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4a031-126">Text value</span></span>

<span data-ttu-id="4a031-127">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4a031-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a031-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a031-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a031-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a031-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4a031-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a031-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4a031-131">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="4a031-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4a031-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a031-132">Validation File</span></span>  <br/> |<span data-ttu-id="4a031-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4a031-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a031-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a031-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a031-135">True</span><span class="sxs-lookup"><span data-stu-id="4a031-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a031-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a031-136">See also</span></span>

- [<span data-ttu-id="4a031-137">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4a031-137">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

