---
title: Référence de classe CChkSGFiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Recherchez des informations de référence pour l’API CHKSGFILES Exchange 2013.
ms.openlocfilehash: 2daf31c41a47684b85ede196b415884335c3ca79
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510532"
---
# <a name="cchksgfiles-class-reference"></a>Référence de classe CChkSGFiles

Recherchez des informations de référence pour l’API CHKSGFILES Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
L’API CHKSGFILES permet aux applications de sauvegarde et de restauration de vérifier l’intégrité des bases de données et des fichiers journaux de transactions Exchange Server 2013 par programme. Vous pouvez utiliser cette API dans les applications de sauvegarde et de restauration qui utilisent le service VSS (Volume Shadow Copy Service).
  
> [!NOTE]
> Stockage groupes ne sont pas disponibles dans Exchange 2013. La prise en charge des groupes de stockage a été supprimée des versions de Exchange à partir Exchange Server 2010. Pour la compatibilité ascendante avec les bases de données et les groupes de stockage dans les versions de Exchange antérieures à Exchange 2010, l’API CHKSGFILES vous permet de spécifier des groupes de stockage. Lorsque vous exécutez CHKSGFILES sur des bases de données Exchange 2013, vous devez définir des paramètres qui spécifient un identificateur de groupe de stockage sur une chaîne vide. 
  
## <a name="file-location"></a>Emplacement du fichier
<a name="bk_fileslocation"> </a>

L’API CHKSGFILES est Exchange 2013. Vous pouvez utiliser cette API sur un ordinateur sur qui le rôle serveur de boîtes aux lettres est installé. 
  
Par défaut, la DLL CHKSGFILES est installée dans le répertoire C:\Program Files\Microsoft\Exchange\V15\Bin.
  
Exchange 2013 inclut uniquement une version 64 bits (amd64) de l’API CHKSGFILES. 
  
Vous pouvez télécharger un fichier .zip qui inclut la bibliothèque CHKSGFILE.lib et les fichiers d’en-tête CHKSGFILES.hxx à utiliser dans votre application personnalisée à partir du Centre de téléchargement [Microsoft.](https://www.microsoft.com/download/details.aspx?id=36802)
  
## <a name="development-languages"></a>Langages de développement
<a name="bk_developmentlanguages"> </a>

L’API CHKSGFILES est conçue pour une utilisation avec des versions de Visual Studio à partir de Visual Studio 2005 en C/C++ natif. L’API CHKSGFILES n’est pas destinée à être utilisé dans le code géré. Bien que vous pouvez créer un assembly COM Interop avec CHKSGFILES, nous n’expédions pas un assembly COM Interop pris en charge avec Exchange 2013.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Fonction CChkSGFiles.CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Fonction CChkSGFiles.Delete](cchksgfiles-delete-function.md)
    
- [Énumération CChkSGFiles.ERR](cchksgfiles-err-enumeration.md)
    
- [Fonction CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Fonction CChkSGFiles.ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Fonction CChkSGFiles.ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Fonction CChkSGFiles.ErrGetHeader (réservé)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Fonction CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)
    
- [Fonction CChkSGFiles.ErrTerm](cchksgfiles-errterm-function.md)
    
- [Énumération CChkSGFiles.iDbInvalid](cchksgfiles-idbinvalid-enumeration.md)
    
- [Fonction CChkSGFiles.New](cchksgfiles-new-function.md)
    
- [Énumération CChkSGFiles.NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [Structure CChkSGFiles.PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Fonction CChkSGFiles.PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>Voir aussi

- [Développement d’Exchange et Exchange Online](../exchange-server-development.md)
- [Sauvegarde, restauration et récupération d’urgence](https://technet.microsoft.com/library/dd876874)
    

