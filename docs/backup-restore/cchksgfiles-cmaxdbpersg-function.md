---
title: Fonction fonction cchksgfiles. CMaxDbPerSG
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: b7c3517779eb07ef053c1dd4fa25544310fb3343
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455260"
---
# <a name="cchksgfilescmaxdbpersg-function"></a><span data-ttu-id="c867c-103">Fonction fonction cchksgfiles. CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="c867c-103">CChkSGFiles.CMaxDbPerSG function</span></span>

<span data-ttu-id="c867c-104">**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="c867c-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="c867c-105">Renvoie le nombre maximal de bases de données autorisées dans un seul groupe de stockage Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="c867c-105">Returns the maximum number of databases allowed in a single Exchange server storage group.</span></span>
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a><span data-ttu-id="c867c-106">Paramètres</span><span class="sxs-lookup"><span data-stu-id="c867c-106">Parameters</span></span>

<span data-ttu-id="c867c-107">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c867c-107">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="c867c-108">Valeur renvoyée</span><span class="sxs-lookup"><span data-stu-id="c867c-108">Return value</span></span>

<span data-ttu-id="c867c-109">Nombre maximal de bases de données que le serveur Exchange Server spécifié autorise par groupe de stockage.</span><span class="sxs-lookup"><span data-stu-id="c867c-109">The maximum number of databases that the specified Exchange server allows per storage group.</span></span> <span data-ttu-id="c867c-110">Étant donné que les groupes de stockage ne font pas partie d’Exchange 2013, cette fonction renvoie la valeur 1.</span><span class="sxs-lookup"><span data-stu-id="c867c-110">Because storage groups are not part of Exchange 2013, this function returns 1.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c867c-111">Remarques</span><span class="sxs-lookup"><span data-stu-id="c867c-111">Remarks</span></span>

<span data-ttu-id="c867c-112">Vous pouvez utiliser l’objet **CCheckSGFiles** pour valider des bases de données (et des fichiers journaux de transactions) dans un seul groupe de stockage, afin que la valeur renvoyée par la fonction **CMaxDbPerSG** représente également le nombre maximal de bases de données que vous pouvez vérifier à l’aide d’une instance de la classe **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="c867c-112">You can use the **CCheckSGFiles** object to validate databases (and transaction log files) in only one storage group, so the value returned by the **CMaxDbPerSG** function also represents the maximum number of databases that you can check by using an instance of the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="c867c-113">Notez que, par défaut, Exchange Server 2003 et Exchange Server 2007 autorisent un maximum de cinq bases de données par groupe de stockage.</span><span class="sxs-lookup"><span data-stu-id="c867c-113">Note that by default, Exchange Server 2003 and Exchange Server 2007 allow a maximum of five databases per storage group.</span></span>
  
## <a name="requirements"></a><span data-ttu-id="c867c-114">Configuration requise</span><span class="sxs-lookup"><span data-stu-id="c867c-114">Requirements</span></span>

<span data-ttu-id="c867c-115">Exchange 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="c867c-115">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="c867c-116">Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.</span><span class="sxs-lookup"><span data-stu-id="c867c-116">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

