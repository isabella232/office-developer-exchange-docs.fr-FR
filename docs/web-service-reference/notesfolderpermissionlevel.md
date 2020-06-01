---
title: NotesFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotesFolderPermissionLevel
api_type:
- schema
ms.assetid: 76a2520c-f453-4fd7-b3eb-1c5f4666680a
description: L’élément NotesFolderPermissionLevel contient les autorisations pour le dossier Notes par défaut. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 205802592a1fc01451b4fc497e9e0c4c66afd478
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462625"
---
# <a name="notesfolderpermissionlevel"></a><span data-ttu-id="6bcbb-104">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="6bcbb-104">NotesFolderPermissionLevel</span></span>

<span data-ttu-id="6bcbb-105">L’élément **NotesFolderPermissionLevel** contient les autorisations pour le dossier Notes par défaut.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-105">The **NotesFolderPermissionLevel** element contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="6bcbb-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6bcbb-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<NotesFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</NotesFolderPermissionLevel>
```

 <span data-ttu-id="6bcbb-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="6bcbb-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6bcbb-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6bcbb-108">Attributes and elements</span></span>

<span data-ttu-id="6bcbb-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bcbb-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="6bcbb-110">Attributes</span></span>

<span data-ttu-id="6bcbb-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bcbb-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6bcbb-112">Child elements</span></span>

<span data-ttu-id="6bcbb-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bcbb-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6bcbb-114">Parent elements</span></span>

|<span data-ttu-id="6bcbb-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6bcbb-115">**Element**</span></span>|<span data-ttu-id="6bcbb-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="6bcbb-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bcbb-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="6bcbb-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="6bcbb-118">Contient les paramètres de niveau d’autorisation de délégué pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="6bcbb-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bcbb-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6bcbb-120">Text value</span></span>

<span data-ttu-id="6bcbb-121">Le tableau suivant répertorie les valeurs de texte qui représentent les niveaux d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="6bcbb-122">**Valeurs de texte de niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="6bcbb-122">**Permission level text values**</span></span>

|<span data-ttu-id="6bcbb-123">**Niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="6bcbb-123">**Permission level**</span></span>|<span data-ttu-id="6bcbb-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="6bcbb-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6bcbb-125">Aucun</span><span class="sxs-lookup"><span data-stu-id="6bcbb-125">None</span></span>  <br/> |<span data-ttu-id="6bcbb-126">L’utilisateur délégué ne dispose pas des autorisations d’accès au dossier Notes.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-126">The delegate user has no access permissions to the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="6bcbb-127">Relecteur</span><span class="sxs-lookup"><span data-stu-id="6bcbb-127">Reviewer</span></span>  <br/> |<span data-ttu-id="6bcbb-128">L’utilisateur délégué peut lire les éléments dans le dossier Notes.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-128">The delegate user can read items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="6bcbb-129">Auteur</span><span class="sxs-lookup"><span data-stu-id="6bcbb-129">Author</span></span>  <br/> |<span data-ttu-id="6bcbb-130">L’utilisateur délégué peut lire et créer des éléments dans le dossier Notes.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-130">The delegate user can read and create items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="6bcbb-131">Éditeur</span><span class="sxs-lookup"><span data-stu-id="6bcbb-131">Editor</span></span>  <br/> |<span data-ttu-id="6bcbb-132">L’utilisateur délégué peut lire, créer et modifier des éléments dans le dossier Notes.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-132">The delegate user can read, create, and modify items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="6bcbb-133">Personnalisé</span><span class="sxs-lookup"><span data-stu-id="6bcbb-133">Custom</span></span>  <br/> |<span data-ttu-id="6bcbb-134">L’utilisateur délégué dispose d’autorisations d’accès personnalisées au dossier Notes.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-134">The delegate user has custom access permissions to the Notes folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6bcbb-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="6bcbb-135">Remarks</span></span>

<span data-ttu-id="6bcbb-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6bcbb-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bcbb-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6bcbb-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bcbb-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6bcbb-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6bcbb-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6bcbb-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6bcbb-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6bcbb-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="6bcbb-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6bcbb-141">Validation File</span></span>  <br/> |<span data-ttu-id="6bcbb-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6bcbb-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6bcbb-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6bcbb-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6bcbb-144">False</span><span class="sxs-lookup"><span data-stu-id="6bcbb-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bcbb-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6bcbb-145">See also</span></span>



[<span data-ttu-id="6bcbb-146">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="6bcbb-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="6bcbb-147">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="6bcbb-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="6bcbb-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6bcbb-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6bcbb-149">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="6bcbb-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

