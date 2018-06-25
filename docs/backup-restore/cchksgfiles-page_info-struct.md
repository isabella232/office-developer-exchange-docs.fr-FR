---
title: Struct CChkSGFiles.PAGE_INFO
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
description: 'Dernière modification : le 22 février 2013'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755685"
---
# <a name="cchksgfilespageinfo-struct"></a>Struct CChkSGFiles.PAGE_INFO

**S’applique à :** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Contient des informations pour une page de base de données Exchange. Cette structure est utilisée avec la fonction **ErrCheckDbPages** . 
  
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

## <a name="members"></a>Membres

### <a name="ulpgno"></a>ulPgNo
  
Long non signé. Numéro de page logique de la page de base de données à vérifier. Cette valeur doit être définie avant d’appeler **ErrCheckDbPages**. Si l’application lit le fichier basé sur le fichier décalages et doit par conséquent mapper les décalages fichier aux numéros de page logique, vous trouverez la méthode **PgnoFromFileOffset** permet de déterminer la valeur de ce champ. **ErrCheckDbPages** ne modifie pas cette valeur. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Boolean. La valeur TRUE indique que la page de base de données contient des données. La valeur FALSE indique que la page contienne des zéros. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Boolean. La valeur TRUE indique qu’il y a une incohérence dans des totaux détectée dans la page de base de données, mais qu’il s’agit d’une erreur peut être corrigée. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="checksumactual"></a>checksumActual
  
Nombre entier non signé 64 bits. Indique la valeur de la somme de contrôle stockée dans la base de données de cette page logique. **ErrCheckDbPages** définit cette valeur. 
    
### <a name="checksumexpected"></a>checksumExpected
  
Nombre entier non signé 64 bits. Il s’agit de la valeur de somme de contrôle attendue est calculée de la page de la base de données ; Il est défini par **ErrCheckDbPages**. Si cette valeur est différente de celui stocké dans la page de base de données (autrement dit, la valeur retournée dans **checksumActual**), **ErrCheckDbPages** indique qu’une erreur a été trouvée dans cette page de la base de données. 
    
### <a name="dbtime"></a>dbTime
  
Nombre entier non signé 64 bits. **ErrCheckDbPages** définit ce membre à l’horodatage dans la page de base de données. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Nombre entier non signé 64-cc. **ErrCheckDbPages** définit ce membre à la valeur calculée de somme de contrôle du contenu de la page à l’exclusion des données qui ne sont pas nécessaires lors de la détermination de l’équivalence logique de page. Par exemple, il est inutile à prendre en compte les valeurs de données dans l’espace de page de base de données inutilisés. Ce membre est valide uniquement si les valeurs **checksumActual** et **checksumExpected** sont égales. 
    
### <a name="ulflags"></a>ulFlags
  
Nombre entier non signé 64 bits. Réservé à une utilisation ultérieure. La valeur de ce champ doit être définie sur 0 (zéro) avant d’appeler **ErrCheckDbPages**.
    
## <a name="remarks"></a>Remarques

Lorsque vous appelez la fonction **ErrCheckDbPages** , le paramètre **rgPageInfo** est un tableau de **PAGE\_INFO** structures. Il doit y avoir un **PAGE\_INFO** structure pour chaque page de base de données à vérifier. 
  
L’application doit définir le membre **ulPgno** à la valeur correcte et doit également définir le membre **ulFlags** à 0 (zéro) avant d’appeler **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Configuration requise

Exchange Server 2013 inclut uniquement une version 64 bits de l’API CHKSGFILES.
  
Le compte que l’application s’exécute sous doit disposer des autorisations d’accès en lecture aux base de données et les fichiers journaux qui doivent être vérifiées.
  

