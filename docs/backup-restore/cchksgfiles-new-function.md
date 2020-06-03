---
title: Fonction fonction cchksgfiles. New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: d18d3ef20890012a1d8c193ec87bdca10a1ed451
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455232"
---
# <a name="cchksgfilesnew-function"></a><span data-ttu-id="28f99-103">Fonction fonction cchksgfiles. New</span><span class="sxs-lookup"><span data-stu-id="28f99-103">CChkSGFiles.New function</span></span>

<span data-ttu-id="28f99-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="28f99-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="28f99-105">Crée une instance de la classe **fonction cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="28f99-105">Creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="28f99-106">Vous devez appeler cette fonction pour pouvoir spécifier le groupe de stockage et les bases de données à vérifier.</span><span class="sxs-lookup"><span data-stu-id="28f99-106">You must call this function before you can specify the storage group and databases to be checked.</span></span> 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a><span data-ttu-id="28f99-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="28f99-107">Parameters</span></span>

<span data-ttu-id="28f99-108">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28f99-108">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="28f99-109">Valeur renvoyée</span><span class="sxs-lookup"><span data-stu-id="28f99-109">Return value</span></span>

<span data-ttu-id="28f99-110">Référence (pointeur) à l’objet nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="28f99-110">A reference (pointer) to the newly created object.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28f99-111">Remarques</span><span class="sxs-lookup"><span data-stu-id="28f99-111">Remarks</span></span>

<span data-ttu-id="28f99-112">La **nouvelle** fonction crée un objet **CCheckSGFiles** et renvoie à l’appelant une référence (pointeur) à cet objet.</span><span class="sxs-lookup"><span data-stu-id="28f99-112">The **New** function creates a **CCheckSGFiles** object and returns to the caller a reference (pointer) to that object.</span></span> <span data-ttu-id="28f99-113">Vous devez appeler cette fonction avant d’appeler une des autres fonctions de la classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="28f99-113">You must call this function before it calls any of the other functions in the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="28f99-114">Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la **nouvelle** fonction dans la partie à thread unique de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="28f99-114">If you're using CHKSGFILES in a multithreaded application, you must call the **New** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="28f99-115">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="28f99-115">Requirements</span></span>

<span data-ttu-id="28f99-116">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="28f99-116">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="28f99-117">Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.</span><span class="sxs-lookup"><span data-stu-id="28f99-117">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

