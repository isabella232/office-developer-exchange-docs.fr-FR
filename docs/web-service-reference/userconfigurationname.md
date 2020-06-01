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
description: L’élément UserConfigurationName représente le nom d’un objet de configuration utilisateur. Le nom de l’objet de configuration de l’utilisateur est l’identificateur d’un objet de configuration utilisateur.
ms.openlocfilehash: 020b55919f7f81602a5eb072652d82168607d306
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466030"
---
# <a name="userconfigurationname"></a>UserConfigurationName

L’élément **UserConfigurationName** représente le nom d’un objet de configuration utilisateur. Le nom de l’objet de configuration de l’utilisateur est l’identificateur d’un objet de configuration utilisateur. 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

**UserConfigurationNameType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Nom** <br/> |Contient une valeur de type String qui représente le nom d’un objet de configuration utilisateur. Cet attribut est obligatoire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Représente l’identificateur de dossier du dossier qui contient l’objet de configuration de l’utilisateur.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Représente un nom de dossier unique du dossier qui contient l’objet de configuration de l’utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DeleteUserConfiguration](deleteuserconfiguration.md) <br/> |Représente une demande de suppression d’un objet de configuration utilisateur.  <br/> |
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Représente une demande d’obtention d’un objet de configuration utilisateur.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Définit un objet de configuration utilisateur unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

