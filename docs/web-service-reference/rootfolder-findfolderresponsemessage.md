---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: L’élément RootFolder contient les résultats d’une recherche d’un dossier racine unique lors d’une opération FindFolder.
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829253"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="362c6-103">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="362c6-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="362c6-104">L’élément **RootFolder** contient les résultats d’une recherche d’un dossier racine unique lors d’une [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="362c6-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="362c6-105">**FindFolderParentType**</span><span class="sxs-lookup"><span data-stu-id="362c6-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="362c6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="362c6-106">Attributes and elements</span></span>

<span data-ttu-id="362c6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="362c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="362c6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="362c6-108">Attributes</span></span>

|<span data-ttu-id="362c6-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="362c6-109">**Attribute**</span></span>|<span data-ttu-id="362c6-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="362c6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="362c6-111">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="362c6-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="362c6-112">Représente l’index suivant doit être utilisé pour la requête suivante lors de l’utilisation d’une vue indexée de pagination.</span><span class="sxs-lookup"><span data-stu-id="362c6-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="362c6-113">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="362c6-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="362c6-114">Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lors de l’utilisation des affichages de page en fraction.</span><span class="sxs-lookup"><span data-stu-id="362c6-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="362c6-115">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="362c6-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="362c6-116">Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination en fraction.</span><span class="sxs-lookup"><span data-stu-id="362c6-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="362c6-117">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="362c6-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="362c6-118">Indique si les résultats actuels de contient le dernier dossier dans la requête, telles que davantage de pagination n’est pas nécessaire.</span><span class="sxs-lookup"><span data-stu-id="362c6-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="362c6-119">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="362c6-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="362c6-120">Représente le nombre total de dossiers qui transmet la restriction.</span><span class="sxs-lookup"><span data-stu-id="362c6-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="362c6-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="362c6-121">Child elements</span></span>

|<span data-ttu-id="362c6-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="362c6-122">**Element**</span></span>|<span data-ttu-id="362c6-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="362c6-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="362c6-124">Dossiers</span><span class="sxs-lookup"><span data-stu-id="362c6-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="362c6-125">Contient un tableau des dossiers qui que se trouve à l’aide de l' [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="362c6-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="362c6-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="362c6-126">Parent elements</span></span>

|<span data-ttu-id="362c6-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="362c6-127">**Element**</span></span>|<span data-ttu-id="362c6-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="362c6-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="362c6-129">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="362c6-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="362c6-130">Contient l’état et les résultats d’une demande [d’opération FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="362c6-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="362c6-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="362c6-131">Remarks</span></span>

<span data-ttu-id="362c6-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="362c6-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="362c6-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="362c6-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="362c6-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="362c6-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="362c6-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="362c6-135">Schema name</span></span>  <br/> |<span data-ttu-id="362c6-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="362c6-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="362c6-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="362c6-137">Validation file</span></span>  <br/> |<span data-ttu-id="362c6-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="362c6-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="362c6-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="362c6-139">Can be empty</span></span>  <br/> |<span data-ttu-id="362c6-140">False</span><span class="sxs-lookup"><span data-stu-id="362c6-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="362c6-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="362c6-141">See also</span></span>



[<span data-ttu-id="362c6-142">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="362c6-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="362c6-143">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="362c6-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

