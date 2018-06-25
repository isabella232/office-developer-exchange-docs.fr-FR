---
title: Fonction CChkSGFiles.ErrCheckLogs
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754748"
---
# <a name="cchksgfileserrchecklogs-function"></a><span data-ttu-id="bd520-103">Fonction CChkSGFiles.ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="bd520-103">CChkSGFiles.ErrCheckLogs function</span></span>

<span data-ttu-id="bd520-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="bd520-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="bd520-105">Valide les fichiers journaux de tous les fichiers de base de données n’a été spécifiés dans la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="bd520-105">Validates the log files of all the database files that were specified in the **ErrInit** function.</span></span> <span data-ttu-id="bd520-106">Les journaux validés sont ceux qui existent dans le chemin d’accès, et dont le nom de fichier journal de base de trois lettres transmis à **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="bd520-106">The validated logs are those that exist in the path, and that have the three-letter base log file name passed to **ErrInit**.</span></span>
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="bd520-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="bd520-107">Parameters</span></span>

### <a name="pfonlyunnecessarylogscorrupt"></a><span data-ttu-id="bd520-108">pfOnlyUnnecessaryLogsCorrupt</span><span class="sxs-lookup"><span data-stu-id="bd520-108">pfOnlyUnnecessaryLogsCorrupt</span></span> 
  
<span data-ttu-id="bd520-109">Paramètre de sortie.</span><span class="sxs-lookup"><span data-stu-id="bd520-109">Output parameter.</span></span> <span data-ttu-id="bd520-110">Lorsque **la valeur true**, ce paramètre indique que les erreurs ont été trouvées dans les fichiers journaux des transactions, mais ces erreurs ont été tous trouvés dans les fichiers journaux qui ne sont pas nécessaires pour mettre la base de données à un état d’arrêt correct sans perte de données.</span><span class="sxs-lookup"><span data-stu-id="bd520-110">When **true**, this parameter indicates that errors were found in the transaction log files, but those errors were all found in log files that are not needed to bring the database to a clean-shutdown state without data loss.</span></span> <span data-ttu-id="bd520-111">Une valeur **true** est renvoyée dans ce paramètre est valide uniquement lorsque **ErrCheckLogs** renvoie **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="bd520-111">A **true** value returned in this parameter is valid only when **ErrCheckLogs** returns **errSuccess**.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="bd520-112">ulFlags</span><span class="sxs-lookup"><span data-stu-id="bd520-112">ulFlags</span></span>
  
<span data-ttu-id="bd520-113">Paramètre d’entrée facultatif.</span><span class="sxs-lookup"><span data-stu-id="bd520-113">Optional input parameter.</span></span> <span data-ttu-id="bd520-114">Cette valeur est réservée pour une utilisation future.</span><span class="sxs-lookup"><span data-stu-id="bd520-114">This value is reserved for future use.</span></span> <span data-ttu-id="bd520-115">La valeur transmise à ce paramètre doit être 0 (zéro).</span><span class="sxs-lookup"><span data-stu-id="bd520-115">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="bd520-116">Valeur renvoy�e</span><span class="sxs-lookup"><span data-stu-id="bd520-116">Return value</span></span>

