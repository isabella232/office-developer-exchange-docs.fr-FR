---
title: Struct fonction cchksgfiles. PAGE_INFO
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
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 5ec9f4303b26ea95b125adac6943945ae1276439
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456338"
---
# <a name="cchksgfilespage_info-struct"></a><span data-ttu-id="87b87-103">Struct fonction cchksgfiles. PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="87b87-103">CChkSGFiles.PAGE_INFO struct</span></span>

<span data-ttu-id="87b87-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="87b87-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="87b87-105">Contient des informations sur une page de base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="87b87-105">Holds information for an Exchange database page.</span></span> <span data-ttu-id="87b87-106">Cette structure est utilisée avec la fonction **ErrCheckDbPages** .</span><span class="sxs-lookup"><span data-stu-id="87b87-106">This structure is used with the **ErrCheckDbPages** function.</span></span> 
  
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

## <a name="members"></a><span data-ttu-id="87b87-107">Members</span><span class="sxs-lookup"><span data-stu-id="87b87-107">Members</span></span>

### <a name="ulpgno"></a><span data-ttu-id="87b87-108">ulPgNo</span><span class="sxs-lookup"><span data-stu-id="87b87-108">ulPgNo</span></span>
  
<span data-ttu-id="87b87-109">Long non signé.</span><span class="sxs-lookup"><span data-stu-id="87b87-109">Unsigned Long.</span></span> <span data-ttu-id="87b87-110">Numéro de page logique de la page de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="87b87-110">Logical page number of the database page to be checked.</span></span> <span data-ttu-id="87b87-111">Cette valeur doit être définie avant l’appel de **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="87b87-111">This value must be set before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="87b87-112">Si l’application lit le fichier en fonction des décalages de fichiers et doit donc mapper les offsets de fichier aux numéros de page logiques, la méthode **PgnoFromFileOffset** est utile pour déterminer la valeur de ce champ.</span><span class="sxs-lookup"><span data-stu-id="87b87-112">If the application is reading the file based on file offsets, and must therefore map those file offsets to logical page numbers, you will find the **PgnoFromFileOffset** method useful to determine the value for this field.</span></span> <span data-ttu-id="87b87-113">**ErrCheckDbPages** ne modifie pas cette valeur.</span><span class="sxs-lookup"><span data-stu-id="87b87-113">**ErrCheckDbPages** does not modify this value.</span></span> 
    
### <a name="fpageisinitialized"></a><span data-ttu-id="87b87-114">fPageIsInitialized</span><span class="sxs-lookup"><span data-stu-id="87b87-114">fPageIsInitialized</span></span> 
  
<span data-ttu-id="87b87-115">Type Boolean.</span><span class="sxs-lookup"><span data-stu-id="87b87-115">Boolean.</span></span> <span data-ttu-id="87b87-116">La valeur TRUE indique que la page de base de données contient des données.</span><span class="sxs-lookup"><span data-stu-id="87b87-116">A value of TRUE indicates that the database page contains data.</span></span> <span data-ttu-id="87b87-117">La valeur FALSe indique que la page contient uniquement des zéros.</span><span class="sxs-lookup"><span data-stu-id="87b87-117">A value of FALSE indicates that the page contains only zeros.</span></span> <span data-ttu-id="87b87-118">**ErrCheckDbPages** définit cette valeur.</span><span class="sxs-lookup"><span data-stu-id="87b87-118">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="fcorrectableerror"></a><span data-ttu-id="87b87-119">fCorrectableError</span><span class="sxs-lookup"><span data-stu-id="87b87-119">fCorrectableError</span></span>
  
<span data-ttu-id="87b87-120">Type Boolean.</span><span class="sxs-lookup"><span data-stu-id="87b87-120">Boolean.</span></span> <span data-ttu-id="87b87-121">La valeur TRUE indique qu’il y a eu une incohérence de checksum détectée dans la page de base de données, mais qu’il s’agit d’une erreur correcte.</span><span class="sxs-lookup"><span data-stu-id="87b87-121">A value of TRUE indicates that there was a checksum mismatch detected in the database page, but that it is a correctable error.</span></span> <span data-ttu-id="87b87-122">**ErrCheckDbPages** définit cette valeur.</span><span class="sxs-lookup"><span data-stu-id="87b87-122">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumactual"></a><span data-ttu-id="87b87-123">checksumActual</span><span class="sxs-lookup"><span data-stu-id="87b87-123">checksumActual</span></span>
  
<span data-ttu-id="87b87-124">Entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="87b87-124">Unsigned 64-bit integer.</span></span> <span data-ttu-id="87b87-125">Indique la valeur de checksum stockée dans la base de données pour cette page logique.</span><span class="sxs-lookup"><span data-stu-id="87b87-125">Indicates the checksum value stored in the database for this logical page.</span></span> <span data-ttu-id="87b87-126">**ErrCheckDbPages** définit cette valeur.</span><span class="sxs-lookup"><span data-stu-id="87b87-126">**ErrCheckDbPages** sets this value.</span></span> 
    
