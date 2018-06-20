---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: L’élément SendItem est l’élément racine dans une demande d’envoi d’un élément dans la banque d’informations Exchange.
ms.openlocfilehash: c5ce52ee4643219aa31ae59e8b7d40d7a904c8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829340"
---
# <a name="senditem"></a>SendItem

L’élément **SendItem** est l’élément racine dans une demande d’envoi d’un élément dans la banque d’informations Exchange. 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **SendItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |Indique si une copie de l’élément envoyé est enregistrée. L’enregistrement action dépend de la valeur de **SaveItemToFolder** et si un élément [SavedItemFolderId](saveditemfolderid.md) est présent dans la demande. Cet élément est obligatoire.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Attribut SaveItemToFolder

|**Valeur**|**Description**|
|:-----|:-----|
|**valeur True** <br/> |Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément est enregistré dans le dossier éléments envoyés. Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, l’élément est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|**False** <br/> |Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément n’est pas enregistré. Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, une réponse d’erreur s’afficheront avec un élément [ResponseCode](responsecode.md) qui contient la valeur **ErrorInvalidSendItemSaveSettings** .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemId](itemids.md) <br/> |Contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui servent à supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Si un élément dans le dossier éléments envoyés est envoyé, l’élément envoyé est supprimé et une copie de celle-ci est placée dans le dossier éléments envoyés.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SendItem](senditem-operation.md)

