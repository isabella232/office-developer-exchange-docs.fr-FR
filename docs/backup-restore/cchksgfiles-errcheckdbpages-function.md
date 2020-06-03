---
title: Fonction fonction cchksgfiles. ErrCheckDbPages
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
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 78d2dbee6253096d597b4ec2de3878f40ee1b6d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526724"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="a7900-103">Fonction fonction cchksgfiles. ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="a7900-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="a7900-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a7900-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="a7900-105">Valide une plage de pages dans une base de données spécifiée.</span><span class="sxs-lookup"><span data-stu-id="a7900-105">Validates a range of pages in a specified database.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="a7900-106">Paramètres</span><span class="sxs-lookup"><span data-stu-id="a7900-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="a7900-107">iDb</span><span class="sxs-lookup"><span data-stu-id="a7900-107">iDb</span></span>
  
<span data-ttu-id="a7900-108">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="a7900-108">Input parameter.</span></span> <span data-ttu-id="a7900-109">Index du tableau de bases de données spécifié dans le paramètre **rgwszDb []** de la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="a7900-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="a7900-110">La base de données indexée par ce paramètre est vérifiée.</span><span class="sxs-lookup"><span data-stu-id="a7900-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="a7900-111">pvPageBuffer</span><span class="sxs-lookup"><span data-stu-id="a7900-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="a7900-112">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="a7900-112">Input parameter.</span></span> <span data-ttu-id="a7900-113">Pointeur vers une mémoire tampon contenant une ou plusieurs pages de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="a7900-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="a7900-114">La taille de la mémoire tampon doit être un multiple de la taille de la page de la base de données, tel qu’il est renvoyé dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="a7900-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="a7900-115">L’application appelante doit remplir la mémoire tampon avec le contenu de la page de base de données avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="a7900-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="a7900-116">cbPageBuffer</span><span class="sxs-lookup"><span data-stu-id="a7900-116">cbPageBuffer</span></span>
  
<span data-ttu-id="a7900-117">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="a7900-117">Input parameter.</span></span> <span data-ttu-id="a7900-118">Taille du paramètre **pvPageBuffer** , en octets.</span><span class="sxs-lookup"><span data-stu-id="a7900-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="a7900-119">Cette valeur doit être un multiple de la taille de la page de la base de données, tel qu’il est renvoyé dans le paramètre **pcbDbPageSize** par la fonction **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="a7900-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="a7900-120">rgPageInfo[]</span><span class="sxs-lookup"><span data-stu-id="a7900-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="a7900-121">Paramètre d’entrée/sortie.</span><span class="sxs-lookup"><span data-stu-id="a7900-121">Input/output parameter.</span></span> <span data-ttu-id="a7900-122">Tableau des structures **d' \_ infos sur la page** que **ErrCheckDbPages** remplit avec les résultats détaillés de chaque page de base de données qui est vérifiée.</span><span class="sxs-lookup"><span data-stu-id="a7900-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="a7900-123">Le tableau doit avoir un élément pour chaque page de base de données passée dans le paramètre **pvPageBuffer** , et le champ **ulPgno** dans chaque structure d' \*\* \_ informations de page\*\* doit être défini sur le numéro de page logique qui correspond à la page de base de données.</span><span class="sxs-lookup"><span data-stu-id="a7900-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="a7900-124">Pour plus d’informations, consultez la section « Remarques » plus loin dans cette rubrique.</span><span class="sxs-lookup"><span data-stu-id="a7900-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="a7900-125">cPageInfo</span><span class="sxs-lookup"><span data-stu-id="a7900-125">cPageInfo</span></span>
  
<span data-ttu-id="a7900-126">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="a7900-126">Input parameter.</span></span> <span data-ttu-id="a7900-127">Nombre d’entrées dans le tableau **rgPageInfo []** .</span><span class="sxs-lookup"><span data-stu-id="a7900-127">The number of entries in the **rgPageInfo[]** array.</span></span> <span data-ttu-id="a7900-128">Cette valeur doit être égale au nombre de pages de base de données transmises dans le paramètre **pvPageBuffer** .</span><span class="sxs-lookup"><span data-stu-id="a7900-128">This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="a7900-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="a7900-129">ulFlags</span></span> 
  
