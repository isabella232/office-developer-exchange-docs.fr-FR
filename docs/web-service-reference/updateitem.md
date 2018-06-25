---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: L’élément UpdateItem définit une demande de mise à jour d’un élément dans une boîte aux lettres.
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838893"
---
# <a name="updateitem"></a>UpdateItem

L’élément **UpdateItem** définit une demande de mise à jour d’un élément dans une boîte aux lettres. 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 **UpdateItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ConflictResolution** <br/> |Identifie le type de résolution de conflit pour essayer pendant une mise à jour. La valeur par défaut est résoudre automatiquement.  <br/> |
|**MessageDisposition** <br/> |Décrit comment l’élément est traitée une fois qu’il est mis à jour. L’attribut **MessageDisposition** est requis pour les éléments de message, y compris les messages de réunion comme annulations de réunion, les demandes de réunion et les demandes de réunion.  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |Décrit comment les mises à jour de réunion sont communiquées après qu’un élément de calendrier est mis à jour. Cet attribut est requis pour les éléments de calendrier et occurrences d’élément de calendrier.  <br/> |
|**SuppressReadReceipts** <br/> |Indique si les confirmations de lecture de l’élément mis à jour doivent être supprimées. Une valeur de texte de **la valeur true** indique read accusés de réception doivent être supprimées. La valeur **false** indique que les confirmations de lecture sont envoyées à l’expéditeur. Cet attribut est facultatif.  <br/> Cet attribut est une nouveauté d’Exchange Server 2013 SP1.  <br/> |
   
#### <a name="conflictresolution-attribute"></a>Attribut ConflictResolution

|**Valeur**|**Description**|
|:-----|:-----|
|NeverOverwrite  <br/> |S’il existe un conflit, l’opération de mise à jour échoue et une erreur est renvoyée.  <br/> |
|Résolution automatique  <br/> |L’opération de mise à jour corrige automatiquement tout conflit.  <br/> |
|AlwaysOverwrite  <br/> |S’il existe un conflit, l’opération de mise à jour remplacera les informations.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Attribut MessageDisposition

|**Valeur**|**Description**|
|:-----|:-----|
|SaveOnly  <br/> |L’élément est mis à jour et enregistré dans le dossier actif.  <br/> |
|SendOnly  <br/> |L’élément est mis à jour et envoyé, mais aucune copie n’est enregistrée.  <br/> |
|SendAndSaveCopy  <br/> |L’élément est mis à jour et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>Attribut SendMeetingInvitationsOrCancellations

|**Valeur**|**Description**|
|:-----|:-----|
|SendToNone  <br/> |L’élément de calendrier est mis à jour mais les mises à jour ne sont pas envoyées aux participants.  <br/> |
|SendOnlyToAll  <br/> |L’élément de calendrier est mis à jour et la mise à jour de réunion est envoyée à tous les participants, mais n’est pas enregistré dans le dossier éléments envoyés.  <br/> |
|SendOnlyToChanged  <br/> |L’élément de calendrier est mis à jour et la mise à jour de réunion est envoyée uniquement aux participants qui sont affectées par la modification de la réunion.  <br/> |
|SendToAllAndSaveCopy  <br/> |L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier éléments envoyés.  <br/> |
|SendToChangedAndSaveCopy  <br/> |L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants qui sont affectées par la modification de la réunion et une copie est enregistrée dans le dossier éléments envoyés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.  <br/> |
|[ItemChanges](itemchanges.md) <br/> |Contient un tableau d’éléments [ItemChange](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[UpdateItem Operation](updateitem-operation.md)

