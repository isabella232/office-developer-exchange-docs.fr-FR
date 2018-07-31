---
title: UserConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: L’élément UserConfigurationName représente le nom d’un objet de configuration utilisateur. Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur.
ms.openlocfilehash: 33b3fc316a06b8088eb20a71788a9e6a3394d0d4
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354301"
---
# <a name="userconfigurationname"></a><span data-ttu-id="de4c3-104">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="de4c3-104">UserConfigurationName</span></span>

<span data-ttu-id="de4c3-105">L’élément **UserConfigurationName** représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de4c3-105">The **UserConfigurationName** element represents the name of a user configuration object.</span></span> <span data-ttu-id="de4c3-106">Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de4c3-106">The user configuration object name is the identifier for a user configuration object.</span></span> 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

<span data-ttu-id="de4c3-107">**UserConfigurationNameType**</span><span class="sxs-lookup"><span data-stu-id="de4c3-107">**UserConfigurationNameType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="de4c3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de4c3-108">Attributes and elements</span></span>

<span data-ttu-id="de4c3-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de4c3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de4c3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="de4c3-110">Attributes</span></span>

|<span data-ttu-id="de4c3-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="de4c3-111">**Attribute**</span></span>|<span data-ttu-id="de4c3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="de4c3-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="de4c3-113">**Name**</span><span class="sxs-lookup"><span data-stu-id="de4c3-113">**Name**</span></span> <br/> |<span data-ttu-id="de4c3-114">Contient une valeur de type string qui représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de4c3-114">Contains a string value that represents the name of a user configuration object.</span></span> <span data-ttu-id="de4c3-115">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="de4c3-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="de4c3-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de4c3-116">Child elements</span></span>

|<span data-ttu-id="de4c3-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de4c3-117">**Element**</span></span>|<span data-ttu-id="de4c3-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="de4c3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de4c3-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="de4c3-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="de4c3-120">Représente l’identificateur de dossier du dossier qui contient l’objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de4c3-120">Represents the folder identifier of the folder that contains the user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="de4c3-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="de4c3-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="de4c3-122">Représente un nom de dossier unique du dossier qui contient l’objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de4c3-122">Represents a distinguished folder name of the folder that contains the user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de4c3-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de4c3-123">Parent elements</span></span>

|<span data-ttu-id="de4c3-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de4c3-124">**Element**</span></span>|<span data-ttu-id="de4c3-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="de4c3-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de4c3-126">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="de4c3-126">DeleteUserConfiguration</span></span>](deleteuserconfiguration.md) <br/> |<span data-ttu-id="de4c3-127">Représente une demande pour supprimer un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de4c3-127">Represents a request to delete a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="de4c3-128">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="de4c3-128">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="de4c3-129">Représente une demande pour obtenir un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="de4c3-129">Represents a request to get a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="de4c3-130">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="de4c3-130">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="de4c3-131">Définit un objet de configuration utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="de4c3-131">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="de4c3-132">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="de4c3-132">Text value</span></span>

<span data-ttu-id="de4c3-133">Aucun.</span><span class="sxs-lookup"><span data-stu-id="de4c3-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de4c3-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="de4c3-134">Remarks</span></span>

<span data-ttu-id="de4c3-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="de4c3-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de4c3-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de4c3-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de4c3-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de4c3-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de4c3-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de4c3-138">Schema Name</span></span>  <br/> |<span data-ttu-id="de4c3-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="de4c3-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="de4c3-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de4c3-140">Validation File</span></span>  <br/> |<span data-ttu-id="de4c3-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="de4c3-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de4c3-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de4c3-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="de4c3-143">False</span><span class="sxs-lookup"><span data-stu-id="de4c3-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de4c3-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="de4c3-144">See also</span></span>

- [<span data-ttu-id="de4c3-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="de4c3-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

