---
title: Fonction CChkSGFiles.ErrCheckDbPages
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: f1588b1dbc4bd7e83683fa4432a175405ad17903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754745"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="e2cbe-103">Fonction CChkSGFiles.ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="e2cbe-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="e2cbe-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="e2cbe-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="e2cbe-105">Valide une plage de pages dans une base de données spécifié.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-105">Validates a range of pages in a specified database.</span></span> 
  
```cs
Vitual ERRErrCheckDbPages  
(
    Const ULONGiDb,
    Const VOID  * const pvPageBuffer,
    Const ULONGcbPageBuffer,
    PAGE_INFOrgPageInfo[],
    Const ULONGcPageInfo,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="e2cbe-106">Paramètres</span><span class="sxs-lookup"><span data-stu-id="e2cbe-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="e2cbe-107">iDb</span><span class="sxs-lookup"><span data-stu-id="e2cbe-107">iDb</span></span>
  
<span data-ttu-id="e2cbe-108">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-108">Input parameter.</span></span> <span data-ttu-id="e2cbe-109">Un index dans le tableau des bases de données spécifié dans le paramètre **[] rgwszDb** à la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="e2cbe-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="e2cbe-110">La base de données indexée par ce paramètre sera vérifiée.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="e2cbe-111">pvPageBuffer</span><span class="sxs-lookup"><span data-stu-id="e2cbe-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="e2cbe-112">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-112">Input parameter.</span></span> <span data-ttu-id="e2cbe-113">Pointeur vers un tampon qui contient une ou plusieurs pages de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="e2cbe-114">La taille de la mémoire tampon doit être un multiple de la taille de page de base de données, renvoyée dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="e2cbe-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="e2cbe-115">L’application appelante doit remplir la mémoire tampon avec le contenu de page de base de données avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="e2cbe-116">cbPageBuffer</span><span class="sxs-lookup"><span data-stu-id="e2cbe-116">cbPageBuffer</span></span>
  
<span data-ttu-id="e2cbe-117">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-117">Input parameter.</span></span> <span data-ttu-id="e2cbe-118">La taille du paramètre **pvPageBuffer** , en octets.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="e2cbe-119">Cette valeur doit être un multiple de la taille de page de base de données, renvoyée dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="e2cbe-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="e2cbe-120">[] rgPageInfo</span><span class="sxs-lookup"><span data-stu-id="e2cbe-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="e2cbe-121">Paramètre d’entrée/sortie.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-121">Input/output parameter.</span></span> <span data-ttu-id="e2cbe-122">Un tableau de **PAGE\_INFO** structures **ErrCheckDbPages** remplit avec le détail des résultats de chaque page de base de données est vérifiée.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="e2cbe-123">Le tableau doit avoir un élément pour chaque page de base de données transmis dans le paramètre **pvPageBuffer** et le champ **ulPgno** dans chaque **PAGE\_INFO** structure doit être définie sur le numéro de page logique qui correspond à la page de base de données.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="e2cbe-124">Pour plus d’informations, voir « Remarques » plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="e2cbe-125">cPageInfo</span><span class="sxs-lookup"><span data-stu-id="e2cbe-125">cPageInfo</span></span>
  
<span data-ttu-id="e2cbe-126">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-126">Input parameter.</span></span> <span data-ttu-id="e2cbe-127">Le nombre d’entrées dans le tableau **[] rgPageInfo** .</span><span class="sxs-lookup"><span data-stu-id="e2cbe-127">The number of entries in the **rgPageInfo[]** array.</span></span> <span data-ttu-id="e2cbe-128">Cette valeur doit être égale au nombre de pages de base de données transmis dans le paramètre **pvPageBuffer** .</span><span class="sxs-lookup"><span data-stu-id="e2cbe-128">This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="e2cbe-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="e2cbe-129">ulFlags</span></span> 
  
<span data-ttu-id="e2cbe-130">Paramètre d’entrée facultatif.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-130">Optional input parameter.</span></span> <span data-ttu-id="e2cbe-131">Cette valeur est réservée pour une utilisation future.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-131">This value is reserved for future use.</span></span> <span data-ttu-id="e2cbe-132">La valeur passée dans ce paramètre doit être 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="e2cbe-132">The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="e2cbe-133">Valeur renvoy�e</span><span class="sxs-lookup"><span data-stu-id="e2cbe-133">Return value</span></span>

<span data-ttu-id="e2cbe-134">Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="e2cbe-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e2cbe-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="e2cbe-135">Remarks</span></span>

<span data-ttu-id="e2cbe-136">Notez que vous devez avoir spécifié la base de données dans le tableau des bases de données transmis à la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="e2cbe-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="e2cbe-137">En outre, **ErrCheckDbHeaders** doit être appelé avant **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="e2cbe-138">L’application appelante doit allouer une mémoire tampon qui est suffisante pour contenir les pages de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-138">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked.</span></span> <span data-ttu-id="e2cbe-139">L’application est chargée pour remplir la mémoire tampon avec le contenu d’une ou plusieurs des pages de base de données.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-139">The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="e2cbe-140">L’application appelante doit appeler **ErrCheckDbHeaders** avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="e2cbe-141">Cette fonction peut être appelée autant de fois que nécessaire pour couvrir toutes les pages de tous les fichiers de base de données qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="e2cbe-142">Dans le paramètre **[] rgPageInfo** , chaque élément renvoyé contient des informations sur la page de base de données dans un **PAGE\_INFO** structure.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="e2cbe-143">Si la fonction **ErrCheckDbPages** renvoie une erreur, l’application doit vérifier chacune **PAGE\_INFO** structure pour déterminer la page sur laquelle l’erreur a été trouvé.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="e2cbe-144">Par exemple, comparant les valeurs **checksumActual** et **checksumExpected** indique si une erreur de somme de contrôle a été détectée sur cette page de la base de données.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="e2cbe-145">Si **ErrCheckDbPages** détecte des erreurs dans le contenu de la base de données, il crée une entrée de journal des événements d’erreur Windows.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="e2cbe-146">L’objet **CChkSGFiles** détermine si les bases de données qui utilisent la fonction **ErrInit** ont été réellement activés.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="e2cbe-147">Plus précisément, **CChkSGFiles** utilise la fonction de **ErrCheckDbPages** pour déterminer si le même nombre de pages de base de données indiqué par **ErrCheckDbHeaders** ont été vérifié réellement.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="e2cbe-148">Si le nombre approprié de pages dans chaque base de données n’ont pas été archivé avec succès, la fonction **ErrTerm** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="e2cbe-149">Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckDbPages** dans la partie de l’application multithread.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="e2cbe-150">Notez que **ErrCheckDbPages** est généralement appelée plusieurs fois pour chaque base de données est vérifiée.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="e2cbe-151">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="e2cbe-151">Requirements</span></span>

<span data-ttu-id="e2cbe-152">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="e2cbe-153">Le compte que l’application s’exécute sous doit avoir lecture des autorisations pour les fichiers journaux et de base de données qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="e2cbe-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

