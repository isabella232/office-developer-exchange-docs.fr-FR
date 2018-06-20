---
title: Fonction CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754752"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a><span data-ttu-id="41b3c-103">Fonction CChkSGFiles.ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="41b3c-103">CChkSGFiles.ErrCheckDbHeaders function</span></span>

<span data-ttu-id="41b3c-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="41b3c-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span> 
  
<span data-ttu-id="41b3c-105">Valide les en-têtes des fichiers de base de données qui ont été spécifiés par la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="41b3c-105">Validates the headers of the database files that were specified by the **ErrInit** function.</span></span> <span data-ttu-id="41b3c-106">Cette fonction renvoie également la taille de la page et le nombre de pages dans chacune des bases de données spécifiés.</span><span class="sxs-lookup"><span data-stu-id="41b3c-106">This function also returns the page size and number of pages in each of the specified databases.</span></span> 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="41b3c-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="41b3c-107">Parameters</span></span>

### <a name="pcbdbpagesize"></a><span data-ttu-id="41b3c-108">pcbDbPageSize</span><span class="sxs-lookup"><span data-stu-id="41b3c-108">pcbDbPageSize</span></span> 
  
<span data-ttu-id="41b3c-109">Paramètre de sortie.</span><span class="sxs-lookup"><span data-stu-id="41b3c-109">Output parameter.</span></span> <span data-ttu-id="41b3c-110">La taille de page de chacune des bases de données spécifiées, en octets.</span><span class="sxs-lookup"><span data-stu-id="41b3c-110">The page size of each of the specified databases, in bytes.</span></span>
    
### <a name="pcheaderpagesperdb"></a><span data-ttu-id="41b3c-111">pcHeaderPagesPerDb</span><span class="sxs-lookup"><span data-stu-id="41b3c-111">pcHeaderPagesPerDb</span></span> 
  
<span data-ttu-id="41b3c-112">Paramètre de sortie.</span><span class="sxs-lookup"><span data-stu-id="41b3c-112">Output parameter.</span></span> <span data-ttu-id="41b3c-113">Le nombre de pages au début de chaque spécifié de base de données qui sont réservés par le moteur de base de données pour un usage interne.</span><span class="sxs-lookup"><span data-stu-id="41b3c-113">The number of pages at the beginning of each specified database that are reserved by the database engine for internal use.</span></span> <span data-ttu-id="41b3c-114">Notez que vous ne devez *pas* les pages d’en-tête passe à la fonction **ErrCheckDbPages** pour la validation.</span><span class="sxs-lookup"><span data-stu-id="41b3c-114">Note that you should *not* pass header pages to the **ErrCheckDbPages** function for validation.</span></span> 
    
### <a name="pidberrorencountered"></a><span data-ttu-id="41b3c-115">piDbErrorEncountered</span><span class="sxs-lookup"><span data-stu-id="41b3c-115">piDbErrorEncountered</span></span>
  
<span data-ttu-id="41b3c-116">Paramètre de sortie.</span><span class="sxs-lookup"><span data-stu-id="41b3c-116">Output parameter.</span></span> <span data-ttu-id="41b3c-117">Si la valeur de retour de la fonction indique une erreur, ce paramètre est un index dans le tableau **[] rgwszDb** transmis à la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="41b3c-117">If the return value of the function indicates an error, this parameter will be an index into the **rgwszDb[]** array passed to the **ErrInit** function.</span></span> <span data-ttu-id="41b3c-118">L’élément de tableau indexé représente la base de données dans laquelle l’erreur.</span><span class="sxs-lookup"><span data-stu-id="41b3c-118">The indexed array element represents the database in which the error was encountered.</span></span> <span data-ttu-id="41b3c-119">Si la fonction ne retourne pas une valeur d’erreur, cette valeur de paramètre non valide.</span><span class="sxs-lookup"><span data-stu-id="41b3c-119">If the function does not return an error value, this parameter value is invalid.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="41b3c-120">ulFlags</span><span class="sxs-lookup"><span data-stu-id="41b3c-120">ulFlags</span></span> 
  
<span data-ttu-id="41b3c-121">Paramètre d’entrée facultatif.</span><span class="sxs-lookup"><span data-stu-id="41b3c-121">Optional input parameter.</span></span> <span data-ttu-id="41b3c-122">Cette valeur est réservée pour une utilisation future.</span><span class="sxs-lookup"><span data-stu-id="41b3c-122">This value is reserved for future use.</span></span> <span data-ttu-id="41b3c-123">La valeur passée doit être 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="41b3c-123">The value passed should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="41b3c-124">Valeur renvoy�e</span><span class="sxs-lookup"><span data-stu-id="41b3c-124">Return value</span></span>

<span data-ttu-id="41b3c-125">Cette fonction retourne un code d’erreur à partir de l' [énumération CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).</span><span class="sxs-lookup"><span data-stu-id="41b3c-125">This function returns an error code from the [CChkSGFiles.ERR enumeration](cchksgfiles-err-enumeration.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41b3c-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="41b3c-126">Remarks</span></span>

<span data-ttu-id="41b3c-127">**ErrCheckDbHeaders** vérifie que toutes les bases de données sont enregistrées avec **ErrInit** ont la même base de données et de signature page taille du journal.</span><span class="sxs-lookup"><span data-stu-id="41b3c-127">**ErrCheckDbHeaders** verifies that all databases registered with **ErrInit** have the same log signature and database page size.</span></span> <span data-ttu-id="41b3c-128">Vous pouvez également utiliser la valeur du paramètre **genMin** la plus faible et la valeur du paramètre **genMax** la plus élevée pour déterminer l’ensemble des fichiers journaux qui sont nécessaires pour mettre toutes les bases de données enregistrés à un état d’arrêt correct.</span><span class="sxs-lookup"><span data-stu-id="41b3c-128">You can also use the lowest **genMin** parameter value and the highest **genMax** parameter value to determine the set of log files that are necessary to bring all of the registered databases to a clean-shutdown state.</span></span> 
  
<span data-ttu-id="41b3c-129">Le paramètre **piDbErrorEncountered** est défini uniquement lorsqu’une erreur est détectée, comme indiqué par un zéro **ErrCheckDbHeaders** valeur de retour.</span><span class="sxs-lookup"><span data-stu-id="41b3c-129">The **piDbErrorEncountered** parameter is set only when an error is detected, as indicated by a non-zero **ErrCheckDbHeaders** return value.</span></span> 
  
<span data-ttu-id="41b3c-130">Lorsqu’une erreur se produit dans cette fonction, un événement d’erreur sera ajouté au journal des événements Windows.</span><span class="sxs-lookup"><span data-stu-id="41b3c-130">When an error occurs in this function, an error event will be added to the Windows Error event log.</span></span>
  
<span data-ttu-id="41b3c-131">Vous pouvez appeler **ErrCheckDbHeaders** uniquement après l’appel de **ErrInit**, et vous devez l’appeler avant d’appeler **ErrCheckDbPages** et **ErrCheckLogs**.</span><span class="sxs-lookup"><span data-stu-id="41b3c-131">You can call **ErrCheckDbHeaders** only after calling **ErrInit**, and you must call it before calling **ErrCheckDbPages** and **ErrCheckLogs**.</span></span>
  
<span data-ttu-id="41b3c-132">Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrCheckDbHeaders** dans la partie d’un seul thread, et vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="41b3c-132">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrCheckDbHeaders** function in the single-threaded portion, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="41b3c-133">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="41b3c-133">Requirements</span></span>

<span data-ttu-id="41b3c-134">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="41b3c-134">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="41b3c-135">Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="41b3c-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

