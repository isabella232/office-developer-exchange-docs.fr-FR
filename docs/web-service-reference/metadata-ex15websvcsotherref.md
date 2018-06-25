---
title: Métadonnées
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c1cc609b-65ff-4998-8d2b-545f0fdcb54c
description: L’élément Metadata contient des métadonnées relatives à l’application de messagerie.
ms.openlocfilehash: 8dd3a3db5a5e0afc1a23dad44d70fa3353c796f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828459"
---
# <a name="metadata"></a>Métadonnées

L’élément **Metadata** contient des métadonnées relatives à l’application de messagerie. 
  
```XML
<Metadata>
    <EndNodeUrl/>
    <AppStatus/>
    <ActionUrl/>
</Metadata>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[EndNodeUrl](endnodeurl.md) | [AppStatus](appstatus-ex15websvcsotherref.md) | [ActionUrl](actionurl.md)
  
### <a name="parent-elements"></a>Éléments parents

[App](app.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Not applicable  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[App](app.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

