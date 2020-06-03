---
title: Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde de la Banque d’informations Exchange dans Exchange 2013.
ms.openlocfilehash: c101413793cf3b952d3db3e0f792c8bcf2dd9fc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452859"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="bd6d8-103">Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="bd6d8-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="bd6d8-104">Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde de la Banque d’informations Exchange dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="bd6d8-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="bd6d8-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="bd6d8-106">Pendant les opérations de sauvegarde gérées par le service VSS (Volume Shadow Copy Service), Exchange Server 2013 ne peut pas lire chaque fichier de base de données dans son intégralité et vérifier son intégrité.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="bd6d8-107">Par conséquent, vous souhaiterez peut-être que votre application de sauvegarde vérifie l’intégrité du fichier journal des transactions et de la base de données.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="bd6d8-108">Il est recommandé que votre application de sauvegarde vérifie la cohérence physique du jeu de clichés instantanés avant d’informer le rédacteur Exchange que la sauvegarde est terminée.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="bd6d8-109">Après une sauvegarde réussie, la Banque d’Exchange met à jour les en-têtes des bases de données sauvegardées afin de refléter les dernières heures de sauvegarde et de suppression des journaux de transaction du serveur qui ne sont plus nécessaires pour effectuer une reprise à partir de la dernière sauvegarde réussie.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="bd6d8-110">Conditions préalables à la validation de l’intégrité de la sauvegarde</span><span class="sxs-lookup"><span data-stu-id="bd6d8-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="bd6d8-111">Pour que votre application puisse valider l’intégrité de votre sauvegarde, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="bd6d8-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="bd6d8-112">Fichiers à partir de votre sauvegarde de banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="bd6d8-113">Une version de Visual Studio à partir de Visual Studio 2010.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="bd6d8-114">La bibliothèque CHKSGFILES et les fichiers d’en-tête.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="bd6d8-115">Vous pouvez télécharger les fichiers de bibliothèque et d’en-tête à partir du [Centre de téléchargement Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="bd6d8-115">You can download the library and header files from the [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="bd6d8-116">Valider l’intégrité de la sauvegarde</span><span class="sxs-lookup"><span data-stu-id="bd6d8-116">Validate backup integrity</span></span>

<span data-ttu-id="bd6d8-117">La procédure suivante explique comment valider l’intégrité des données dans votre application de sauvegarde et de restauration.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="bd6d8-118">Pour valider l’intégrité de la sauvegarde</span><span class="sxs-lookup"><span data-stu-id="bd6d8-118">To validate backup integrity</span></span>

1. <span data-ttu-id="bd6d8-119">Créez une instance de la classe **fonction cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="bd6d8-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
   ```cpp
   CCheckSGFiles::ERRerr = CCheckSGFiles::errSuccess;
   ULONGiDbError = (ULONG)CCheckSGFiles::iDbInvalid;
   CCheckSGFiles * const pcchecksgfiles = CCheckSGFiles::New();
   if ( NULL == pcchecksgfiles )
   {
     err = CCheckSGFiles::errOutOfMemory;
     printf( "ERROR: Could not allocate CCheckSGFiles object.\n" );
     goto HandleError;
   }
   ```

   <span data-ttu-id="bd6d8-120">Les premières lignes de code créent un objet Error et définissent sa valeur initiale sur Success, et créent un objet qui vérifie la validité de la base de données.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="bd6d8-121">Ensuite, la [fonction fonction cchksgfiles. New](cchksgfiles-new-function.md) crée une nouvelle instance de la classe **fonction cchksgfiles**</span><span class="sxs-lookup"><span data-stu-id="bd6d8-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="bd6d8-122">Une vérification rapide du nouvel objet indique si des problèmes ont eu lieu lors de la création de la nouvelle instance.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="bd6d8-123">Initialisez l’objet **fonction cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="bd6d8-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="bd6d8-124">Pour plus d’informations sur les paramètres, reportez-vous à la [fonction fonction cchksgfiles. ErrInit](cchksgfiles-errinit-function.md).</span><span class="sxs-lookup"><span data-stu-id="bd6d8-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="bd6d8-125">Utilisez la [fonction fonction cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) pour valider l’intégrité de la base de données en vérifiant les en-têtes de la base de données.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
   ```cpp
   err = pcchecksgfiles->ErrCheckDbHeaders(
   &amp;cbDbPageSize,
   &amp;cDbHeaderPages,
   &amp;iDbError );
   if ( CCheckSGFiles::errSuccess != err )
   {
   if ( CCheckSGFiles::iDbInvalid != iDbError )
   {
   printf(
   "ERROR: Database header validation for '%S' failed with error %d (0x%x)\n",
   rgwszDb[ iDbError ],
   err,
   err );
   }
   goto HandleError;
   }
   ```
   
   <span data-ttu-id="bd6d8-126">Pour plus d’informations sur les paramètres, reportez-vous à la [fonction fonction cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).</span><span class="sxs-lookup"><span data-stu-id="bd6d8-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="bd6d8-127">Gérez les erreurs et utilisez la [fonction fonction cchksgfiles. Delete](cchksgfiles-delete-function.md) pour supprimer la classe **fonction cchksgfiles** de la mémoire.</span><span class="sxs-lookup"><span data-stu-id="bd6d8-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="bd6d8-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd6d8-128">See also</span></span>

- [<span data-ttu-id="bd6d8-129">Référence de classe fonction cchksgfiles</span><span class="sxs-lookup"><span data-stu-id="bd6d8-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="bd6d8-130">Créer des applications de sauvegarde et de restauration pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="bd6d8-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="bd6d8-131">Concepts de sauvegarde et de restauration pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="bd6d8-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

