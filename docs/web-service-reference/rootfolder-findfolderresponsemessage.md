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
description: L’élément RootFolder contient les résultats d’une recherche d’un dossier racine unique pendant une opération FindFolder.
ms.openlocfilehash: b5601d6abec67196c9991908e272a2122a201d69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457136"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="10a52-103">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="10a52-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="10a52-104">L’élément **RootFolder** contient les résultats d’une recherche d’un dossier racine unique pendant une [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="10a52-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="10a52-105">**FindFolderParentType**</span><span class="sxs-lookup"><span data-stu-id="10a52-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10a52-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="10a52-106">Attributes and elements</span></span>

<span data-ttu-id="10a52-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="10a52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10a52-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="10a52-108">Attributes</span></span>

|<span data-ttu-id="10a52-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="10a52-109">**Attribute**</span></span>|<span data-ttu-id="10a52-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="10a52-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="10a52-111">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="10a52-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="10a52-112">Représente l’index suivant qui doit être utilisé pour la requête suivante lors de l’utilisation d’une vue de pagination indexée.</span><span class="sxs-lookup"><span data-stu-id="10a52-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="10a52-113">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="10a52-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="10a52-114">Représente la nouvelle valeur de numérateur à utiliser pour la requête suivante lors de l’utilisation d’affichages de page fractionnaires.</span><span class="sxs-lookup"><span data-stu-id="10a52-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="10a52-115">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="10a52-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="10a52-116">Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination fractionnée.</span><span class="sxs-lookup"><span data-stu-id="10a52-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="10a52-117">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="10a52-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="10a52-118">Indique si les résultats actuels contiennent le dernier dossier de la requête, de sorte qu’aucune pagination supplémentaire n’est nécessaire.</span><span class="sxs-lookup"><span data-stu-id="10a52-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="10a52-119">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="10a52-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="10a52-120">Représente le nombre total de dossiers qui ont passé la restriction.</span><span class="sxs-lookup"><span data-stu-id="10a52-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="10a52-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="10a52-121">Child elements</span></span>

|<span data-ttu-id="10a52-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="10a52-122">**Element**</span></span>|<span data-ttu-id="10a52-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="10a52-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10a52-124">Dossiers</span><span class="sxs-lookup"><span data-stu-id="10a52-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="10a52-125">Contient un tableau de dossiers trouvés à l’aide de l' [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="10a52-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10a52-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="10a52-126">Parent elements</span></span>

|<span data-ttu-id="10a52-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="10a52-127">**Element**</span></span>|<span data-ttu-id="10a52-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="10a52-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10a52-129">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="10a52-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="10a52-130">Contient l’État et le résultat d’une demande d' [opération FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="10a52-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="10a52-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="10a52-131">Remarks</span></span>

<span data-ttu-id="10a52-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="10a52-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10a52-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="10a52-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10a52-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="10a52-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="10a52-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="10a52-135">Schema name</span></span>  <br/> |<span data-ttu-id="10a52-136">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="10a52-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="10a52-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="10a52-137">Validation file</span></span>  <br/> |<span data-ttu-id="10a52-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="10a52-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="10a52-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="10a52-139">Can be empty</span></span>  <br/> |<span data-ttu-id="10a52-140">False</span><span class="sxs-lookup"><span data-stu-id="10a52-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10a52-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10a52-141">See also</span></span>



[<span data-ttu-id="10a52-142">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="10a52-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="10a52-143">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="10a52-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