### <a name="checksumexpected"></a><span data-ttu-id="87b87-127">checksumExpected</span><span class="sxs-lookup"><span data-stu-id="87b87-127">checksumExpected</span></span>
  
<span data-ttu-id="87b87-128">Entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="87b87-128">Unsigned 64-bit integer.</span></span> <span data-ttu-id="87b87-129">Il s’agit de la valeur de checksum attendue qui est calculée pour la page de base de données ; elle est définie par **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="87b87-129">This is the expected checksum value that is calculated for the database page; it is set by **ErrCheckDbPages**.</span></span> <span data-ttu-id="87b87-130">Si cette valeur est différente de celle stockée sur la page de base de données (autrement dit, la valeur renvoyée dans **checksumActual**), **ErrCheckDbPages** indique qu’une erreur a été détectée sur cette page de base de données.</span><span class="sxs-lookup"><span data-stu-id="87b87-130">If this value is different from that stored on the database page (that is, the value returned in **checksumActual**), **ErrCheckDbPages** will indicate that an error was found on this database page.</span></span> 
    
### <a name="dbtime"></a><span data-ttu-id="87b87-131">dbTime</span><span class="sxs-lookup"><span data-stu-id="87b87-131">dbTime</span></span>
  
<span data-ttu-id="87b87-132">Entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="87b87-132">Unsigned 64-bit integer.</span></span> <span data-ttu-id="87b87-133">**ErrCheckDbPages** définit ce membre sur l’horodatage sur la page de base de données.</span><span class="sxs-lookup"><span data-stu-id="87b87-133">**ErrCheckDbPages** sets this member to the timestamp on the database page.</span></span> 
    
### <a name="checksumpagestructure"></a><span data-ttu-id="87b87-134">checksumPageStructure</span><span class="sxs-lookup"><span data-stu-id="87b87-134">checksumPageStructure</span></span> 
  
<span data-ttu-id="87b87-135">Entier 64-BT non signé.</span><span class="sxs-lookup"><span data-stu-id="87b87-135">Unsigned 64-bt integer.</span></span> <span data-ttu-id="87b87-136">**ErrCheckDbPages** définit ce membre sur la valeur de checksum calculée du contenu de la page, à l’exclusion des données qui ne sont pas nécessaires lors de la détermination de l’équivalence de page logique.</span><span class="sxs-lookup"><span data-stu-id="87b87-136">**ErrCheckDbPages** sets this member to the calculated checksum value of the contents of the page excluding data which is unnecessary when determining the logical page equivalence.</span></span> <span data-ttu-id="87b87-137">Par exemple, il n’est pas nécessaire de prendre en compte les valeurs des données dans l’espace de la page de base de données non utilisée.</span><span class="sxs-lookup"><span data-stu-id="87b87-137">For example, it is unnecessary to consider the data values in unused database page space.</span></span> <span data-ttu-id="87b87-138">Ce membre est valide uniquement si les valeurs **checksumActual** et **checksumExpected** sont égales les unes des autres.</span><span class="sxs-lookup"><span data-stu-id="87b87-138">This member is only valid if the **checksumActual**  and  **checksumExpected**  values are equal to each other.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="87b87-139">ulFlags</span><span class="sxs-lookup"><span data-stu-id="87b87-139">ulFlags</span></span>
  
<span data-ttu-id="87b87-140">Entier non signé 64 bits.</span><span class="sxs-lookup"><span data-stu-id="87b87-140">Unsigned 64-bit integer.</span></span> <span data-ttu-id="87b87-141">Réservé à une utilisation future.</span><span class="sxs-lookup"><span data-stu-id="87b87-141">Reserved for future use.</span></span> <span data-ttu-id="87b87-142">La valeur de ce champ doit être définie sur 0 (zéro) avant l’appel de **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="87b87-142">The value of this field must be set to 0 (zero) before calling **ErrCheckDbPages**.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="87b87-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="87b87-143">Remarks</span></span>

<span data-ttu-id="87b87-144">Lors de l’appel de la fonction **ErrCheckDbPages** , le paramètre **rgPageInfo** est un tableau de structures d' \*\* \_ infos sur la page\*\* .</span><span class="sxs-lookup"><span data-stu-id="87b87-144">When calling the **ErrCheckDbPages** function, the **rgPageInfo**  parameter is an array of **PAGE\_INFO** structures.</span></span> <span data-ttu-id="87b87-145">Il doit y avoir une structure d' \*\* \_ informations de page\*\* pour chaque page de base de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="87b87-145">There must be one **PAGE\_INFO** structure for each database page to be checked.</span></span> 
  
<span data-ttu-id="87b87-146">L’application doit définir le membre **ulPgno** sur la valeur appropriée, et doit également définir le membre **ulFlags** sur 0 (zéro) avant d’appeler **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="87b87-146">The application must set the **ulPgno**  member to the proper value, and must also set the  **ulFlags**  member to 0 (zero) before calling **ErrCheckDbPages**.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="87b87-147">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="87b87-147">Requirements</span></span>

<span data-ttu-id="87b87-148">Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="87b87-148">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="87b87-149">Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.</span><span class="sxs-lookup"><span data-stu-id="87b87-149">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

