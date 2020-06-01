---
title: Fonction fonction cchksgfiles. ErrInit
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
description: 'Dernière modification : 1er mars 2013'
ms.openlocfilehash: c881691e7c1ba83a396e659f6aac0328625e49a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457010"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="fbdbc-103">Fonction fonction cchksgfiles. ErrInit</span><span class="sxs-lookup"><span data-stu-id="fbdbc-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="fbdbc-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="fbdbc-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="fbdbc-105">Initialise l’objet **fonction cchksgfiles** en spécifiant les bases de données à vérifier et le chemin d’accès et le nom de base des fichiers journaux de transactions à vérifier.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="fbdbc-106">Les applications doivent appeler cette fonction immédiatement après avoir réussi à appeler la **nouvelle** fonction.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="fbdbc-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="fbdbc-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="fbdbc-108">rgwszDb[]</span><span class="sxs-lookup"><span data-stu-id="fbdbc-108">rgwszDb[]</span></span>
  
<span data-ttu-id="fbdbc-109">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-109">Input parameter.</span></span> <span data-ttu-id="fbdbc-110">Tableau qui spécifie les bases de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-110">An array that specifies the databases to be checked.</span></span> <span data-ttu-id="fbdbc-111">Chaque élément de tableau est une chaîne Unicode terminée par un caractère null qui contient le chemin d’accès et le nom de fichier d’une base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-111">Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="fbdbc-112">cDB</span><span class="sxs-lookup"><span data-stu-id="fbdbc-112">cDB</span></span>
  
<span data-ttu-id="fbdbc-113">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-113">Input parameter.</span></span> <span data-ttu-id="fbdbc-114">Nombre d’éléments de chemin d’accès de base de données valides dans le tableau **rgwszDb** .</span><span class="sxs-lookup"><span data-stu-id="fbdbc-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="fbdbc-115">wszLogPath</span><span class="sxs-lookup"><span data-stu-id="fbdbc-115">wszLogPath</span></span>
  
<span data-ttu-id="fbdbc-116">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-116">Input parameter.</span></span> <span data-ttu-id="fbdbc-117">Chemin d’accès complet des fichiers du journal des transactions à vérifier, sous la forme d’une chaîne Unicode terminée par un caractère null.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="fbdbc-118">wszBaseName</span><span class="sxs-lookup"><span data-stu-id="fbdbc-118">wszBaseName</span></span>
  
<span data-ttu-id="fbdbc-119">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-119">Input parameter.</span></span> <span data-ttu-id="fbdbc-120">Nom de base à trois lettres des fichiers journaux de transactions Exchange, sous la forme d’une chaîne Unicode terminée par un caractère null.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="fbdbc-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="fbdbc-121">ulFlags</span></span>
  
<span data-ttu-id="fbdbc-122">Paramètre d’entrée facultatif.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-122">Optional input parameter.</span></span> <span data-ttu-id="fbdbc-123">Cette valeur est réservée à un usage ultérieur.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-123">This value is reserved for future use.</span></span> <span data-ttu-id="fbdbc-124">La valeur passée par ce paramètre doit être 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="fbdbc-124">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="fbdbc-125">Valeur renvoyée</span><span class="sxs-lookup"><span data-stu-id="fbdbc-125">Return value</span></span>

<span data-ttu-id="fbdbc-126">Un code d’erreur à partir de l’énumération [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="fbdbc-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fbdbc-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="fbdbc-127">Remarks</span></span>

<span data-ttu-id="fbdbc-128">La fonction **ErrInit** enregistre les bases de données et les fichiers journaux qui doivent être vérifiés.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="fbdbc-129">Cette fonction doit être appelée après l’appel de la fonction **New** , mais avant l’appel de toute autre fonction **ChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="fbdbc-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="fbdbc-130">Vous devez fournir tous les noms de base de données, le chemin d’accès au fichier journal et le nom de base comme chaînes Unicode terminées par un caractère null.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="fbdbc-131">Vous pouvez vérifier uniquement les fichiers de base de données, uniquement les fichiers journaux, ou les fichiers de base de données et les fichiers journaux.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="fbdbc-132">Toutefois, lors de l’appel de cette fonction, l’application doit spécifier au moins une entité à vérifier.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="fbdbc-133">Le passage de la valeur 0 (zéro) pour **CDB** et null pour **wszLogPath** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="fbdbc-134">Si la valeur de **CDB** est différente de 0 (zéro), le fait de transmettre null pour **rgwszDb** génère une erreur.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="fbdbc-135">Pour vérifier les fichiers de base de données, l’application doit fournir les noms de base de données.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="fbdbc-136">Si NULL est passé pour **wszBaseName** mais **wszLogPath** n’est pas null, une erreur est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="fbdbc-137">Un nom de base de fichier journal est toujours requis lors de la vérification des fichiers journaux.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="fbdbc-138">Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrInit** dans la partie à thread unique de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="fbdbc-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="fbdbc-139">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="fbdbc-139">Requirements</span></span>

<span data-ttu-id="fbdbc-140">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="fbdbc-141">Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.</span><span class="sxs-lookup"><span data-stu-id="fbdbc-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

