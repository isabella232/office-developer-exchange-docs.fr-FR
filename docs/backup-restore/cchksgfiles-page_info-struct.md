---
title: Struct CChkSGFiles.PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755685"
---
# <a name="cchksgfilespageinfo-struct"></a><span data-ttu-id="2cdab-103">Struct CChkSGFiles.PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="2cdab-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="2cdab-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="2cdab-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="2cdab-105">Contient des informations pour une page de base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="2cdab-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="2cdab-106">Cette structure est utilisée avec la fonction **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="2cdab-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a><span data-ttu-id="2cdab-107">Membres</span><span class="sxs-lookup"><span data-stu-id="2cdab-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="2cdab-108">ulPgNo</span><span class="sxs-lookup"><span data-stu-id="2cdab-108">ulPgNo</span></span>
  
<span data-ttu-id="2cdab-109">Long non signé.</span><span class="sxs-lookup"><span data-stu-id="2cdab-109">Unsigned Long.</span></span> <span data-ttu-id="2cdab-110">Numéro de page logique de la page de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="2cdab-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="2cdab-111">Cette valeur doit être définie avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="2cdab-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="2cdab-112">Si l’application lit le fichier basé sur le fichier décalages et doit par conséquent mapper les décalages fichier aux numéros de page logique, vous trouverez la méthode **PgnoFromFileOffset** permet de déterminer la valeur de ce champ.</span><span class="sxs-lookup"><span data-stu-id="2cdab-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="2cdab-113">**ErrCheckDbPages** ne modifie pas cette valeur.</span><span class="sxs-lookup"><span data-stu-id="2cdab-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="2cdab-114">fPageIsInitialized</span><span class="sxs-lookup"><span data-stu-id="2cdab-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="2cdab-115">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2cdab-115">Boolean.</span></span> <span data-ttu-id="2cdab-116">La valeur TRUE indique que la page de base de données contient des données.</span><span class="sxs-lookup"><span data-stu-id="2cdab-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="2cdab-117">La valeur FALSE indique que la page contienne des zéros.</span><span class="sxs-lookup"><span data-stu-id="2cdab-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="2cdab-118">**ErrCheckDbPages** définit cette valeur.</span><span class="sxs-lookup"><span data-stu-id="2cdab-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="2cdab-119">fCorrectableError</span><span class="sxs-lookup"><span data-stu-id="2cdab-119">fCorrectableError</span></span>
  
<span data-ttu-id="2cdab-120">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2cdab-120">Boolean.</span></span> <span data-ttu-id="2cdab-121">La valeur TRUE indique qu’il y a une incohérence dans des totaux détectée dans la page de base de données, mais qu’il s’agit d’une erreur peut être corrigée.</span><span class="sxs-lookup"><span data-stu-id="2cdab-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="2cdab-122">**ErrCheckDbPages** définit cette valeur.</span><span class="sxs-lookup"><span data-stu-id="2cdab-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="2cdab-123">checksumActual</span><span class="sxs-lookup"><span data-stu-id="2cdab-123">checksumActual</span></span>
  
<span data-ttu-id="2cdab-124">Nombre entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="2cdab-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="2cdab-125">Indique la valeur de la somme de contrôle stockée dans la base de données de cette page logique.</span><span class="sxs-lookup"><span data-stu-id="2cdab-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="2cdab-126">**ErrCheckDbPages** définit cette valeur.</span><span class="sxs-lookup"><span data-stu-id="2cdab-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="2cdab-127">checksumExpected</span><span class="sxs-lookup"><span data-stu-id="2cdab-127">checksumExpected</span></span>
  
<span data-ttu-id="2cdab-128">Nombre entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="2cdab-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="2cdab-129">Il s’agit de la valeur de somme de contrôle attendue est calculée de la page de la base de données ; Il est défini par **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="2cdab-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="2cdab-130">Si cette valeur est différente de celui stocké dans la page de base de données (autrement dit, la valeur retournée dans **checksumActual**), **ErrCheckDbPages** indique qu’une erreur a été trouvée dans cette page de la base de données.</span><span class="sxs-lookup"><span data-stu-id="2cdab-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="2cdab-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="2cdab-131">dbTime</span></span>
  
<span data-ttu-id="2cdab-132">Nombre entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="2cdab-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="2cdab-133">**ErrCheckDbPages** définit ce membre à l’horodatage dans la page de base de données.</span><span class="sxs-lookup"><span data-stu-id="2cdab-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="2cdab-134">checksumPageStructure</span><span class="sxs-lookup"><span data-stu-id="2cdab-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="2cdab-135">Nombre entier non signé 64-cc.</span><span class="sxs-lookup"><span data-stu-id="2cdab-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="2cdab-136">**ErrCheckDbPages** définit ce membre à la valeur calculée de somme de contrôle du contenu de la page à l’exclusion des données qui ne sont pas nécessaires lors de la détermination de l’équivalence logique de page.</span><span class="sxs-lookup"><span data-stu-id="2cdab-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="2cdab-137">Par exemple, il est inutile à prendre en compte les valeurs de données dans l’espace de page de base de données inutilisés.</span><span class="sxs-lookup"><span data-stu-id="2cdab-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="2cdab-138">Ce membre est valide uniquement si les valeurs **checksumActual** et **checksumExpected** sont égales.</span><span class="sxs-lookup"><span data-stu-id="2cdab-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="2cdab-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="2cdab-139">ulFlags</span></span>
  
<span data-ttu-id="2cdab-140">Nombre entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="2cdab-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="2cdab-141">Réservé à une utilisation ultérieure.</span><span class="sxs-lookup"><span data-stu-id="2cdab-141">Reserved for future use.</span></span> <span data-ttu-id="2cdab-142">La valeur de ce champ doit être définie sur 0 (zéro) avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="2cdab-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2cdab-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="2cdab-143">Remarks</span></span>

<span data-ttu-id="2cdab-144">Lorsque vous appelez la fonction **ErrCheckDbPages** , le paramètre **rgPageInfo** est un tableau de **PAGE\_INFO** structures.</span><span class="sxs-lookup"><span data-stu-id="2cdab-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="2cdab-145">Il doit y avoir un **PAGE\_INFO** structure pour chaque page de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="2cdab-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="2cdab-146">L’application doit définir le membre **ulPgno** à la valeur correcte et doit également définir le membre **ulFlags** à 0 (zéro) avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="2cdab-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="2cdab-147">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="2cdab-147">Requirements</span></span>

<span data-ttu-id="2cdab-148">Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="2cdab-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="2cdab-149">Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="2cdab-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

