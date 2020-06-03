---
title: Valider l’intégrité de la sauvegarde à l’aide de l’outil Eseutil dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0d325ba-4482-4ca2-9a69-c890f985b206
description: Découvrez comment utiliser l’outil de ligne de commande Eseutil pour valider une sauvegarde de la Banque d’informations Exchange.
ms.openlocfilehash: e8f1a46e2d94729ae5586861317312e277216d63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452796"
---
#  <a name="validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013"></a>Valider l’intégrité de la sauvegarde à l’aide de l’outil Eseutil dans Exchange 2013

Découvrez comment utiliser l’outil de ligne de commande Eseutil pour valider une sauvegarde de la Banque d’informations Exchange. 
  
**S’applique à :** Exchange Server 2013 
  
Étant donné que le service VSS (Volume Shadow Copy Service) peut créer des sauvegardes alors qu’Exchange continue d’écrire dans la base de données, le serveur ne touche pas toutes les pages et effectue les vérifications de cohérence nécessaires. Pour cette raison, toute application de sauvegarde et de restauration qui utilise VSS doit vérifier la cohérence de capture instantanée. Exchange Server 2013 prend en charge les deux méthodes suivantes pour vérifier la cohérence des captures instantanées : 
  
- API CHKSGFILES
    
- Outil de ligne de commande Eseutil
    
Nous vous recommandons d’utiliser l’API CHKSGFILES, car il est plus facile pour l’application de sauvegarde de détecter, de diagnostiquer et de signaler les erreurs détectées lors de la vérification de cohérence CHKSGFILES. Pour plus d’informations sur l’utilisation de l’API CHKSGFILES, consultez la rubrique validation de l' [intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).
  
## <a name="running-the-eseutil-tool"></a>Exécution de l’outil Eseutil

Pour vérifier la cohérence des captures instantanées, exécutez la commande Eseutil sur la base de données et les fichiers journaux identifiés dans le tableau suivant. 
  
**Tableau 1. Commandes Eseutil. exe pour chaque type de sauvegarde**

|**Type de fichier/type de sauvegarde**|**Sauvegarde complète**|**Copie de sauvegarde**|**Sauvegarde incrémentielle**|**Sauvegarde différentielle**|
|:-----|:-----|:-----|:-----|:-----|
|. edb  <br/> |"Eseutil/k/i"  <br/> |"Eseutil/k/i"  <br/> |Non applicable  <br/> |Non applicable  <br/> |
|. log  <br/> |« Eseutil/k » (1)  <br/> |« Eseutil/k » (1)  <br/> |"Eseutil/k" (2)  <br/> |"Eseutil/k" (2)  <br/> |
   
> [!NOTE]
> Vous n’avez pas besoin d’exécuter la commande Eseutil sur les fichiers. stm et. chk. 
  
Tous les fichiers journaux dont le numéro de génération est supérieur ou égal au numéro de génération du fichier journal de point de contrôle sont requis afin de récupérer une base de données de captures instantanées. S’il existe, le fichier journal actuel (Enn. log) est également requis pour la récupération de la base de données. Si l’un des fichiers journaux requis échoue à la vérification de cohérence, le demandeur doit s’assurer que l’état du composant de sauvegarde est défini sur FALSe avant d’appeler la méthode [BackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa382651%28v=vs.85%29.aspx) . Pour identifier le fichier journal de point de contrôle, exécutez Eseutil. exe sur le fichier de point de contrôle de capture instantanée et analysez la sortie pour « point de contrôle : ». L’exemple suivant montre comment exécuter Eseutil. exe avec un fichier de point de contrôle. 
  
```cpp
c:\eseutil.exe /mk E01.chk
Checkpoint: (0x20, 9D, 187)
```

La deuxième ligne de l’exemple est la valeur renvoyée, où 0x20 est le numéro de génération de journal hexadécimal du fichier journal de point de contrôle. Dans cet exemple, tous les fichiers journaux, y compris E01000020. log et supérieur, ne doivent pas être endommagés afin de récupérer la base de données de capture instantanée, même si la base de données elle-même a déjà passé la vérification de cohérence physique.
  
Tous les fichiers journaux d’un jeu de sauvegarde incrémentielle ou différentiel sont requis pour la récupération de la base de données. Vous pouvez vérifier la cohérence d’une séquence de journal en exécutant eseutil. exe avec le préfixe du fichier journal. L’exemple suivant montre comment exécuter des vérifications de cohérence sur tous les fichiers au format E01xxxxx. log sur un chemin d’accès donné.
  
```cpp
c:\eseutil /k E01
```

## <a name="checking-the-eseutilexe-output"></a>Vérification de la sortie d’Eseutil. exe

Le demandeur doit vérifier que toutes les valeurs d’erreur de sortie ERRORLEVEL renvoyées sont non négatives. Pour plus d’informations sur les valeurs ERRORLEVEL, voir [Reference for Common Eseutil Errors](https://technet.microsoft.com/library/aa996759%28v=exchg.80%29.aspx). Pour afficher le ERRORLEVEL à partir de la ligne de commande, tapez « echo% errorlevel% » une fois l’exécution de Eseutil. exe terminée. Un ERRORLEVEL négatif indique qu’un ou plusieurs fichiers sont endommagés.
  
Avant que le demandeur appelle la méthode **BackupComplete** , il doit s’assurer que l’état du composant de sauvegarde reflète le résultat de la vérification de cohérence. Si une corruption a été détectée, l’État prend la valeur FALSe ; Si aucune altération n’a été détectée, l’État est TRUE. 
  
## <a name="see-also"></a>Voir aussi

- [Valider l’intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Référence de classe fonction cchksgfiles](cchksgfiles-class-reference.md)
- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

