---
title: UserConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: L’élément UserConfigurationName représente le nom d’un objet de configuration utilisateur. Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur.
ms.openlocfilehash: 40580343e92493c3d39b090371708269ec3274b9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838948"
---
# <a name="userconfigurationname"></a>UserConfigurationName

L’élément **UserConfigurationName** représente le nom d’un objet de configuration utilisateur. Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur. 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

 **UserConfigurationNameType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Name** <br/> |Contient une valeur de type string qui représente le nom d’un objet de configuration utilisateur. Cet attribut est requis.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Représente l’identificateur de dossier du dossier qui contient l’objet de configuration utilisateur.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Représente un nom de dossier unique du dossier qui contient l’objet de configuration utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |Représente une demande pour supprimer un objet de configuration utilisateur.  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Représente une demande pour obtenir un objet de configuration utilisateur.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Définit un objet de configuration utilisateur unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

