---
title: Fonction CChkSGFiles.PgnoFromFileOffset
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
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: d42ba7c8178c6fccdddec0b5da88a972f51184c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754753"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="6235e-103">Fonction CChkSGFiles.PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="6235e-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="6235e-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="6235e-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="6235e-105">Renvoie le numéro de page logique de la base de données qui correspond à l’index spécifié d’octets dans le fichier de base de données physique.</span><span class="sxs-lookup"><span data-stu-id="6235e-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="6235e-106">Si le décalage de fichier n’est pas valide, ou si la fonction **ErrCheckDbHeaders** n’a pas été appelée pour les bases de données, cette fonction renvoie la valeur 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="6235e-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="6235e-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="6235e-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="6235e-108">ibFileOffset</span><span class="sxs-lookup"><span data-stu-id="6235e-108">ibFileOffset</span></span>
  
<span data-ttu-id="6235e-109">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="6235e-109">Input parameter.</span></span> <span data-ttu-id="6235e-110">Offset dans un fichier de base de données, en octets.</span><span class="sxs-lookup"><span data-stu-id="6235e-110">The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="6235e-111">Valeur renvoy�e</span><span class="sxs-lookup"><span data-stu-id="6235e-111">Return value</span></span>

<span data-ttu-id="6235e-112">Numéro de page logique du fichier de base de données qui inclut l’offset spécifié.</span><span class="sxs-lookup"><span data-stu-id="6235e-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6235e-113">Remarques</span><span class="sxs-lookup"><span data-stu-id="6235e-113">Remarks</span></span>

<span data-ttu-id="6235e-114">Si le paramètre **ibFileOffset** n’est pas valide, la fonction **PgnoFromFileOffset** renvoie la valeur 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="6235e-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="6235e-115">**PgnoFromFileOffset** renvoie également 0 (zéro) si vous n’avez pas appelé la fonction **ErrCheckDbHeaders** sur l’instance **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="6235e-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="6235e-116">Vous devez appeler **ErrCheckDbHeaders** pour initialiser la taille de page de base de données et du nombre de pages allouées aux en-têtes de base de données.</span><span class="sxs-lookup"><span data-stu-id="6235e-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="6235e-117">Vous devez utiliser **PgnoFromFileOffset** pour remplir le **PAGE\_INFO** éléments en vue de l’appel **ErrCheckDbPages**de structure.</span><span class="sxs-lookup"><span data-stu-id="6235e-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="6235e-118">Le paramètre **rgPageInfo** pour **ErrCheckDbPages** requiert une structure **PAGE_INFO** , avec les valeurs du membre **ulPgno** correctement initialisé chaque élément dans le tableau.</span><span class="sxs-lookup"><span data-stu-id="6235e-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="6235e-119">Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **PgnoFromFileOffset** dans la partie de l’application multithread.</span><span class="sxs-lookup"><span data-stu-id="6235e-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="6235e-120">Notez que vous devez généralement appeler cette fonction plusieurs fois pour chaque base de données en cours d’archivage.</span><span class="sxs-lookup"><span data-stu-id="6235e-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="6235e-121">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="6235e-121">Requirements</span></span>

<span data-ttu-id="6235e-122">Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="6235e-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="6235e-123">L’application s’exécute sous le compte doit avoir autorisation de lecture sur les base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="6235e-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

