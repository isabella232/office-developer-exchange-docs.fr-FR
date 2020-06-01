---
title: Struct fonction cchksgfiles. PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Dernière modification : 22 février 2013'
ms.openlocfilehash: 5ec9f4303b26ea95b125adac6943945ae1276439
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456338"
---
# <a name="cchksgfilespage_info-struct"></a>Struct fonction cchksgfiles. PAGE_INFO

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Contient des informations sur une page de base de données Exchange. Cette structure est utilisée avec la fonction **ErrCheckDbPages** . 
  
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
  
Long non signé. Numéro de page logique de la page de base de données à vérifier. Cette valeur doit être définie avant l’appel de **ErrCheckDbPages**. Si l’application lit le fichier en fonction des décalages de fichiers et doit donc mapper les offsets de fichier aux numéros de page logiques, la méthode **PgnoFromFileOffset** est utile pour déterminer la valeur de ce champ. **ErrCheckDbPages** ne modifie pas cette valeur. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Type Boolean. La valeur TRUE indique que la page de base de données contient des données. La valeur FALSe indique que la page contient uniquement des zéros. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Type Boolean. La valeur TRUE indique qu’il y a eu une incohérence de checksum détectée dans la page de base de données, mais qu’il s’agit d’une erreur correcte. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="checksumactual"></a>checksumActual
  
Entier non signé 64 bits. Indique la valeur de checksum stockée dans la base de données pour cette page logique. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="checksumexpected"></a>checksumExpected
  
Entier non signé 64 bits. Il s’agit de la valeur de checksum attendue qui est calculée pour la page de base de données ; elle est définie par **ErrCheckDbPages**. Si cette valeur est différente de celle stockée sur la page de base de données (autrement dit, la valeur renvoyée dans **checksumActual**), **ErrCheckDbPages** indique qu’une erreur a été détectée sur cette page de base de données. 
    
### <a name="dbtime"></a>dbTime
  
Entier non signé 64 bits. **ErrCheckDbPages** définit ce membre sur l’horodatage sur la page de base de données. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Entier 64-BT non signé. **ErrCheckDbPages** définit ce membre sur la valeur de checksum calculée du contenu de la page, à l’exclusion des données qui ne sont pas nécessaires lors de la détermination de l’équivalence de page logique. Par exemple, il n’est pas nécessaire de prendre en compte les valeurs des données dans l’espace de la page de base de données non utilisée. Ce membre est valide uniquement si les valeurs **checksumActual** et **checksumExpected** sont égales les unes des autres. 
    
### <a name="ulflags"></a>ulFlags
  
Entier non signé 64 bits. Réservé à une utilisation future. La valeur de ce champ doit être définie sur 0 (zéro) avant l’appel de **ErrCheckDbPages**.
    
## <a name="remarks"></a>Remarques

Lors de l’appel de la fonction **ErrCheckDbPages** , le paramètre **rgPageInfo** est un tableau de structures d' ** \_ infos sur la page** . Il doit y avoir une structure d' ** \_ informations de page** pour chaque page de base de données à vérifier. 
  
L’application doit définir le membre **ulPgno** sur la valeur appropriée, et doit également définir le membre **ulFlags** sur 0 (zéro) avant d’appeler **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte sous lequel l’application s’exécute doit disposer d’autorisations d’accès en lecture à la base de données et des fichiers journaux à vérifier.
  

