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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754749"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Valider l’intégrité des sauvegardes en utilisant l’API CHKSGFILES dans Exchange 2013

Découvrez comment utiliser l’API CHKSGFILES pour valider une sauvegarde de la banque d’informations Exchange dans Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
Au cours des opérations de sauvegarde gérées par Volume Shadow Copy Service (VSS), Exchange Server 2013 ne peut pas lire chaque fichier de base de données dans son intégralité et vérifier leur intégrité somme de contrôle. Par conséquent, vous souhaiterez votre application de sauvegarde pour vérifier l’intégrité des fichiers de journal de base de données et des transactions. Il est recommandé que votre application de sauvegarde de vérifier la cohérence physique du jeu de clichés instantanés avant informant l’enregistreur Exchange que la sauvegarde est terminée. Après une sauvegarde réussie, la banque d’informations Exchange met à jour les en-têtes sauvegardées bases de données pour refléter la dernière sauvegarde réussie heures et supprime les journaux de transactions à partir du serveur qui ne sont plus requis pour restaurer par progression à partir de la dernière sauvegarde réussie.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Conditions requises pour la validation de l’intégrité des sauvegardes

Avant que votre application peut valider l’intégrité de la sauvegarde, vous devez avoir accès à ce qui suit :
  
- Fichiers de la sauvegarde de la banque Exchange.
- Une version de Visual Studio commençant par Visual Studio 2010.
- Les fichiers de bibliothèque et d’en-tête CHKSGFILES. Vous pouvez télécharger les fichiers d’en-tête et de bibliothèque à partir du [Centre de téléchargement Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
    
## <a name="validate-backup-integrity"></a>Valider l’intégrité des sauvegardes

La procédure suivante explique comment valider l’intégrité des données dans la sauvegarde et restauration d’application.
  
### <a name="to-validate-backup-integrity"></a>Pour valider l’intégrité des sauvegardes

1. Créer une nouvelle instance de la classe **CChkSGFiles** . 
   
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

   Les premières lignes de code créer un objet error et définissez sa valeur initiale à succès et créer un objet qui vérifie la validité de la base de données. Ensuite, la [fonction CChkSGFiles.New](cchksgfiles-new-function.md) crée une nouvelle instance de la classe **CChkSGFiles** . Une vérification rapide du nouvel objet indique si des problèmes lors de la nouvelle instance a été créée. 
    
2. Initialiser l’objet **CChkSGFiles** . 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Pour plus d’informations sur les paramètres, voir la [fonction CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md).
   
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
   
   Pour plus d’informations sur les paramètres, voir la [fonction CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md).
   
4. Gestion des erreurs et utilisez la [fonction CChkSGFiles.Delete](cchksgfiles-delete-function.md) pour supprimer la classe **CChkSGFiles** de la mémoire. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>Voir aussi

- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Créer la sauvegarde et de restaurer des applications pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

