---
title: Fonction cchksgfiles. ERR, énumération
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
description: Dernière modification le 9 mars 2015
ms.openlocfilehash: dbc76601a808f79ce3ed5b5dc9fbe4cf92efb015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455253"
---
# <a name="cchksgfileserr-enumeration"></a><span data-ttu-id="137b3-103">Fonction cchksgfiles. ERR, énumération</span><span class="sxs-lookup"><span data-stu-id="137b3-103">CChkSGFiles.ERR enumeration</span></span> 
  
<span data-ttu-id="137b3-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="137b3-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="137b3-105">Indique les résultats de la fonction appelée.</span><span class="sxs-lookup"><span data-stu-id="137b3-105">Indicates the results of the called function.</span></span> <span data-ttu-id="137b3-106">Cette énumération est renvoyée par de nombreuses fonctions de la classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="137b3-106">This enumeration is returned by many functions of the **CCheckSGFiles** class.</span></span> 
  
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

## <a name="values"></a><span data-ttu-id="137b3-107">Values</span><span class="sxs-lookup"><span data-stu-id="137b3-107">Values</span></span>

|<span data-ttu-id="137b3-108">**Nom du membre**</span><span class="sxs-lookup"><span data-stu-id="137b3-108">**Member name**</span></span>|<span data-ttu-id="137b3-109">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="137b3-109">**Value**</span></span>|<span data-ttu-id="137b3-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="137b3-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="137b3-111">errSuccess</span><span class="sxs-lookup"><span data-stu-id="137b3-111">errSuccess</span></span>  <br/> |<span data-ttu-id="137b3-112">0</span><span class="sxs-lookup"><span data-stu-id="137b3-112">0</span></span>  <br/> |<span data-ttu-id="137b3-113">La fonction s’est terminée sans erreur.</span><span class="sxs-lookup"><span data-stu-id="137b3-113">The function completed without any errors.</span></span>  <br/> |
|<span data-ttu-id="137b3-114">errTaskDropped</span><span class="sxs-lookup"><span data-stu-id="137b3-114">errTaskDropped</span></span>  <br/> |<span data-ttu-id="137b3-115">-106</span><span class="sxs-lookup"><span data-stu-id="137b3-115">-106</span></span>  <br/> |<span data-ttu-id="137b3-116">Renvoyé par la fonction **ErrTerm** pour indiquer que toutes les pages de base de données et tous les fichiers journaux de transaction ont été vérifiés, ou que des erreurs ont été rencontrées lors de la vérification.</span><span class="sxs-lookup"><span data-stu-id="137b3-116">Returned by the **ErrTerm** function to indicate that not all database pages and transaction log files were checked, or that errors were encountered during the verification.</span></span>  <br/> |
|<span data-ttu-id="137b3-117">errRequiredLogFilesMissing</span><span class="sxs-lookup"><span data-stu-id="137b3-117">errRequiredLogFilesMissing</span></span>  <br/> |<span data-ttu-id="137b3-118">-543</span><span class="sxs-lookup"><span data-stu-id="137b3-118">-543</span></span>  <br/> |<span data-ttu-id="137b3-119">Un ou plusieurs fichiers journaux requis pour ramener la base de données à un état d’arrêt correct n’ont pas été trouvés dans le chemin d’accès au fichier journal, ou n’ont pas le nom de base à trois lettres spécifié.</span><span class="sxs-lookup"><span data-stu-id="137b3-119">One or more log files that are required to bring the database to a clean-shutdown state was not found in the log file path, or did not have the specified three-letter base name.</span></span>  <br/> |
|<span data-ttu-id="137b3-120">errInvalidParameter</span><span class="sxs-lookup"><span data-stu-id="137b3-120">errInvalidParameter</span></span>  <br/> |<span data-ttu-id="137b3-121">-1003</span><span class="sxs-lookup"><span data-stu-id="137b3-121">-1003</span></span>  <br/> |<span data-ttu-id="137b3-122">Un ou plusieurs paramètres transmis à la fonction ne sont pas valides.</span><span class="sxs-lookup"><span data-stu-id="137b3-122">One or more parameters that were passed to the function were invalid.</span></span>  <br/> |
|<span data-ttu-id="137b3-123">errOutOfMemory</span><span class="sxs-lookup"><span data-stu-id="137b3-123">errOutOfMemory</span></span>  <br/> |<span data-ttu-id="137b3-124">-1011</span><span class="sxs-lookup"><span data-stu-id="137b3-124">-1011</span></span>  <br/> |<span data-ttu-id="137b3-125">Mémoire insuffisante pour terminer l’opération demandée.</span><span class="sxs-lookup"><span data-stu-id="137b3-125">Insufficient memory was available to complete the requested operation.</span></span>  <br/> |
|<span data-ttu-id="137b3-126">errReadVerifyFailure</span><span class="sxs-lookup"><span data-stu-id="137b3-126">errReadVerifyFailure</span></span>  <br/> |<span data-ttu-id="137b3-127">-1018</span><span class="sxs-lookup"><span data-stu-id="137b3-127">-1018</span></span>  <br/> |<span data-ttu-id="137b3-128">La somme de contrôle stockée sur une page de base de données ne correspond pas à son checksum attendu.</span><span class="sxs-lookup"><span data-stu-id="137b3-128">The checksum that is stored on a database page does not match its expected checksum.</span></span>  <br/> |
|<span data-ttu-id="137b3-129">errTooManyActiveUsers</span><span class="sxs-lookup"><span data-stu-id="137b3-129">errTooManyActiveUsers</span></span>  <br/> |<span data-ttu-id="137b3-130">-1059</span><span class="sxs-lookup"><span data-stu-id="137b3-130">-1059</span></span>  <br/> |<span data-ttu-id="137b3-131">La fonction **ErrTerm** a été appelée alors que l’objet était toujours en cours d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="137b3-131">The **ErrTerm** function was called while the object was still being used.</span></span> <span data-ttu-id="137b3-132">Cela peut se produire si **ErrTerm** est appelé avant que **ErrCheckDbPages** ou **ErrCheckLogFiles** n’ait été renvoyé.</span><span class="sxs-lookup"><span data-stu-id="137b3-132">This can occur if **ErrTerm** is called before **ErrCheckDbPages** or **ErrCheckLogFiles** has returned.</span></span>  <br/> |
   
## <a name="requirements"></a><span data-ttu-id="137b3-133">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="137b3-133">Requirements</span></span>

<span data-ttu-id="137b3-134">Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="137b3-134">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="137b3-135">Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.</span><span class="sxs-lookup"><span data-stu-id="137b3-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

