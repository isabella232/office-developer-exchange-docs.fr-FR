---
title: Application
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92b776b5-fec6-4443-a606-51ccb06f7afd
description: L’élément application contient des informations sur un fichier manifeste XML pour une application de messagerie qui est installé dans une boîte aux lettres.
ms.openlocfilehash: c63bbbf6eb3bf718b2cf81e67d9ec978b3bc5f8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755214"
---
# <a name="app"></a>Application

L’élément **application** contient des informations sur un fichier manifeste XML pour une application de messagerie qui est installé dans une boîte aux lettres. 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Métadonnées](metadata-ex15websvcsotherref.md) | [manifeste](manifest.md)
  
### <a name="parent-elements"></a>Éléments parents

[Applications](apps.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Not applicable  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Applications](apps.md)
- [Métadonnées](metadata-ex15websvcsotherref.md)
- [Manifeste](manifest.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

