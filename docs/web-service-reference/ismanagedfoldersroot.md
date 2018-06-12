---
title: IsManagedFoldersRoot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsManagedFoldersRoot
api_type:
- schema
ms.assetid: 00823fb9-bf8b-49bb-8e1b-d698c6d4063f
description: L’élément IsManagedFoldersRoot indique si le dossier géré est la racine de tous les dossiers gérés.
ms.openlocfilehash: 3484a3fef56545a9a8d56af65f56f75205918ec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828044"
---
# <a name="ismanagedfoldersroot"></a>IsManagedFoldersRoot

L’élément **IsManagedFoldersRoot** indique si le dossier géré est la racine de tous les dossiers gérés. 
  
```xml
<IsManagedFoldersRoot/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contient des informations sur un dossier géré.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une valeur Boolean est requise si cet élément est présent. La valeur **true** indique que le dossier est le dossier racine du dossier géré. la valeur **false** indique que le dossier n’est pas le dossier racine du dossier géré. 
  
## <a name="remarks"></a>Note

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

