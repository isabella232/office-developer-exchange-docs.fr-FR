---
title: Métadonnées
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c1cc609b-65ff-4998-8d2b-545f0fdcb54c
description: L’élément Metadata contient les métadonnées relatives à l’application de messagerie.
ms.openlocfilehash: b7dd13936a25a43394b9a2d5eea8808fe08b4eb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460588"
---
# <a name="metadata"></a>Métadonnées

L’élément **Metadata** contient les métadonnées relatives à l’application de messagerie. 
  
```XML
<Metadata>
    <EndNodeUrl/>
    <AppStatus/>
    <ActionUrl/>
</Metadata>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[EndNodeUrl](endnodeurl.md)  |  [AppStatus](appstatus-ex15websvcsotherref.md)  |  [ActionUrl](actionurl.md)
  
### <a name="parent-elements"></a>Éléments parents

[App](app.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Non applicable  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[App](app.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

