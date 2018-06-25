---
title: Valider l’intégrité des sauvegardes en utilisant l’API CHKSGFILES dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde de la banque d’informations Exchange dans Exchange 2013.
ms.openlocfilehash: 968484cd5bb7439730685643683e1d850bec33ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754749"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="8f9d3-103">Valider l’intégrité des sauvegardes en utilisant l’API CHKSGFILES dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8f9d3-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="8f9d3-104">Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde de la banque d’informations Exchange dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="8f9d3-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8f9d3-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="8f9d3-106">Au cours des opérations de sauvegarde gérées par Volume Shadow Copy Service (VSS), Exchange Server 2013 ne peut pas lire chaque fichier de base de données dans son intégralité et vérifier leur intégrité somme de contrôle.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="8f9d3-107">Par conséquent, vous souhaiterez votre application de sauvegarde pour vérifier l’intégrité des fichiers de journal de base de données et des transactions.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="8f9d3-108">Il est recommandé que votre application de sauvegarde de vérifier la cohérence physique du jeu de clichés instantanés avant informant l’enregistreur Exchange que la sauvegarde est terminée.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="8f9d3-109">Après une sauvegarde réussie, la banque d’informations Exchange met à jour les en-têtes sauvegardées bases de données pour refléter la dernière sauvegarde réussie heures et supprime les journaux de transactions à partir du serveur qui ne sont plus requis pour restaurer par progression à partir de la dernière sauvegarde réussie.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="8f9d3-110">Conditions requises pour la validation de l’intégrité des sauvegardes</span><span class="sxs-lookup"><span data-stu-id="8f9d3-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="8f9d3-111">Avant que votre application peut valider l’intégrité de la sauvegarde, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="8f9d3-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="8f9d3-112">Fichiers de la sauvegarde de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="8f9d3-113">Une version de Visual Studio commençant par Visual Studio 2010.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="8f9d3-114">Les fichiers de bibliothèque et d’en-tête CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="8f9d3-115">Vous pouvez télécharger les fichiers d’en-tête et de bibliothèque à partir du [Centre de téléchargement Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="8f9d3-115">You can download the library and header files from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="8f9d3-116">Valider l’intégrité des sauvegardes</span><span class="sxs-lookup"><span data-stu-id="8f9d3-116">Validate backup integrity</span></span>

<span data-ttu-id="8f9d3-117">La procédure suivante explique comment valider l’intégrité des données dans la sauvegarde et restauration d’application.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="8f9d3-118">Pour valider l’intégrité des sauvegardes</span><span class="sxs-lookup"><span data-stu-id="8f9d3-118">To validate backup integrity</span></span>

1. <span data-ttu-id="8f9d3-119">Créer une nouvelle instance de la classe **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="8f9d3-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
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

   <span data-ttu-id="8f9d3-120">Les premières lignes de code créer un objet error et définissez sa valeur initiale à succès et créer un objet qui vérifie la validité de la base de données.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="8f9d3-121">Ensuite, la [fonction CChkSGFiles.New](cchksgfiles-new-function.md) crée une nouvelle instance de la classe **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="8f9d3-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="8f9d3-122">Une vérification rapide du nouvel objet indique si des problèmes lors de la nouvelle instance a été créée.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="8f9d3-123">Initialiser l’objet **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="8f9d3-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="8f9d3-124">Pour plus d’informations sur les paramètres, voir la [fonction CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md).</span><span class="sxs-lookup"><span data-stu-id="8f9d3-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="8f9d3-125">Utilisez la [fonction CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) pour valider l’intégrité de la base de données en vérifiant les en-têtes de base de données.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
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
   
   <span data-ttu-id="8f9d3-126">Pour plus d’informations sur les paramètres, voir la [fonction CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).</span><span class="sxs-lookup"><span data-stu-id="8f9d3-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="8f9d3-127">Gestion des erreurs et utilisez la [fonction CChkSGFiles.Delete](cchksgfiles-delete-function.md) pour supprimer la classe **CChkSGFiles** de la mémoire.</span><span class="sxs-lookup"><span data-stu-id="8f9d3-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="8f9d3-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8f9d3-128">See also</span></span>

- [<span data-ttu-id="8f9d3-129">Référence de classe CChkSGFiles</span><span class="sxs-lookup"><span data-stu-id="8f9d3-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="8f9d3-130">Créer la sauvegarde et de restaurer des applications pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8f9d3-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="8f9d3-131">Concepts de sauvegarde et de restauration pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8f9d3-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

