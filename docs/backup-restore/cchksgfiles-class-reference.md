---
title: Référence de classe fonction cchksgfiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Recherchez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.
ms.openlocfilehash: 38b1f2c900767c22594636f0c6ddf4855961aec4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526731"
---
# <a name="cchksgfiles-class-reference"></a>Référence de classe fonction cchksgfiles

Recherchez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.
  
**S’applique à :** Exchange Server 2013 
  
L’API CHKSGFILES permet aux applications de sauvegarde et de restauration de vérifier l’intégrité des fichiers journaux de transactions et des bases de données Exchange Server 2013 par programme. Vous pouvez utiliser cette API dans les applications de sauvegarde et de restauration qui utilisent le service VSS (Volume Shadow Copy Service).
  
> [!NOTE]
> Les groupes de stockage ne sont pas disponibles dans Exchange 2013. La prise en charge des groupes de stockage a été supprimée des versions d’Exchange à partir d’Exchange Server 2010. Pour assurer la compatibilité descendante avec les bases de données et les groupes de stockage dans les versions d’Exchange antérieures à Exchange 2010, l’API CHKSGFILES vous permet de spécifier des groupes de stockage. Lorsque vous exécutez CHKSGFILES sur des bases de données Exchange 2013, vous devez définir des paramètres qui spécifient un identificateur de groupe de stockage sur une chaîne vide. 
  
## <a name="file-location"></a>Emplacement du fichier
<a name="bk_fileslocation"> </a>

L’API CHKSGFILES est fournie dans le cadre d’Exchange 2013. Vous pouvez utiliser cette API sur un ordinateur sur lequel le rôle serveur de boîtes aux lettres est installé. 
  
Par défaut, la DLL CHKSGFILES est installée dans le répertoire C:\Program Files\Microsoft\Exchange\V15\Bin
  
Exchange 2013 inclut uniquement une version 64 bits (amd64) de l’API CHKSGFILES. 
  
Vous pouvez télécharger un fichier. zip qui inclut la bibliothèque CHKSGFILE. lib et des fichiers d’en-tête CHKSGFILES. hxx à utiliser dans votre application personnalisée à partir du [Centre de téléchargement Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).
  
## <a name="development-languages"></a>Langages de développement
<a name="bk_developmentlanguages"> </a>

L’API CHKSGFILES est conçue pour une utilisation avec les versions de Visual Studio à partir de Visual Studio 2005 en mode natif C/C++. L’API CHKSGFILES n’est pas destinée à être utilisée dans du code managé. Bien que vous puissiez créer un assembly d’interopérabilité COM avec CHKSGFILES, nous ne fournissons pas d’assembly d’interopérabilité COM pris en charge avec Exchange 2013.
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Fonction fonction cchksgfiles. CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Fonction fonction cchksgfiles. Delete](cchksgfiles-delete-function.md)
    
- [Fonction cchksgfiles. ERR, énumération](cchksgfiles-err-enumeration.md)
    
- [Fonction fonction cchksgfiles. ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Fonction fonction cchksgfiles. ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Fonction fonction cchksgfiles. ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Fonction fonction cchksgfiles. ErrGetHeader (réservée)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Fonction fonction cchksgfiles. ErrInit](cchksgfiles-errinit-function.md)
    
- [Fonction fonction cchksgfiles. ErrTerm](cchksgfiles-errterm-function.md)
    
- [Fonction cchksgfiles. iDbInvalid, énumération](cchksgfiles-idbinvalid-enumeration.md)
    
- [Fonction fonction cchksgfiles. New](cchksgfiles-new-function.md)
    
- [Fonction cchksgfiles. NO_FLAGS, énumération](cchksgfiles-no_flags-enumeration.md)
    
- [Struct fonction cchksgfiles. PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Fonction fonction cchksgfiles. PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>Voir aussi

- [Développement d’Exchange et Exchange Online](../exchange-server-development.md)
- [Sauvegarde, restauration et récupération d’urgence](https://technet.microsoft.com/library/dd876874)
    

