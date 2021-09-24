---
title: Manifeste
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: L’élément Manifest contient le fichier manifeste d’application codé en base 64.
ms.openlocfilehash: 418191c47af0422c2d555b577dd804e02f0e38ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524762"
---
# <a name="manifest"></a>Manifeste

**L’élément Manifest** contient le fichier manifeste d’application codé en base 64. 
  
```XML
<Manifest></Manifest>
```

 **base64Binary**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Manifestes](manifests.md)  |  [InstallApp](installapp.md)  |  [ClientExtension](clientextension.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément Manifest est une représentation ASCII de la forme encodée binaire en base 64 du fichier manifeste de l’application cliente.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

