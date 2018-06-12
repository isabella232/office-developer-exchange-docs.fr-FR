---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: L’élément TasksFolderPermissionLevel contient les autorisations pour le dossier tâches par défaut. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838673"
---
# <a name="tasksfolderpermissionlevel"></a><span data-ttu-id="9ab9b-104">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="9ab9b-104">TasksFolderPermissionLevel</span></span>

<span data-ttu-id="9ab9b-105">L’élément **TasksFolderPermissionLevel** contient les autorisations pour le dossier tâches par défaut.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-105">The **TasksFolderPermissionLevel** element contains the permissions for the default Tasks folder.</span></span> <span data-ttu-id="9ab9b-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9ab9b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

<span data-ttu-id="9ab9b-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="9ab9b-107">**DelegateFolderPermissionLevelType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9ab9b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9ab9b-108">Attributes and elements</span></span>

<span data-ttu-id="9ab9b-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ab9b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="9ab9b-110">Attributes</span></span>

<span data-ttu-id="9ab9b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ab9b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9ab9b-112">Child elements</span></span>

<span data-ttu-id="9ab9b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9ab9b-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9ab9b-114">Parent elements</span></span>

|<span data-ttu-id="9ab9b-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9ab9b-115">**Element**</span></span>|<span data-ttu-id="9ab9b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ab9b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ab9b-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="9ab9b-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="9ab9b-118">Contient les paramètres au niveau d’autorisation délégué pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="9ab9b-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ab9b-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9ab9b-120">Text value</span></span>

<span data-ttu-id="9ab9b-121">Le tableau suivant répertorie les valeurs de texte qui représentent les niveaux d’autorisation.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="9ab9b-122">**Valeurs de texte de niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="9ab9b-122">**Permission level text values**</span></span>

|<span data-ttu-id="9ab9b-123">**Niveau d’autorisation**</span><span class="sxs-lookup"><span data-stu-id="9ab9b-123">**Permission level**</span></span>|<span data-ttu-id="9ab9b-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ab9b-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ab9b-125">None</span><span class="sxs-lookup"><span data-stu-id="9ab9b-125">None</span></span>  <br/> |<span data-ttu-id="9ab9b-126">L’utilisateur délégué a des autorisations d’accès au dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-126">The delegate user has no access permissions to the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="9ab9b-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="9ab9b-127">Reviewer</span></span>  <br/> |<span data-ttu-id="9ab9b-128">L’utilisateur délégué peut lire des éléments dans le dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-128">The delegate user can read items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="9ab9b-129">Auteur</span><span class="sxs-lookup"><span data-stu-id="9ab9b-129">Author</span></span>  <br/> |<span data-ttu-id="9ab9b-130">L’utilisateur délégué pouvant lire et créer des éléments dans le dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-130">The delegate user can read and create items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="9ab9b-131">Editor</span><span class="sxs-lookup"><span data-stu-id="9ab9b-131">Editor</span></span>  <br/> |<span data-ttu-id="9ab9b-132">L’utilisateur délégué peut lire, créer et modifier des éléments dans le dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-132">The delegate user can read, create, and modify items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="9ab9b-133">Personnalisé</span><span class="sxs-lookup"><span data-stu-id="9ab9b-133">Custom</span></span>  <br/> |<span data-ttu-id="9ab9b-134">L’utilisateur délégué dispose des autorisations d’accès personnalisé au dossier tâches.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-134">The delegate user has custom access permissions to the Tasks folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ab9b-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="9ab9b-135">Remarks</span></span>

<span data-ttu-id="9ab9b-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9ab9b-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ab9b-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9ab9b-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ab9b-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9ab9b-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ab9b-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9ab9b-139">Schema Name</span></span>  <br/> |<span data-ttu-id="9ab9b-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9ab9b-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ab9b-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9ab9b-141">Validation File</span></span>  <br/> |<span data-ttu-id="9ab9b-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ab9b-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ab9b-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9ab9b-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ab9b-144">False</span><span class="sxs-lookup"><span data-stu-id="9ab9b-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ab9b-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9ab9b-145">See also</span></span>

- [<span data-ttu-id="9ab9b-146">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="9ab9b-146">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="9ab9b-147">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="9ab9b-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="9ab9b-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9ab9b-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="9ab9b-149">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="9ab9b-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)
