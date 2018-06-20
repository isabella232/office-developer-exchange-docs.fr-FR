---
title: Valider l’intégrité des sauvegardes à l’aide l’outil Eseutil dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Découvrez comment utiliser l’outil de ligne de commande Eseutil pour valider une sauvegarde de la banque d’informations Exchange.
ms.openlocfilehash: 03c4c23d433418911240bbe7c337308a989f3739
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754741"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Valider l’intégrité des sauvegardes à l’aide l’outil Eseutil dans Exchange 2013

Découvrez comment utiliser l’outil de ligne de commande Eseutil pour valider une sauvegarde de la banque d’informations Exchange. 
  
**S’applique à :** Exchange Server 2013 
  
Étant donné que le Volume Shadow Copy Service (VSS) peut créer des sauvegardes pendant que Exchange continue à écrire dans la base de données, le serveur ne pas toutes les pages et effectuer les vérifications de cohérence nécessaires. Pour cette raison, n’importe quelle application de sauvegarde et de restauration qui utilise le service VSS doit vérifier la cohérence de la capture instantanée. Exchange Server 2013 prend en charge les deux méthodes suivantes pour la vérification de cohérence de la capture instantanée : 
  
- L’API CHKSGFILES
    
- L’outil de ligne de commande Eseutil
    
Nous vous recommandons d’utiliser l’API CHKSGFILES, car il est plus facile pour l’application de sauvegarde détecter, diagnostiquer et signaler les erreurs rencontrées lors de la cohérence CHKSGFILES vérifier. Pour plus d’informations sur la façon d’utiliser l’API CHKSGFILES, voir [l’intégrité des sauvegardes de valider en utilisant l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).
  
## <a name="running-the-eseutil-tool"></a>Exécution de l’outil Eseutil

Pour vérifier la cohérence de la capture instantanée, exécutez la commande eseutil par rapport aux base de données et les fichiers journaux qui sont identifiés dans le tableau suivant. 
  
**Le tableau 1. Commandes Eseutil.exe pour chaque type de sauvegarde**

|**Type de sauvegarde/de type de fichier**|**Sauvegarde complète**|**Copie de sauvegarde**|**Sauvegarde incrémentielle**|**Sauvegarde différentielle**|
|:-----|:-----|:-----|:-----|:-----|
|.edb  <br/> |« eseutil /k /i »  <br/> |« eseutil /k /i »  <br/> |Not applicable  <br/> |Not applicable  <br/> |
|.log  <br/> |« eseutil /k » (1)  <br/> |« eseutil /k » (1)  <br/> |« eseutil /k » (2)  <br/> |« eseutil /k » (2)  <br/> |
   
> [!NOTE]
> Il est inutile d’exécuter la commande eseutil sur les fichiers .stm et .chk. 
  
Tous les fichiers journaux qui ont une génération du fichier journal numéro qui est égale ou supérieure à la génération du numéro du fichier journal au point de contrôle sont requis afin de récupérer une base de données de capture instantanée. S’il existe, le fichier journal actuel (Enn.log) est également requis pour la récupération de la base de données. Si un des fichiers journaux requis échoue la vérification de cohérence, le demandeur devez vous assurer que l’état du composant de sauvegarde est défini sur FALSE avant d’appeler la méthode [BackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382651%28v=vs.85%29.aspx) . Pour identifier le fichier journal de point de contrôle, exécutez Eseutil.exe sur le fichier de point de contrôle de capture instantanée et analyser la sortie pour » au point de contrôle :. » L’exemple suivant montre comment exécuter Eseutil.exe sur un fichier de point de contrôle. 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

La deuxième ligne dans l’exemple est la valeur de retour, où 0 x 20 est le numéro de génération de journal hexadécimal du fichier journal au point de contrôle. Dans cet exemple, les fichiers journaux, y compris E01000020.log et supérieur, doit n'être pas endommagé afin de récupérer la base de données de capture instantanée, même si la base de données est déjà passée la vérification de cohérence physique.
  
Tous les fichiers journaux dans un jeu de sauvegarde incrémentiel ou différentiel sont requis pour la récupération de base de données. Vous pouvez vérifier la cohérence d’une séquence de journal en exécutant Eseutil.exe sur le préfixe du fichier journal. L’exemple suivant montre comment exécuter les vérifications de cohérence sur tous les fichiers au format E01xxxxx.log sur un chemin d’accès donné.
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a>Vérification de la sortie Eseutil.exe

Le demandeur doit vérifier que toutes les quitter niveau d’erreur Erreur valeurs renvoyées sont non négatifs. Pour plus d’informations sur les valeurs de niveau d’erreur, voir [référence des erreurs courantes de Eseutil](http://technet.microsoft.com/en-us/library/aa996759%28v=exchg.80%29.aspx). Pour afficher le niveau d’erreur à la ligne de commande, tapez « echo %errorlevel% » après la fin de Eseutil.exe. Un niveau d’erreur négative indique qu’un ou plusieurs fichiers est endommagé.
  
Avant le demandeur appelle la méthode **BackupComplete** , il doit Assurez-vous que l’état du composant de sauvegarde reflète le résultat de la vérification de cohérence. Si toute corruption a été trouvée, l’état sera FALSE ; Si aucune corruption a été trouvée, l’état est TRUE. 
  
## <a name="see-also"></a>Voir aussi

- [Valider l’intégrité des sauvegardes en utilisant l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [Créer la sauvegarde et de restaurer des applications pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

