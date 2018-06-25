---
title: UserParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bad7311f-7ecd-4f0c-b8e7-dd8f7d378f55
description: L’élément UserParameters contient une liste des extensions de client activé et désactivé.
ms.openlocfilehash: e0a72fe13255380ee56b32c863fb3bffb2e1ac5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838970"
---
# <a name="userparameters"></a>UserParameters

L’élément **UserParameters** contient une liste des extensions de client activé et désactivé. 
  
```XML
<UserParameters UserId="" EnabledOnly="">
   <UserEnabledExtensions/>
   <UserDisabledExtensions/>
</UserParameters>
```

 **GetClientExtensionUserParametersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|UserId  <br/> |La valeur de texte de l’attribut **UserId** est l’identificateur de l’utilisateur.  <br/> |
|EnabledOnly  <br/> |La valeur de texte de **EnabledOnly** indique si la réponse contient uniquement les extensions activées.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[UserEnabledExtensions](userenabledextensions.md) | [UserDisabledExtensions](userdisabledextensions.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetClientExtension](getclientextension.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

