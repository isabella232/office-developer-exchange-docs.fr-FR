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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452859"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013

Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde de la Banque d’informations Exchange dans Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Pendant les opérations de sauvegarde gérées par le service VSS (Volume Shadow Copy Service), Exchange Server 2013 ne peut pas lire chaque fichier de base de données dans son intégralité et vérifier son intégrité. Par conséquent, vous souhaiterez peut-être que votre application de sauvegarde vérifie l’intégrité du fichier journal des transactions et de la base de données. Il est recommandé que votre application de sauvegarde vérifie la cohérence physique du jeu de clichés instantanés avant d’informer le rédacteur Exchange que la sauvegarde est terminée. Après une sauvegarde réussie, la Banque d’Exchange met à jour les en-têtes des bases de données sauvegardées afin de refléter les dernières heures de sauvegarde et de suppression des journaux de transaction du serveur qui ne sont plus nécessaires pour effectuer une reprise à partir de la dernière sauvegarde réussie.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Conditions préalables à la validation de l’intégrité de la sauvegarde

Pour que votre application puisse valider l’intégrité de votre sauvegarde, vous devez avoir accès à ce qui suit :
  
- Fichiers à partir de votre sauvegarde de banque Exchange.
- Une version de Visual Studio à partir de Visual Studio 2010.
- La bibliothèque CHKSGFILES et les fichiers d’en-tête. Vous pouvez télécharger les fichiers de bibliothèque et d’en-tête à partir du [Centre de téléchargement Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).
    
## <a name="validate-backup-integrity"></a>Valider l’intégrité de la sauvegarde

La procédure suivante explique comment valider l’intégrité des données dans votre application de sauvegarde et de restauration.
  
### <a name="to-validate-backup-integrity"></a>Pour valider l’intégrité de la sauvegarde

1. Créez une instance de la classe **fonction cchksgfiles** . 
   
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

   Les premières lignes de code créent un objet Error et définissent sa valeur initiale sur Success, et créent un objet qui vérifie la validité de la base de données. Ensuite, la [fonction fonction cchksgfiles. New](cchksgfiles-new-function.md) crée une nouvelle instance de la classe **fonction cchksgfiles** Une vérification rapide du nouvel objet indique si des problèmes ont eu lieu lors de la création de la nouvelle instance. 
    
2. Initialisez l’objet **fonction cchksgfiles** . 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Pour plus d’informations sur les paramètres, reportez-vous à la [fonction fonction cchksgfiles. ErrInit](cchksgfiles-errinit-function.md).
   
3. Utilisez la [fonction fonction cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) pour valider l’intégrité de la base de données en vérifiant les en-têtes de la base de données.
   
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
   
   Pour plus d’informations sur les paramètres, reportez-vous à la [fonction fonction cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).
   
4. Gérez les erreurs et utilisez la [fonction fonction cchksgfiles. Delete](cchksgfiles-delete-function.md) pour supprimer la classe **fonction cchksgfiles** de la mémoire. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>Voir aussi

- [Référence de classe fonction cchksgfiles](cchksgfiles-class-reference.md)
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

