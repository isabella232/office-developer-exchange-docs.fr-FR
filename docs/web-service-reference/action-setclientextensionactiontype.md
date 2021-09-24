---
title: Action (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: L’élément Action contient l’action que le serveur Exchange doit prendre sur une application.
ms.openlocfilehash: a0f5c2743ef976db2faddbb7509a8a015ef4dd8f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510378"
---
# <a name="action-setclientextensionactiontype"></a>Action (SetClientExtensionActionType)

**L’élément Action** contient l’action que le serveur Exchange doit prendre sur une application. 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 **SetClientExtensionActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ActionId  <br/> |Spécifie l’identificateur de l’action. Cet attribut est obligatoire.  <br/> |
|ExtensionId  <br/> |Spécifie l’identificateur de l’extension. Cet attribut est facultatif.  <br/> |
   
#### <a name="actionid"></a>ActionId

|**Valeur**|**Description**|
|:-----|:-----|
|Configurer  <br/> |Indique une action de configuration.  <br/> |
|Installer  <br/> |Indique une action d’installation.  <br/> |
|Désinstaller  <br/> |Indique une action de désinstallation.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ClientExtension](clientextension.md) <br/> |Contient des informations utilisateur et de configuration sur une application.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Actions (ArrayOfSetClientExtensionActionsType)](actions-arrayofsetclientextensionactionstype.md) <br/> |Spécifie un tableau d’éléments **Action.**  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

