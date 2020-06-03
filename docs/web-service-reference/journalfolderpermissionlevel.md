---
title: JournalFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- JournalFolderPermissionLevel
api_type:
- schema
ms.assetid: 564525fa-cd95-4c1a-9d6c-3806be664579
description: L’élément JournalFolderPermissionLevel contient les autorisations pour le dossier journal par défaut. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 5c0f30932eb3fbbeef1a8e34611deeb1ffef402c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529048"
---
# <a name="journalfolderpermissionlevel"></a><span data-ttu-id="32557-104">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="32557-104">JournalFolderPermissionLevel</span></span>

<span data-ttu-id="32557-105">L’élément **JournalFolderPermissionLevel** contient les autorisations pour le dossier journal par défaut.</span><span class="sxs-lookup"><span data-stu-id="32557-105">The **JournalFolderPermissionLevel** element contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="32557-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="32557-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<JournalFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</JournalFolderPermissionLevel>
```

 <span data-ttu-id="32557-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="32557-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32557-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="32557-108">Attributes and elements</span></span>

<span data-ttu-id="32557-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="32557-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32557-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="32557-110">Attributes</span></span>

<span data-ttu-id="32557-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="32557-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32557-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="32557-112">Child elements</span></span>

<span data-ttu-id="32557-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="32557-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32557-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="32557-114">Parent elements</span></span>

|<span data-ttu-id="32557-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="32557-115">**Element**</span></span>|<span data-ttu-id="32557-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="32557-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32557-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="32557-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="32557-118">Contient les paramètres de niveau d’autorisation de délégué pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="32557-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="32557-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="32557-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32557-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="32557-120">Text value</span></span>

<span data-ttu-id="32557-121">Le tableau suivant répertorie les valeurs de texte qui représentent les niveaux d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="32557-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="32557-122">**Valeurs de texte de niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="32557-122">**Permission level text values**</span></span>

|<span data-ttu-id="32557-123">**Niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="32557-123">**Permission level**</span></span>|<span data-ttu-id="32557-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="32557-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32557-125">Aucun</span><span class="sxs-lookup"><span data-stu-id="32557-125">None</span></span>  <br/> |<span data-ttu-id="32557-126">L’utilisateur délégué ne dispose pas d’autorisations d’accès au dossier journal.</span><span class="sxs-lookup"><span data-stu-id="32557-126">The delegate user has no access permissions to the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="32557-127">Relecteur</span><span class="sxs-lookup"><span data-stu-id="32557-127">Reviewer</span></span>  <br/> |<span data-ttu-id="32557-128">L’utilisateur délégué peut lire les éléments dans le dossier journal.</span><span class="sxs-lookup"><span data-stu-id="32557-128">The delegate user can read items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="32557-129">Auteur</span><span class="sxs-lookup"><span data-stu-id="32557-129">Author</span></span>  <br/> |<span data-ttu-id="32557-130">L’utilisateur délégué peut lire et créer des éléments dans le dossier journal.</span><span class="sxs-lookup"><span data-stu-id="32557-130">The delegate user can read and create items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="32557-131">Éditeur</span><span class="sxs-lookup"><span data-stu-id="32557-131">Editor</span></span>  <br/> |<span data-ttu-id="32557-132">L’utilisateur délégué peut lire, créer et modifier des éléments dans le dossier journal.</span><span class="sxs-lookup"><span data-stu-id="32557-132">The delegate user can read, create, and modify items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="32557-133">Personnalisé</span><span class="sxs-lookup"><span data-stu-id="32557-133">Custom</span></span>  <br/> |<span data-ttu-id="32557-134">L’utilisateur délégué dispose d’autorisations d’accès personnalisées au dossier journal.</span><span class="sxs-lookup"><span data-stu-id="32557-134">The delegate user has custom access permissions to the Journal folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="32557-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="32557-135">Remarks</span></span>

<span data-ttu-id="32557-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="32557-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32557-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="32557-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32557-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="32557-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32557-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="32557-139">Schema Name</span></span>  <br/> |<span data-ttu-id="32557-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="32557-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="32557-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="32557-141">Validation File</span></span>  <br/> |<span data-ttu-id="32557-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32557-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32557-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="32557-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="32557-144">False</span><span class="sxs-lookup"><span data-stu-id="32557-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32557-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="32557-145">See also</span></span>



[<span data-ttu-id="32557-146">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="32557-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="32557-147">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="32557-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="32557-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="32557-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="32557-149">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="32557-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

