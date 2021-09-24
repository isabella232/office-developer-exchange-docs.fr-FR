---
title: Validation de l’intégrité de la sauvegarde à l’aide de l’outil Eseutil Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Découvrez comment utiliser l’outil en ligne de commande Eseutil pour valider une sauvegarde de la Exchange store.
ms.openlocfilehash: 0ac994201d1f6c711e5d4d0a3d5835f9bac6e041
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516222"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Validation de l’intégrité de la sauvegarde à l’aide de l’outil Eseutil Exchange 2013

Découvrez comment utiliser l’outil en ligne de commande Eseutil pour valider une sauvegarde de la Exchange store. 
  
**S’applique à :** Exchange Server 2013 
  
Étant donné que le service VSS (Volume Shadow Copy Service) peut créer des sauvegardes alors que Exchange continue d’écrire dans la base de données, le serveur ne touche pas à toutes les pages et n’effectue pas les vérifications de cohérence nécessaires. Pour cette raison, toute application de sauvegarde et de restauration qui utilise VSS doit vérifier la cohérence des captures instantanées. Exchange Server 2013 prend en charge les deux méthodes suivantes pour vérifier la cohérence des captures instantanées : 
  
- The CHKSGFILES API
    
- Outil de ligne de commande Eseutil
    
Nous vous recommandons d’utiliser l’API CHKSGFILES, car il est plus facile pour l’application de sauvegarde de détecter, diagnostiquer et signaler les erreurs détectées lors de la vérification de la cohérence CHKSGFILES. Pour plus d’informations sur l’utilisation de l’API CHKSGFILES, voir Valider l’intégrité de la sauvegarde à l’aide de [l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).
  
## <a name="running-the-eseutil-tool"></a>Exécution de l’outil Eseutil

Pour vérifier la cohérence de la capture instantanée, exécutez la commande eseutil sur la base de données et les fichiers journaux identifiés dans le tableau suivant. 
  
**Tableau 1. Eseutil.exe commandes de sauvegarde pour chaque type de sauvegarde**

|**Type de fichier/type de sauvegarde**|**Sauvegarde complète**|**Copier la sauvegarde**|**Sauvegarde incrémentielle**|**Sauvegarde différentielle**|
|:-----|:-----|:-----|:-----|:-----|
|.edb  <br/> |« eseutil /k /i »  <br/> |« eseutil /k /i »  <br/> |Non applicable  <br/> |Non applicable  <br/> |
|.log  <br/> |« eseutil /k » (1)  <br/> |« eseutil /k » (1)  <br/> |« eseutil /k » (2)  <br/> |« eseutil /k » (2)  <br/> |
   
> [!NOTE]
> Vous n’avez pas besoin d’exécuter la commande eseutil sur les fichiers .stm et .chk. 
  
Tous les fichiers journaux dont le numéro de génération est égal ou supérieur au numéro de génération du fichier journal de point de contrôle sont nécessaires pour récupérer une base de données de capture instantanée. S’il existe, le fichier journal actuel (Enn.log) est également requis pour la récupération de base de données. Si l’un des fichiers journaux requis échoue à la vérification de la cohérence, le demandeur doit s’assurer que l’état du composant de sauvegarde est définie sur FALSE avant d’appeler la méthode [BackupComplete.](https://msdn.microsoft.com/library/windows/desktop/aa382651%28v=vs.85%29.aspx) Pour identifier le fichier journal de point de contrôle, Eseutil.exe le fichier de point de contrôle instantané et l’aperçu de la sortie de « Point de contrôle : ». L’exemple suivant montre comment exécuter des Eseutil.exe un fichier de point de contrôle. 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

La deuxième ligne de l’exemple est la valeur de retour, où 0x20 est le numéro de génération hexadécimal du fichier journal de point de contrôle. Dans cet exemple, tous les fichiers journaux, y compris E01000020.log et supérieur, ne doivent pas être endommagés pour récupérer la base de données de capture instantanée, même si la base de données elle-même a déjà passé la vérification de cohérence physique.
  
Tous les fichiers journaux d’un jeu de sauvegarde incrémentielle ou différentielle sont requis pour la récupération de base de données. Vous pouvez vérifier la cohérence d’une séquence de journaux en exécutant Eseutil.exe par rapport au préfixe du fichier journal. L’exemple suivant montre comment exécuter des vérifications de cohérence sur tous les fichiers du formulaire E01xxxxx.log sur un chemin d’accès donné.
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a>Vérification de la sortie Eseutil.exe de l’enregistrement

Le demandeur doit vérifier que toutes les valeurs d’erreur ERRORLEVEL de sortie renvoyées sont non liées. Pour plus d’informations sur les valeurs ERRORLEVEL, voir [Reference for Common Eseutil Errors](https://technet.microsoft.com/library/aa996759%28v=exchg.80%29.aspx). Pour voir errorLEVEL sur la ligne de commande, tapez « echo %errorlevel% » une fois Eseutil.exe'exécution. Une erreur ERRORLEVEL négative indique qu’un ou plusieurs fichiers sont endommagés.
  
Avant que le demandeur appelle la **méthode BackupComplete,** il doit s’assurer que l’état du composant de sauvegarde reflète le résultat de la vérification de la cohérence. Si une altération a été trouvée, l’état est FALSE ; Si aucune altération n’a été trouvée, l’état est TRUE. 
  
## <a name="see-also"></a>Voir aussi

- [Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

