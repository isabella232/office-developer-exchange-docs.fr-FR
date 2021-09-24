---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: L’élément UserParameters contient une liste des extensions client activées et désactivées.
ms.openlocfilehash: 1d93ec0f4e44b238fcb9aca23672c262795290a6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510728"
---
# <a name="userparameters"></a>UserParameters

**L’élément UserParameters** contient une liste des extensions client activées et désactivées. 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 **GetClientExtensionUserParametersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|UserId  <br/> |La valeur de texte de **l’attribut UserId** est l’identificateur de l’utilisateur.  <br/> |
|EnabledOnly  <br/> |La valeur de texte **de EnabledOnly** indique si la réponse contient uniquement les extensions activées.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[UserEnabledExtensions](userenabledextensions.md)  |  [UserDisabledExtensions](userdisabledextensions.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetClientExtension](getclientextension.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

