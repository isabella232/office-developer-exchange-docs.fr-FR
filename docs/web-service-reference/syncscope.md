---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: L’élément SyncScope spécifie si seuls les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de synchronisation.
ms.openlocfilehash: 5e5d19809cea1f8f244444c09615ee888fea05be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538897"
---
# <a name="syncscope"></a>SyncScope

**L’élément SyncScope** spécifie si seuls les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de synchronisation. 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 **SyncFolderItemsScopeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |Élément qui définit une demande de synchronisation des éléments dans un Exchange de la boutique.  <br/> Voici l’expression XPath de cet élément :  <br/> /SyncFolderItems  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément SyncScope.** 
  
**Valeurs des éléments SyncScope**

|**Valeur**|**Description**|
|:-----|:-----|
|NormalItems  <br/> |Spécifie que seuls les éléments du dossier sont renvoyés dans une réponse de synchronisation.  <br/> |
|NormalAndAssociatedItems  <br/> |Spécifie que les éléments du dossier et les informations associées au dossier sont renvoyés dans une réponse de synchronisation.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

