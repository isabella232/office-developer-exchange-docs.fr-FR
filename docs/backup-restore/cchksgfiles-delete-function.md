---
title: Fonction CChkSGFiles.Delete
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
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754746"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="0eea2-103">Fonction CChkSGFiles.Delete</span><span class="sxs-lookup"><span data-stu-id="0eea2-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="0eea2-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0eea2-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="0eea2-105">Détruit une instance existante de la classe **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0eea2-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="0eea2-106">Vous devez appeler cette fonction après que l’application a terminé l’utilisation de l’objet spécifié.</span><span class="sxs-lookup"><span data-stu-id="0eea2-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="0eea2-107">Paramètres</span><span class="sxs-lookup"><span data-stu-id="0eea2-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="0eea2-108">pcchecksgfiles</span><span class="sxs-lookup"><span data-stu-id="0eea2-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="0eea2-109">Paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="0eea2-109">Input parameter.</span></span> <span data-ttu-id="0eea2-110">Pointeur vers un objet **CCheckSGFiles** existant.</span><span class="sxs-lookup"><span data-stu-id="0eea2-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="0eea2-111">La mémoire associée à l’objet puis sera libérée.</span><span class="sxs-lookup"><span data-stu-id="0eea2-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="0eea2-112">Valeur renvoyée</span><span class="sxs-lookup"><span data-stu-id="0eea2-112">Return value</span></span>

<span data-ttu-id="0eea2-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0eea2-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0eea2-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="0eea2-114">Remarks</span></span>

<span data-ttu-id="0eea2-115">La fonction **Supprimer** libère la mémoire associée à l’objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0eea2-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="0eea2-116">Une fois que vous appelez **Delete**, le pointeur passé dans le paramètre *pcchecksgfiles* n’est pas valide et aucune autre opération ne peut être effectuées sur cet objet.</span><span class="sxs-lookup"><span data-stu-id="0eea2-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="0eea2-117">Si l’application utilise la fonction **ErrCheckDbPages** , l’application doit libérer la mémoire tampon manuellement. la fonction **Supprimer** sera libère pas.</span><span class="sxs-lookup"><span data-stu-id="0eea2-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="0eea2-118">Si vous utilisez CHKSGFILES dans une application multithread, vous devez appeler la fonction **Supprimer** dans la partie d’un seul thread de l’application, et vous pouvez l’appeler qu’une seule fois pour chaque objet **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="0eea2-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="0eea2-119">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="0eea2-119">Requirements</span></span>

<span data-ttu-id="0eea2-120">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="0eea2-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="0eea2-121">Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.</span><span class="sxs-lookup"><span data-stu-id="0eea2-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