<span data-ttu-id="bd520-117">Code d’erreur à partir de l’énumération [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="bd520-117">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
<span data-ttu-id="bd520-118">Il est important de noter que cette fonction peut renvoyer **errSuccess** même cas d’erreurs dans les fichiers journaux.</span><span class="sxs-lookup"><span data-stu-id="bd520-118">It's important to remember that this function can return **errSuccess** even when errors are found in the log files.</span></span> <span data-ttu-id="bd520-119">Par conséquent, lorsque **ErrCheckLogs** renvoie **errSuccess**, l’application doit également vérifier le paramètre de retour **pfOnlyUnnecessaryLogsCorrupt** .</span><span class="sxs-lookup"><span data-stu-id="bd520-119">Therefore, when **ErrCheckLogs** returns **errSuccess**, the application should also check the  **pfOnlyUnnecessaryLogsCorrupt** return parameter.</span></span> <span data-ttu-id="bd520-120">Si **pfOnlyUnnecessaryLogsCorrupts** a la **valeur true** lorsque **ErrCheckLogs** renvoie **errSuccess**, cela indique qu’une ou plusieurs erreurs ont été détectés, mais uniquement dans les fichiers journaux non nécessaires pour mettre à jour la base de données.</span><span class="sxs-lookup"><span data-stu-id="bd520-120">If **pfOnlyUnnecessaryLogsCorrupts** is **true** when **ErrCheckLogs** returns **errSuccess**, this indicates that one or more errors were found, but only in log files not needed to bring the database up-to-date.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd520-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="bd520-121">Remarks</span></span>

<span data-ttu-id="bd520-122">La fonction **ErrCheckDbHeaders** doit être appelée avant que la fonction **ErrCheckLogs** peut être appelée.</span><span class="sxs-lookup"><span data-stu-id="bd520-122">The **ErrCheckDbHeaders** function must be called before the **ErrCheckLogs** function can be called.</span></span> 
  
<span data-ttu-id="bd520-123">Lorsque les fichiers journaux des transactions de base de données sont vérifiées, certaines des fichiers journaux seront nécessaires pour mettre les bases de données dans le groupe de stockage pour un état d’arrêt correct sans perte de données, tandis que d’autres fichiers journaux ne peuvent pas être nécessaires.</span><span class="sxs-lookup"><span data-stu-id="bd520-123">When Exchange database transaction log files are being checked, some of the log files will be necessary to bring the databases in the storage group to a clean-shutdown state without data loss, whereas other log files might not be needed.</span></span> <span data-ttu-id="bd520-124">La fonction **ErrCheckLogs** détermine les plus anciens et les fichiers journaux plus récents qui sont nécessaires pour mettre à jour les bases de données.</span><span class="sxs-lookup"><span data-stu-id="bd520-124">The **ErrCheckLogs** function determines both the oldest and the newest log files that are needed to bring the databases up to date.</span></span> 
  
<span data-ttu-id="bd520-125">La fonction **ErrCheckLogs** vérifie tous les fichiers journaux dans les chemins d’accès spécifiés qui ont également le nom de fichier de base de trois lettres spécifié, tel qu’il est transmis à la fonction **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="bd520-125">The **ErrCheckLogs** function verifies all the log files in the specified paths that also have the specified three-letter base file name, as passed to the **ErrInit** function.</span></span> 
  
<span data-ttu-id="bd520-126">Si aucune erreur n’est détectée dans les fichiers journaux, **ErrCheckLogs** renvoie **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="bd520-126">If no errors are found in the log files, **ErrCheckLogs** returns **errSuccess**.</span></span> 
  
<span data-ttu-id="bd520-127">Si les fichiers journaux requis sont endommagées, **ErrCheckLogs** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="bd520-127">If any of the required log files are found to be corrupted, **ErrCheckLogs** returns an error.</span></span> 
  
<span data-ttu-id="bd520-128">Si des erreurs sont détectées uniquement dans les fichiers journaux qui sont antérieurs à la plus ancienne ceux qui sont nécessaires, la fonction renvoie **errSuccess** et définit le paramètre de retour **pfOnlyUnnecessaryLogCorrupt** sur **true**.</span><span class="sxs-lookup"><span data-stu-id="bd520-128">If errors are found only in log files that are older than the earliest ones needed, the function returns **errSuccess** and sets the return parameter **pfOnlyUnnecessaryLogCorrupt** to **true**.</span></span> <span data-ttu-id="bd520-129">L’application doit reconnaître qu’il existe des erreurs dans certains de ces fichiers journaux ancienne, et dans ce cas, il sera peut-être avertir l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bd520-129">The application should recognize that there are errors in some of those old log files, and if so, it will possibly alert the user.</span></span> <span data-ttu-id="bd520-130">Dans tous les cas, ces erreurs ne doivent pas affecter l’intégrité globale de la base de données ou affecter la réussite de lire les journaux.</span><span class="sxs-lookup"><span data-stu-id="bd520-130">In any case, those errors should not affect the overall integrity of the database or affect whether playing the logs forward will succeed.</span></span>
  
<span data-ttu-id="bd520-131">Si des erreurs sont détectées dans tous les fichiers journaux créés après la plus proche journal détermine **ErrCheckLogs** est nécessaire, la fonction renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="bd520-131">If errors are found in any log file created after the earliest log that **ErrCheckLogs** determines is needed, the function returns an error.</span></span> <span data-ttu-id="bd520-132">L’erreur s’afficheront même si l’erreur du fichier journal a été trouvée dans un fichier journal qui a été généré postérieure à ce qui est nécessaire pour mettre à jour la base de données.</span><span class="sxs-lookup"><span data-stu-id="bd520-132">The error will be returned even if the log file error was found in a log file that was generated later than what is needed to bring the database up to date.</span></span> <span data-ttu-id="bd520-133">Bien qu’il est possible de mettre les bases de données à un état d’arrêt correct à l’aide de fichiers journaux identifiés, spécifiées dans les fichiers plus tard endommagé journaux des transactions n’est pas appliquées, entraînant une perte de données lors de la base de données est restaurée.</span><span class="sxs-lookup"><span data-stu-id="bd520-133">Although it would be possible to bring the databases to a clean-shutdown state by using the identified log files, transactions specified in the later corrupted log files would not be applied, resulting in data loss when the database is restored.</span></span> 
  
<span data-ttu-id="bd520-134">L’objet **CChkSGFiles** détermine si tous les fichiers journaux enregistrés avec la fonction **ErrInit** vérifiés réellement.</span><span class="sxs-lookup"><span data-stu-id="bd520-134">The **CChkSGFiles** object determines whether all of the log files registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="bd520-135">Si ce n’est pas le cas, tous les journaux ont été correctement désactivée, la fonction **ErrTerm** renvoie une erreur.</span><span class="sxs-lookup"><span data-stu-id="bd520-135">If not all of the logs were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="bd520-136">Si vous utilisez CHKSGFILES dans une application multithread, vous pouvez appeler la fonction **ErrCheckLogs** dans la partie de l’application multithread, mais vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="bd520-136">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckLogs** function in the multithreaded portion of the application, but you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="bd520-137">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="bd520-137">Requirements</span></span>

<span data-ttu-id="bd520-138">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="bd520-138">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="bd520-139">Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="bd520-139">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

