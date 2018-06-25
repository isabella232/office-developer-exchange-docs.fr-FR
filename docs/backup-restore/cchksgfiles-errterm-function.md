---
title: Fonction CChkSGFiles.ErrTerm
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Dernière modification : 25 février 2013'
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754750"
---
# <a name="cchksgfileserrterm-function"></a><span data-ttu-id="0e63c-103">Fonction CChkSGFiles.ErrTerm</span><span class="sxs-lookup"><span data-stu-id="0e63c-103">CChkSGFiles.ErrTerm function</span></span>
  
<span data-ttu-id="0e63c-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0e63c-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="0e63c-105">Fournit un état global de la vérification de base de données et journaux, ce qui indique si les pages de base de données et les journaux ont été vérifiées avec succès.</span><span class="sxs-lookup"><span data-stu-id="0e63c-105">Provides an overall status of the database and log verification, which indicates whether all the database pages and logs were successfully verified.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="0e63c-106">Groupes de stockage ne sont pas disponibles dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="0e63c-106">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="0e63c-107">Pour assurer la compatibilité descendante avec les bases de données et les groupes de stockage dans les versions d’Exchange antérieures à Exchange Server 2010, l’API CHKSGFILES vous permet de spécifier les groupes de stockage.</span><span class="sxs-lookup"><span data-stu-id="0e63c-107">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange Server 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="0e63c-108">Lorsque vous exécutez CHKSGFILES par rapport à des bases de données Exchange 2013, vous devez définir les paramètres que vous spécifiez un identificateur de groupe de stockage sur une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="0e63c-108">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="0e63c-109">Paramètres</span><span class="sxs-lookup"><span data-stu-id="0e63c-109">Parameters</span></span>

### <a name="ulflags"></a><span data-ttu-id="0e63c-110">ulFlags</span><span class="sxs-lookup"><span data-stu-id="0e63c-110">ulFlags</span></span>
  
<span data-ttu-id="0e63c-111">Paramètre d’entrée facultatif.</span><span class="sxs-lookup"><span data-stu-id="0e63c-111">Optional input parameter.</span></span> <span data-ttu-id="0e63c-112">Cette valeur est réservée pour une utilisation future.</span><span class="sxs-lookup"><span data-stu-id="0e63c-112">This value is reserved for future use.</span></span> <span data-ttu-id="0e63c-113">La valeur transmise à ce paramètre doit être 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="0e63c-113">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="0e63c-114">Valeur renvoy�e</span><span class="sxs-lookup"><span data-stu-id="0e63c-114">Return value</span></span>

<span data-ttu-id="0e63c-115">Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="0e63c-115">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0e63c-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="0e63c-116">Remarks</span></span>

<span data-ttu-id="0e63c-117">L’objet **CChkSGFiles** détermine si les bases de données qui utilisent la fonction **ErrInit** ont été réellement activés.</span><span class="sxs-lookup"><span data-stu-id="0e63c-117">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="0e63c-118">Cet objet utilise la fonction **ErrCheckDbPages** pour vérifier que le même nombre de pages identifiées par la fonction **ErrCheckDbHeaders** ont été vérifiées réellement de base de données.</span><span class="sxs-lookup"><span data-stu-id="0e63c-118">This object uses the **ErrCheckDbPages** function to verify that the same number of database pages identified by the **ErrCheckDbHeaders** function were actually verified.</span></span> <span data-ttu-id="0e63c-119">Si le nombre approprié de pages dans chaque base de données n’est pas vérifié avec succès, la fonction **ErrTerm** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="0e63c-119">If the correct number of pages in each database are not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="0e63c-120">Si le nombre de pages de base de données avec **ErrCheckDbPages** est inférieur à celui indiqué par **ErrCheckDbHeaders**, cette fonction crée une erreur dans le journal des événements Windows et **ErrTerm** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="0e63c-120">If the number of database pages checked with **ErrCheckDbPages** is less than that indicated by **ErrCheckDbHeaders**, this function creates an error in the Windows Event log, and **ErrTerm** returns an error.</span></span> 
  
<span data-ttu-id="0e63c-121">Si le nombre de pages de base de données avec **ErrCheckDbPages** est supérieur à celle indiquée par **ErrCheckDbHeaders**, cette fonction crée un message d’avertissement dans le journal des événements Windows pour indiquer que l’application peut inutilement contrôler certains pages de base de données plusieurs fois.</span><span class="sxs-lookup"><span data-stu-id="0e63c-121">If the number of database pages checked with **ErrCheckDbPages** is greater than that indicated by **ErrCheckDbHeaders**, this function creates a warning in the Windows Event log to indicate that the application might be unnecessarily checking some database pages more than once.</span></span> <span data-ttu-id="0e63c-122">Dans ce cas, toutefois, la fonction **ErrTerm** réussit.</span><span class="sxs-lookup"><span data-stu-id="0e63c-122">In this case, however, the **ErrTerm** function succeeds.</span></span> 
  
<span data-ttu-id="0e63c-123">L’objet **CChkSGFiles** détermine également si les fichiers journaux enregistrés avec **ErrInit** vérifiés réellement.</span><span class="sxs-lookup"><span data-stu-id="0e63c-123">The **CChkSGFiles** object also determines whether the log files registered with **ErrInit** were actually checked.</span></span> <span data-ttu-id="0e63c-124">Si ce n’est pas le cas, tous les journaux ont été correctement activé, la fonction **ErrTerm** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="0e63c-124">If not all the logs were successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="0e63c-125">Lorsque **ErrTerm** renvoie une erreur, il sera la première erreur qu’il trouve, même si elle vérifie l’état de vérification pour toutes les bases de données sont enregistrées avec **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="0e63c-125">When **ErrTerm** returns an error, it will be the first error it finds, even though it checks the verification status for all databases registered with **ErrInit**.</span></span>
  
<span data-ttu-id="0e63c-126">Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **ErrTerm** dans la partie d’un seul thread de l’application, et vous ne pouvez l’appeler aucuns plus qu’une fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0e63c-126">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrTerm** function in the single-threaded portion of the application, and you can call it no more than once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="0e63c-127">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="0e63c-127">Requirements</span></span>

<span data-ttu-id="0e63c-128">Exchange 2013 inclut uniquement une version 64 bits de CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="0e63c-128">Exchange 2013 only includes a 64-bit version of CHKSGFILES.</span></span>
  
<span data-ttu-id="0e63c-129">Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="0e63c-129">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

