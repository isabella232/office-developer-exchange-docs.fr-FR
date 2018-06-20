---
title: Référence de classe CChkSGFiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Trouvez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.
ms.openlocfilehash: 583ac5e16ab60d119c3028bf81123e9f60a58ff4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754747"
---
# <a name="cchksgfiles-class-reference"></a>Référence de classe CChkSGFiles

Trouvez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
L’API CHKSGFILES permet aux applications de sauvegarde et de restauration vérifier l’intégrité des fichiers journaux des transactions Exchange Server 2013 et des bases de données par programme. Vous pouvez utiliser cette API de sauvegarde et restauration des applications qui utilisent le Volume Shadow Copy Service (VSS).
  
> [!NOTE]
> Groupes de stockage ne sont pas disponibles dans Exchange 2013. Prise en charge des groupes de stockage a été supprimé des versions d’Exchange commençant par Exchange Server 2010. Pour assurer la compatibilité descendante avec les bases de données et les groupes de stockage dans les versions d’Exchange antérieures à Exchange 2010, l’API CHKSGFILES vous permet de spécifier les groupes de stockage. Lorsque vous exécutez CHKSGFILES par rapport à des bases de données Exchange 2013, vous devez définir les paramètres que vous spécifiez un identificateur de groupe de stockage sur une chaîne vide. 
  
## <a name="file-location"></a>Emplacement de fichier
<a name="bk_fileslocation"> </a>

L’API CHKSGFILES est fourni dans le cadre d’Exchange 2013. Vous pouvez utiliser cette API sur un ordinateur ayant le rôle de serveur de boîtes aux lettres est installé. 
  
Par défaut, la DLL CHKSGFILES est installée dans le répertoire C:\Program Files\Microsoft\Exchange\V15\Bin.
  
Exchange 2013 inclut uniquement une version 64 bits (amd64) de l’API CHKSGFILES. 
  
Vous pouvez télécharger un fichier .zip qui inclut la bibliothèque CHKSGFILE.lib et fichiers d’en-tête CHKSGFILES.hxx pour une utilisation dans votre application personnalisée à partir du [Centre de téléchargement Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
  
## <a name="development-languages"></a>Langages de développement
<a name="bk_developmentlanguages"> </a>

L’API CHKSGFILES est destinée aux versions de Visual Studio commençant par Visual Studio 2005 dans C/C++ natif. L’API CHKSGFILES n’est pas destiné à être utilisés dans du code managé. Bien que vous pouvez créer un assembly d’interopérabilité COM avec CHKSGFILES, nous ne sont pas fournis un assembly d’interopérabilité COM pris en charge avec Exchange 2013.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Fonction CChkSGFiles.CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Fonction CChkSGFiles.Delete](cchksgfiles-delete-function.md)
    
- [Énumération CChkSGFiles.ERR](cchksgfiles-err-enumeration.md)
    
- [Fonction CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Fonction CChkSGFiles.ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Fonction CChkSGFiles.ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Fonction CChkSGFiles.ErrGetHeader (réservée)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Fonction CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)
    
- [Fonction CChkSGFiles.ErrTerm](cchksgfiles-errterm-function.md)
    
- [Énumération CChkSGFiles.iDbInvalid](cchksgfiles-idbinvalid-enumeration.md)
    
- [Fonction CChkSGFiles.New](cchksgfiles-new-function.md)
    
- [Énumération CChkSGFiles.NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [Struct CChkSGFiles.PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Fonction CChkSGFiles.PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>Voir aussi

- [Exchange Online et développement Exchange](../exchange-server-development.md)
- [Sauvegarde, restauration et récupération d’urgence](http://technet.microsoft.com/en-us/library/dd876874)
    

