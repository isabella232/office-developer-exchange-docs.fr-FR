---
title: Structure CChkSGFiles.PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: f324ec9aca6f94911041c227ce039139292a10aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516257"
---
# <a name="cchksgfilespage_info-struct"></a>Structure CChkSGFiles.PAGE_INFO

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Contient des informations pour une page Exchange base de données. Cette structure est utilisée avec la **fonction ErrCheckDbPages.** 
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a>Members

### <a name="ulpgno"></a>ulPgNo
  
Long non signé. Numéro de page logique de la page de base de données à vérifier. Cette valeur doit être définie avant **d’appeler ErrCheckDbPages.** Si l’application lit le fichier en fonction des décalages de fichier et doit par conséquent maquer ces décalages de fichiers sur des numéros de page logiques, la méthode **PgnoFromFileOffset** est utile pour déterminer la valeur de ce champ. **ErrCheckDbPages ne** modifie pas cette valeur. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Booléen. La valeur TRUE indique que la page de base de données contient des données. La valeur FALSE indique que la page contient uniquement des zéros. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Booléen. La valeur TRUE indique qu’une insistérialisation de la valeur checksum a été détectée dans la page de base de données, mais qu’il s’agit d’une erreur correctable. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="checksumactual"></a>checksumActual
  
Unsigned 64-bit integer. Indique la valeur de la checksum stockée dans la base de données pour cette page logique. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="checksumexpected"></a>checksumExpected
  
Unsigned 64-bit integer. Il s’agit de la valeur de la base de contrôle attendue calculée pour la page de base de données . il est définie par **ErrCheckDbPages**. Si cette valeur est différente de celle stockée sur la page de base de données (autrement dit, la valeur renvoyée dans **checksumActual**), **ErrCheckDbPages** indique qu’une erreur a été trouvée sur cette page de base de données. 
    
### <a name="dbtime"></a>dbTime
  
Unsigned 64-bit integer. **ErrCheckDbPages** définit ce membre sur l’timestamp sur la page de base de données. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Unsigned 64-bt integer. **ErrCheckDbPages** définit ce membre sur la valeur de la table de contrôle calculée du contenu de la page, à l’exclusion des données inutiles lors de la détermination de l’équivalence de la page logique. Par exemple, il est inutile de prendre en compte les valeurs de données dans l’espace de page de base de données inutilisé. Ce membre n’est valide que si les valeurs **checksumActual**  et  **checksumExpected**  sont égales les unes aux autres. 
    
### <a name="ulflags"></a>ulFlags
  
Unsigned 64-bit integer. Réservé à une utilisation future. La valeur de ce champ doit être définie sur 0 (zéro) avant d’appeler **ErrCheckDbPages**.
    
## <a name="remarks"></a>Remarques

Lorsque vous appelez **la fonction ErrCheckDbPages,** le **paramètre rgPageInfo** est un tableau de structures **PAGE \_ INFO.** Il doit y avoir une structure **PAGE \_ INFO** pour chaque page de base de données à vérifier. 
  
L’application doit définir le membre **ulPgno**  sur la valeur appropriée et doit également définir le membre  **ulFlags**  sur 0 (zéro) avant d’appeler **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous qui s’exécute l’application doit avoir des autorisations d’accès en lecture à la base de données et aux fichiers journaux qui doivent être vérifiés.
  

