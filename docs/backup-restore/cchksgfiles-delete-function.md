---
title: Fonction fonction cchksgfiles. Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 38cb72b42727855f652de607bb2a02ecdeaae16e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44447049"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="99bc8-103">Fonction fonction cchksgfiles. Delete</span><span class="sxs-lookup"><span data-stu-id="99bc8-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="99bc8-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="99bc8-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="99bc8-105">Détruit une instance existante de la classe **fonction cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="99bc8-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="99bc8-106">Vous devez appeler cette fonction une fois que l’application a fini de travailler avec l’objet spécifié.</span><span class="sxs-lookup"><span data-stu-id="99bc8-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="99bc8-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="99bc8-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="99bc8-108">pcchecksgfiles</span><span class="sxs-lookup"><span data-stu-id="99bc8-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="99bc8-109">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="99bc8-109">Input parameter.</span></span> <span data-ttu-id="99bc8-110">Pointeur vers un objet **CCheckSGFiles** existant.</span><span class="sxs-lookup"><span data-stu-id="99bc8-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="99bc8-111">La mémoire associée à l’objet sera ensuite libérée.</span><span class="sxs-lookup"><span data-stu-id="99bc8-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="99bc8-112">Valeur renvoyée</span><span class="sxs-lookup"><span data-stu-id="99bc8-112">Return value</span></span>

<span data-ttu-id="99bc8-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="99bc8-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="99bc8-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="99bc8-114">Remarks</span></span>

<span data-ttu-id="99bc8-115">La fonction **Delete** libère la mémoire associée à l’objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="99bc8-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="99bc8-116">Une fois que vous avez appelé **Delete**, le pointeur transmis dans le paramètre *pcchecksgfiles* n’est pas valide et aucune autre opération ne peut être effectuée sur cet objet.</span><span class="sxs-lookup"><span data-stu-id="99bc8-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="99bc8-117">Si l’application utilise la fonction **ErrCheckDbPages** , l’application doit libérer la mémoire tampon manuellement ; la fonction **Delete** ne la libère pas.</span><span class="sxs-lookup"><span data-stu-id="99bc8-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="99bc8-118">Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **Delete** dans la partie à thread unique de l’application, et vous ne pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="99bc8-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="99bc8-119">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="99bc8-119">Requirements</span></span>

<span data-ttu-id="99bc8-120">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="99bc8-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="99bc8-121">Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.</span><span class="sxs-lookup"><span data-stu-id="99bc8-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

