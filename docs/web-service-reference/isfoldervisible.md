---
title: IsFolderVisible
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderVisible
api_type:
- schema
ms.assetid: dd611fb5-9424-4ff9-bb27-c882c73c0c74
description: L’élément IsFolderVisible indique si un utilisateur peut afficher un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 27a6bca9ae71bc93de6c22cb87c8d582025144e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828019"
---
# <a name="isfoldervisible"></a><span data-ttu-id="fbcdf-104">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="fbcdf-104">IsFolderVisible</span></span>

<span data-ttu-id="fbcdf-105">L’élément **IsFolderVisible** indique si un utilisateur peut afficher un dossier.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-105">The **IsFolderVisible** element indicates whether a user can view a folder.</span></span> <span data-ttu-id="fbcdf-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fbcdf-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderVisible/>
```

 <span data-ttu-id="fbcdf-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fbcdf-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbcdf-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fbcdf-108">Attributes and elements</span></span>

<span data-ttu-id="fbcdf-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbcdf-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="fbcdf-110">Attributes</span></span>

<span data-ttu-id="fbcdf-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbcdf-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fbcdf-112">Child elements</span></span>

<span data-ttu-id="fbcdf-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fbcdf-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fbcdf-114">Parent elements</span></span>

|<span data-ttu-id="fbcdf-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fbcdf-115">**Element**</span></span>|<span data-ttu-id="fbcdf-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="fbcdf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbcdf-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="fbcdf-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="fbcdf-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="fbcdf-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="fbcdf-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="fbcdf-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fbcdf-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fbcdf-123">Text value</span></span>

<span data-ttu-id="fbcdf-124">Une valeur de texte de **la valeur true** indique que l’utilisateur peut afficher le dossier.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-124">A text value of **true** indicates that the user can view the folder.</span></span> <span data-ttu-id="fbcdf-125">La valeur **false** indique que l’utilisateur ne peut pas afficher le dossier.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-125">A value of **false** indicates that the user cannot view the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fbcdf-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="fbcdf-126">Remarks</span></span>

<span data-ttu-id="fbcdf-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fbcdf-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbcdf-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fbcdf-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbcdf-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fbcdf-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fbcdf-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fbcdf-130">Schema Name</span></span>  <br/> |<span data-ttu-id="fbcdf-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fbcdf-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="fbcdf-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fbcdf-132">Validation File</span></span>  <br/> |<span data-ttu-id="fbcdf-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fbcdf-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fbcdf-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fbcdf-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="fbcdf-135">False</span><span class="sxs-lookup"><span data-stu-id="fbcdf-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fbcdf-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fbcdf-136">See also</span></span>



- [<span data-ttu-id="fbcdf-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fbcdf-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fbcdf-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="fbcdf-138">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

