---
title: CanCreateSubFolders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateSubFolders
api_type:
- schema
ms.assetid: 4404a1cc-6d3f-4996-9647-58a740e8f883
description: L'élément CanCreateSubFolders indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d8e89c7a07ef1788717f5012840f5b8f79d319e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461596"
---
# <a name="cancreatesubfolders"></a><span data-ttu-id="01fb9-104">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="01fb9-104">CanCreateSubFolders</span></span>

<span data-ttu-id="01fb9-p102">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **CanCreateSubFolders** indique si un utilisateur est autorisé à créer des sous-dossiers dans un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="01fb9-p102">The **CanCreateSubFolders** element indicates whether a user has permission to create subfolders in a folder. This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateSubFolders/>
```

 <span data-ttu-id="01fb9-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="01fb9-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01fb9-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="01fb9-108">Attributes and elements</span></span>

<span data-ttu-id="01fb9-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="01fb9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01fb9-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="01fb9-110">Attributes</span></span>

<span data-ttu-id="01fb9-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="01fb9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01fb9-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="01fb9-112">Child elements</span></span>

<span data-ttu-id="01fb9-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="01fb9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01fb9-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="01fb9-114">Parent elements</span></span>

|<span data-ttu-id="01fb9-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="01fb9-115">**Element**</span></span>|<span data-ttu-id="01fb9-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="01fb9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01fb9-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="01fb9-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="01fb9-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="01fb9-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="01fb9-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="01fb9-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="01fb9-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="01fb9-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01fb9-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="01fb9-123">Text value</span></span>

<span data-ttu-id="01fb9-p105">Une valeur texte **true** indique que l'utilisateur peut créer des sous-dossiers dans le dossier. La valeur **false** indique que l'utilisateur ne peut pas créer des sous-dossiers dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="01fb9-p105">A text value of **true** indicates that the user can create subfolders in the folder. A value of **false** indicates that the user cannot create subfolders in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="01fb9-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="01fb9-126">Remarks</span></span>

<span data-ttu-id="01fb9-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="01fb9-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01fb9-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="01fb9-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01fb9-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="01fb9-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01fb9-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="01fb9-130">Schema Name</span></span>  <br/> |<span data-ttu-id="01fb9-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="01fb9-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="01fb9-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="01fb9-132">Validation File</span></span>  <br/> |<span data-ttu-id="01fb9-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01fb9-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01fb9-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="01fb9-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="01fb9-135">False</span><span class="sxs-lookup"><span data-stu-id="01fb9-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01fb9-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="01fb9-136">See also</span></span>



- [<span data-ttu-id="01fb9-137">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="01fb9-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="01fb9-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="01fb9-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

