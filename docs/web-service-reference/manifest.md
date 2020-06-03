---
title: Manifeste
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af0d7435-fef6-4f0d-bd22-00e3fa576315
description: L’élément manifest contient le fichier manifeste d’application encodé en base64.
ms.openlocfilehash: faac517bf8a8f03c6ae8abffddaf10421eed1699
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530536"
---
# <a name="manifest"></a>Manifeste

L’élément **Manifest** contient le fichier manifeste d’application encodé en base64. 
  
```XML
<Manifest></Manifest>
```

 **Au base64Binary**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Manifestes](manifests.md)  |  [InstallApp](installapp.md)  |  [ClientExtension](clientextension.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément manifest est une représentation ASCII de la forme codée binaire en base64 du fichier manifeste de l’application cliente.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