<span data-ttu-id="a7900-130">Paramètre d’entrée facultatif.</span><span class="sxs-lookup"><span data-stu-id="a7900-130">Optional input parameter.</span></span> <span data-ttu-id="a7900-131">Cette valeur est réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="a7900-131">This value is reserved for future use.</span></span> <span data-ttu-id="a7900-132">La valeur transmise dans ce paramètre doit être 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="a7900-132">The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="a7900-133">Valeur renvoyée</span><span class="sxs-lookup"><span data-stu-id="a7900-133">Return value</span></span>

<span data-ttu-id="a7900-134">Un code d’erreur à partir de l’énumération [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="a7900-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a7900-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="a7900-135">Remarks</span></span>

<span data-ttu-id="a7900-136">Notez que vous devez avoir spécifié la base de données dans le tableau de bases de données transmises à la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="a7900-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="a7900-137">De plus, **ErrCheckDbHeaders** doit être appelé avant **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="a7900-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="a7900-138">L’application appelante doit allouer un tampon de mémoire suffisamment grand pour contenir les pages de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="a7900-138">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked.</span></span> <span data-ttu-id="a7900-139">L’application est chargée de remplir la mémoire tampon avec le contenu d’une ou de plusieurs pages de base de données de ce type.</span><span class="sxs-lookup"><span data-stu-id="a7900-139">The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="a7900-140">L’application appelante doit appeler **ErrCheckDbHeaders** avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="a7900-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="a7900-141">Cette fonction peut être appelée autant de fois que nécessaire pour traiter toutes les pages de tous les fichiers de base de données qui doivent être vérifiés.</span><span class="sxs-lookup"><span data-stu-id="a7900-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="a7900-142">Dans le paramètre **rgPageInfo []** , chaque élément renvoyé contient des informations sur la page de base de données dans une structure d' \*\* \_ informations de page\*\* .</span><span class="sxs-lookup"><span data-stu-id="a7900-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="a7900-143">Si la fonction **ErrCheckDbPages** renvoie une erreur, l’application doit vérifier chaque structure d' \*\* \_ informations\*\* pour déterminer la page sur laquelle l’erreur a été trouvée.</span><span class="sxs-lookup"><span data-stu-id="a7900-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="a7900-144">Par exemple, la comparaison des valeurs **checksumActual** et **checksumExpected** indique si une erreur de checksum a été détectée sur cette page de base de données.</span><span class="sxs-lookup"><span data-stu-id="a7900-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="a7900-145">Si **ErrCheckDbPages** détecte des erreurs dans le contenu de la base de données, il crée une entrée de journal d’événements d’erreurs Windows.</span><span class="sxs-lookup"><span data-stu-id="a7900-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="a7900-146">L’objet **fonction cchksgfiles** détermine si toutes les bases de données enregistrées avec la fonction **ErrInit** ont été vérifiées.</span><span class="sxs-lookup"><span data-stu-id="a7900-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="a7900-147">Plus précisément, **fonction cchksgfiles** utilise la fonction **ErrCheckDbPages** pour déterminer si le même nombre de pages de base de données indiqué par **ErrCheckDbHeaders** a été vérifié.</span><span class="sxs-lookup"><span data-stu-id="a7900-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="a7900-148">Si le nombre correct de pages de chaque base de données n’a pas été correctement vérifié, la fonction **ErrTerm** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="a7900-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="a7900-149">Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckDbPages** dans la partie multithread de l’application.</span><span class="sxs-lookup"><span data-stu-id="a7900-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="a7900-150">Notez que **ErrCheckDbPages** est généralement appelé plusieurs fois pour chaque base de données vérifiée.</span><span class="sxs-lookup"><span data-stu-id="a7900-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="a7900-151">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="a7900-151">Requirements</span></span>

<span data-ttu-id="a7900-152">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="a7900-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="a7900-153">Le compte sous lequel l’application s’exécute doit disposer d’autorisations de lecture pour la base de données et les fichiers journaux qui doivent être vérifiés.</span><span class="sxs-lookup"><span data-stu-id="a7900-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

