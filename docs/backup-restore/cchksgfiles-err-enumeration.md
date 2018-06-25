---
title: Énumération CChkSGFiles.ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: 'Derni�re modification�: lundi 9 mars 2015'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755691"
---
# <a name="cchksgfileserr-enumeration"></a><span data-ttu-id="190bc-103">Énumération CChkSGFiles.ERR</span><span class="sxs-lookup"><span data-stu-id="190bc-103">CChkSGFiles.ERR enumeration</span></span> 
  
<span data-ttu-id="190bc-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="190bc-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="190bc-105">Indique le résultat de la fonction appelée.</span><span class="sxs-lookup"><span data-stu-id="190bc-105">Indicates the results of the called function.</span></span> <span data-ttu-id="190bc-106">Cette énumération est retournée par de nombreuses fonctions de la classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="190bc-106">This enumeration is returned by many functions of the **CCheckSGFiles** class.</span></span> 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a><span data-ttu-id="190bc-107">Valeurs</span><span class="sxs-lookup"><span data-stu-id="190bc-107">Values</span></span>

|<span data-ttu-id="190bc-108">**Nom du membre**</span><span class="sxs-lookup"><span data-stu-id="190bc-108">**Member name**</span></span>|<span data-ttu-id="190bc-109">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="190bc-109">**Value**</span></span>|<span data-ttu-id="190bc-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="190bc-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="190bc-111">errSuccess</span><span class="sxs-lookup"><span data-stu-id="190bc-111">errSuccess</span></span>  <br/> |<span data-ttu-id="190bc-112">0</span><span class="sxs-lookup"><span data-stu-id="190bc-112">0</span></span>  <br/> |<span data-ttu-id="190bc-113">La fonction s’est terminée sans erreur.</span><span class="sxs-lookup"><span data-stu-id="190bc-113">The function completed without any errors.</span></span>  <br/> |
|<span data-ttu-id="190bc-114">errTaskDropped</span><span class="sxs-lookup"><span data-stu-id="190bc-114">errTaskDropped</span></span>  <br/> |<span data-ttu-id="190bc-115">-106</span><span class="sxs-lookup"><span data-stu-id="190bc-115">-106</span></span>  <br/> |<span data-ttu-id="190bc-116">Renvoyée par la fonction **ErrTerm** pour indiquer que pas toutes les pages de base de données et fichiers journaux des transactions ont été vérifiées, ou que des erreurs se sont produites pendant la vérification.</span><span class="sxs-lookup"><span data-stu-id="190bc-116">Returned by the **ErrTerm** function to indicate that not all database pages and transaction log files were checked, or that errors were encountered during the verification.</span></span>  <br/> |
|<span data-ttu-id="190bc-117">errRequiredLogFilesMissing</span><span class="sxs-lookup"><span data-stu-id="190bc-117">errRequiredLogFilesMissing</span></span>  <br/> |<span data-ttu-id="190bc-118">-543</span><span class="sxs-lookup"><span data-stu-id="190bc-118">-543</span></span>  <br/> |<span data-ttu-id="190bc-119">Un ou plusieurs fichiers journaux qui sont nécessaires pour faire de la base de données à un état d’arrêt correct est introuvable dans le chemin d’accès du fichier journal, ou n’a pas le nom de base de trois lettres spécifié.</span><span class="sxs-lookup"><span data-stu-id="190bc-119">One or more log files that are required to bring the database to a clean-shutdown state was not found in the log file path, or did not have the specified three-letter base name.</span></span>  <br/> |
|<span data-ttu-id="190bc-120">errInvalidParameter</span><span class="sxs-lookup"><span data-stu-id="190bc-120">errInvalidParameter</span></span>  <br/> |<span data-ttu-id="190bc-121">-1003</span><span class="sxs-lookup"><span data-stu-id="190bc-121">-1003</span></span>  <br/> |<span data-ttu-id="190bc-122">Un ou plusieurs paramètres qui ont été transmis à la fonction ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="190bc-122">One or more parameters that were passed to the function were invalid.</span></span>  <br/> |
|<span data-ttu-id="190bc-123">errOutOfMemory</span><span class="sxs-lookup"><span data-stu-id="190bc-123">errOutOfMemory</span></span>  <br/> |<span data-ttu-id="190bc-124">-1011</span><span class="sxs-lookup"><span data-stu-id="190bc-124">-1011</span></span>  <br/> |<span data-ttu-id="190bc-125">Mémoire insuffisante n’était disponible pour effectuer l’opération demandée.</span><span class="sxs-lookup"><span data-stu-id="190bc-125">Insufficient memory was available to complete the requested operation.</span></span>  <br/> |
|<span data-ttu-id="190bc-126">errReadVerifyFailure</span><span class="sxs-lookup"><span data-stu-id="190bc-126">errReadVerifyFailure</span></span>  <br/> |<span data-ttu-id="190bc-127">-1018</span><span class="sxs-lookup"><span data-stu-id="190bc-127">-1018</span></span>  <br/> |<span data-ttu-id="190bc-128">La somme de contrôle qui est stocké dans une page de base de données ne correspond pas à la somme de contrôle attendue.</span><span class="sxs-lookup"><span data-stu-id="190bc-128">The checksum that is stored on a database page does not match its expected checksum.</span></span>  <br/> |
|<span data-ttu-id="190bc-129">errTooManyActiveUsers</span><span class="sxs-lookup"><span data-stu-id="190bc-129">errTooManyActiveUsers</span></span>  <br/> |<span data-ttu-id="190bc-130">-1059</span><span class="sxs-lookup"><span data-stu-id="190bc-130">-1059</span></span>  <br/> |<span data-ttu-id="190bc-131">La fonction **ErrTerm** a été appelée alors que l’objet a été en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="190bc-131">The **ErrTerm** function was called while the object was still being used.</span></span> <span data-ttu-id="190bc-132">Cela peut se produire si **ErrTerm** est appelé avant **ErrCheckDbPages** ou **ErrCheckLogFiles** a renvoyé.</span><span class="sxs-lookup"><span data-stu-id="190bc-132">This can occur if **ErrTerm** is called before **ErrCheckDbPages** or **ErrCheckLogFiles** has returned.</span></span>  <br/> |
   
## <a name="requirements"></a><span data-ttu-id="190bc-133">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="190bc-133">Requirements</span></span>

<span data-ttu-id="190bc-134">Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="190bc-134">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="190bc-135">Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="190bc-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

