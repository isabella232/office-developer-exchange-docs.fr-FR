---
title: Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde du magasin Exchange dans Exchange 2013.
ms.openlocfilehash: 7a12a0a8f66128970a782da50ba59f41767c60d3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516229"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES Exchange 2013

Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde du magasin Exchange dans Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Lors des opérations de sauvegarde gérées par le service VSS (Volume Shadow Copy Service), Exchange Server 2013 ne peut pas lire chaque fichier de base de données dans son intégralité et vérifier son intégrité de sommes de contrôle. Par conséquent, vous souhaitez peut-être que votre application de sauvegarde vérifie l’intégrité de la base de données et du fichier journal des transactions. Il est recommandé que votre application de sauvegarde vérifie la cohérence physique du jeu de copies de secours avant d’informer le rédacteur Exchange que la sauvegarde est terminée. Après une sauvegarde réussie, la banque d’informations Exchange met à jour les en-têtes des bases de données de sauvegarde pour refléter les dernières sauvegardes réussies et supprime les journaux de transactions du serveur qui ne sont plus nécessaires à l’avance à partir de la dernière sauvegarde réussie.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Conditions préalables à la validation de l’intégrité de la sauvegarde

Avant que votre application puisse valider l’intégrité de votre sauvegarde, vous devez avoir accès aux informations suivantes :
  
- Les fichiers de votre Exchange de sauvegarde.
- Une version de Visual Studio à partir de Visual Studio 2010.
- La bibliothèque CHKSGFILES et les fichiers d’en-tête. Vous pouvez télécharger la bibliothèque et les fichiers d’en-tête à partir du [Centre de téléchargement Microsoft.](https://www.microsoft.com/download/details.aspx?id=36802)
    
## <a name="validate-backup-integrity"></a>Valider l’intégrité de la sauvegarde

La procédure suivante décrit comment valider l’intégrité des données dans votre application de sauvegarde et de restauration.
  
### <a name="to-validate-backup-integrity"></a>Pour valider l’intégrité de la sauvegarde

1. Créez une instance de la **classe CChkSGFiles.** 
   
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

   Les premières lignes de code créent un objet d’erreur et définissent sa valeur initiale sur succès, et créent un objet qui vérifie la validité de la base de données. Ensuite, la [fonction CChkSGFiles.New](cchksgfiles-new-function.md) crée une instance de la classe **CChkSGFiles.** Une vérification rapide du nouvel objet indique si des problèmes se sont produits lors de la création de la nouvelle instance. 
    
2. Initialiser **l’objet CChkSGFiles.** 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Pour plus d’informations sur les paramètres, voir la fonction [CChkSGFiles.ErrInit.](cchksgfiles-errinit-function.md)
   
3. Utilisez la [fonction CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) pour valider l’intégrité de la base de données en vérifiant les en-têtes de base de données.
   
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
   
   Pour plus d’informations sur les paramètres, voir la fonction [CChkSGFiles.ErrCheckDbHeaders.](cchksgfiles-errcheckdbheaders-function.md)
   
4. Gérer les erreurs et utiliser la [fonction CChkSGFiles.Delete](cchksgfiles-delete-function.md) pour supprimer la classe **CChkSGFiles** de la mémoire. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>Voir aussi

- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

