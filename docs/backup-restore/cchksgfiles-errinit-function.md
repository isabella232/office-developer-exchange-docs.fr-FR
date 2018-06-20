---
title: Fonction CChkSGFiles.ErrInit
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Dernière modification : 03 mars 2013'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754744"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="75540-103">Fonction CChkSGFiles.ErrInit</span><span class="sxs-lookup"><span data-stu-id="75540-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="75540-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="75540-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="75540-105">Initialise l’objet **CChkSGFiles** en spécifiant les bases de données à vérifier et le chemin d’accès et nom de base des fichiers journaux des transactions à vérifier.</span><span class="sxs-lookup"><span data-stu-id="75540-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="75540-106">Applications doivent appeler cette fonction immédiatement après l’appel avec succès la fonction **New** .</span><span class="sxs-lookup"><span data-stu-id="75540-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="75540-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="75540-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="75540-108">[] rgwszDb</span><span class="sxs-lookup"><span data-stu-id="75540-108">rgwszDb[]</span></span>
  
<span data-ttu-id="75540-109">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="75540-109">Input parameter.</span></span> <span data-ttu-id="75540-110">Tableau qui spécifie les bases de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="75540-110">An array that specifies the databases to be checked.</span></span> <span data-ttu-id="75540-111">Chaque élément de tableau est une chaîne Unicode terminée par le caractère null qui contient le chemin d’accès et le nom de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="75540-111">Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="75540-112">cDB</span><span class="sxs-lookup"><span data-stu-id="75540-112">cDB</span></span>
  
<span data-ttu-id="75540-113">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="75540-113">Input parameter.</span></span> <span data-ttu-id="75540-114">Le nombre d’éléments de chemin d’accès valide de la base de données dans le tableau **rgwszDb** .</span><span class="sxs-lookup"><span data-stu-id="75540-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="75540-115">wszLogPath</span><span class="sxs-lookup"><span data-stu-id="75540-115">wszLogPath</span></span>
  
<span data-ttu-id="75540-116">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="75540-116">Input parameter.</span></span> <span data-ttu-id="75540-117">Chemin d’accès complet des fichiers journaux des transactions à vérifier, sous la forme d’une chaîne Unicode terminée par null.</span><span class="sxs-lookup"><span data-stu-id="75540-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="75540-118">wszBaseName</span><span class="sxs-lookup"><span data-stu-id="75540-118">wszBaseName</span></span>
  
<span data-ttu-id="75540-119">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="75540-119">Input parameter.</span></span> <span data-ttu-id="75540-120">Le trois lettres nom de base les fichiers journaux des transactions, sous la forme d’une chaîne Unicode terminée par null.</span><span class="sxs-lookup"><span data-stu-id="75540-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="75540-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="75540-121">ulFlags</span></span>
  
<span data-ttu-id="75540-122">Paramètre d’entrée facultatif.</span><span class="sxs-lookup"><span data-stu-id="75540-122">Optional input parameter.</span></span> <span data-ttu-id="75540-123">Cette valeur est réservée pour une utilisation future.</span><span class="sxs-lookup"><span data-stu-id="75540-123">This value is reserved for future use.</span></span> <span data-ttu-id="75540-124">La valeur transmise à ce paramètre doit être 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="75540-124">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="75540-125">Valeur renvoy�e</span><span class="sxs-lookup"><span data-stu-id="75540-125">Return value</span></span>

<span data-ttu-id="75540-126">Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="75540-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="75540-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="75540-127">Remarks</span></span>

<span data-ttu-id="75540-128">La fonction **ErrInit** enregistre les bases de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="75540-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="75540-129">Cette fonction doit être appelée après la fonction **New** est appelée, mais avant toute autre **ChkSGFiles** l’appel de fonction.</span><span class="sxs-lookup"><span data-stu-id="75540-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="75540-130">Vous devez fournir le nom de base, le chemin d’accès du fichier journal et tous les noms de base de données en tant que chaînes Unicode.</span><span class="sxs-lookup"><span data-stu-id="75540-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="75540-131">Vous pouvez vérifier que les fichiers de base de données, seuls les fichiers journaux ou les fichiers journaux et de base de données.</span><span class="sxs-lookup"><span data-stu-id="75540-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="75540-132">Toutefois, lorsque vous appelez cette fonction, l’application doit spécifier au moins une entité à vérifier.</span><span class="sxs-lookup"><span data-stu-id="75540-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="75540-133">Passer la valeur 0 (zéro) pour **cDB** et NULL pour **wszLogPath** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="75540-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="75540-134">Si la valeur de **cDB** est différente de 0 (zéro), en passant NULL pour **rgwszDb** provoquera une erreur.</span><span class="sxs-lookup"><span data-stu-id="75540-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="75540-135">Pour vérifier les fichiers de base de données, l’application doit fournir les noms de base de données.</span><span class="sxs-lookup"><span data-stu-id="75540-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="75540-136">Si NULL est passé pour **wszBaseName** mais **wszLogPath** n’est pas NULL, une erreur sera renvoyée.</span><span class="sxs-lookup"><span data-stu-id="75540-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="75540-137">Un nom de base du fichier journal est toujours requis lors de la vérification des fichiers journaux.</span><span class="sxs-lookup"><span data-stu-id="75540-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="75540-138">Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrInit** dans la partie d’un seul thread de l’application, et vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="75540-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="75540-139">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="75540-139">Requirements</span></span>

<span data-ttu-id="75540-140">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="75540-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="75540-141">Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="75540-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

