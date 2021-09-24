---
title: CanRenameOrMove
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CanRenameOrMove
api_type:
- schema
ms.assetid: fe0cdb04-5f2b-4f1d-9d12-7ace0883cd86
description: L’élément CanRenameOrMove indique si un dossier géré peut être renommé ou déplacé par le client.
ms.openlocfilehash: 7c452ed65860939e834d77894bdb5e913ecb36a8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518806"
---
# <a name="canrenameormove"></a>CanRenameOrMove

**L’élément CanRenameOrMove** indique si un dossier géré peut être renommé ou déplacé par le client. 
  
```xml
<CanRenameOrMove/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contient des informations sur un dossier géré.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente une valeur boolé américaine. La valeur **true indique** que le dossier peut être renommé ou déplacé ; La valeur **false indique** que le dossier ne peut pas être renommé ou déplacé. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

