---
title: Fonction fonction cchksgfiles. PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 3c8f749a03b4aa251bf9312eba5d7e2d46c91fae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452894"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="b7ba4-103">Fonction fonction cchksgfiles. PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="b7ba4-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="b7ba4-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b7ba4-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="b7ba4-105">Renvoie le numéro de page de base de données logique correspondant à l’index d’octet spécifié dans le fichier de base de données physique.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="b7ba4-106">Si le décalage du fichier n’est pas valide ou si la fonction **ErrCheckDbHeaders** n’a pas été appelée pour les bases de données, cette fonction renvoie la valeur 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="b7ba4-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="b7ba4-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="b7ba4-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="b7ba4-108">ibFileOffset</span><span class="sxs-lookup"><span data-stu-id="b7ba4-108">ibFileOffset</span></span>
  
<span data-ttu-id="b7ba4-109">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-109">Input parameter.</span></span> <span data-ttu-id="b7ba4-110">Offset dans un fichier de base de données, en octets.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-110">The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="b7ba4-111">Valeur renvoyée</span><span class="sxs-lookup"><span data-stu-id="b7ba4-111">Return value</span></span>

<span data-ttu-id="b7ba4-112">Numéro de page logique du fichier de base de données qui inclut le décalage spécifié.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b7ba4-113">Remarques</span><span class="sxs-lookup"><span data-stu-id="b7ba4-113">Remarks</span></span>

<span data-ttu-id="b7ba4-114">Si le paramètre **ibFileOffset** n’est pas valide, la fonction **PgnoFromFileOffset** renvoie 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="b7ba4-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="b7ba4-115">**PgnoFromFileOffset** renvoie également 0 (zéro) si vous n’avez pas appelé la fonction **ErrCheckDbHeaders** sur l’instance **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="b7ba4-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="b7ba4-116">Vous devez appeler **ErrCheckDbHeaders** pour initialiser la taille de la page de base de données et le nombre de pages allouées aux en-têtes de base de données.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="b7ba4-117">Vous devez utiliser **PgnoFromFileOffset** pour remplir les éléments de structure d' \*\* \_ informations\*\* en préparation à l’appel de **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="b7ba4-118">Le paramètre **rgPageInfo** de **ErrCheckDbPages** exige que chaque élément du tableau soit une structure **PAGE_INFO** , avec les valeurs de membre **ulPgno** correctement initialisées.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="b7ba4-119">Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **PgnoFromFileOffset** dans la partie multithread de l’application.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="b7ba4-120">Notez que vous appelez généralement cette fonction plusieurs fois pour chaque base de données vérifiée.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="b7ba4-121">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="b7ba4-121">Requirements</span></span>

<span data-ttu-id="b7ba4-122">Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="b7ba4-123">Le compte sous lequel l’application s’exécute doit disposer d’une autorisation de lecture sur la base de données et les fichiers journaux à vérifier.</span><span class="sxs-lookup"><span data-stu-id="b7ba4-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

