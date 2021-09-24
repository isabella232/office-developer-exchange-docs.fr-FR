---
title: Applications
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f6f0a2ca-22dd-4789-9eed-f0c1ec9036c4
description: L’élément Apps contient des informations sur tous les fichiers manifeste XML pour les applications installées dans une boîte aux lettres.
ms.openlocfilehash: 8a8b6c459a014517936d1c2753c4ce125892dacb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525304"
---
# <a name="apps"></a>Applications

**L’élément Apps** contient des informations sur tous les fichiers manifeste XML pour les applications installées dans une boîte aux lettres. 
  
```XML
<Apps>
    <App/>
</Apps>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Application](app.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetAppManifestsResponse](getappmanifestsresponse.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Non applicable  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Application](app.md)
- [GetAppManifestsResponse](getappmanifestsresponse.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

