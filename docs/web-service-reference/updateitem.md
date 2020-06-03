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
ms.openlocfilehash: 43821db58457ffce22be918a7ba6427f57230010
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466569"
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ConflictResolution** <br/> |Identifie le type de résolution de conflit à essayer pendant une mise à jour. La valeur par défaut est autosolve.  <br/> |
|**MessageDisposition** <br/> |Décrit la façon dont l’élément sera géré après sa mise à jour. L’attribut **MessageDisposition** est requis pour les éléments de message, y compris les messages de réunion, tels que les annulations de réunion, les demandes de réunion et les réponses aux réunions.  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |Indique comment les mises à jour de réunion sont communiquées après la mise à jour d’un élément de calendrier. Cet attribut est requis pour les éléments de calendrier et les occurrences d’élément de calendrier.  <br/> |
|**SuppressReadReceipts** <br/> |Indique si les confirmations de lecture pour l’élément mis à jour doivent être supprimées. Une valeur de texte **true** indique que les confirmations de lecture doivent être supprimées. La valeur **false** indique que les confirmations de lecture seront envoyées à l’expéditeur. Cet attribut est facultatif.  <br/> Cet attribut a été introduit dans Exchange Server 2013 SP1.  <br/> |
   
#### <a name="conflictresolution-attribute"></a>Attribut ConflictResolution

|**Valeur**|**Description**|
|:-----|:-----|
|NeverOverwrite  <br/> |En cas de conflit, l’opération de mise à jour échoue et une erreur est renvoyée.  <br/> |
|Autosolve  <br/> |L’opération de mise à jour résout automatiquement les conflits.  <br/> |
|AlwaysOverwrite  <br/> |En cas de conflit, l’opération de mise à jour remplace les informations.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Attribut MessageDisposition

|**Valeur**|**Description**|
|:-----|:-----|
|SaveOnly  <br/> |L’élément est mis à jour et enregistré dans son dossier actuel.  <br/> |
|SendOnly  <br/> |L’élément est mis à jour et envoyé, mais aucune copie n’est enregistrée.  <br/> |
|Méthodesendandsavecopy  <br/> |L’élément est mis à jour et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>Attribut SendMeetingInvitationsOrCancellations

|**Valeur**|**Description**|
|:-----|:-----|
|SendToNone  <br/> |L’élément de calendrier est mis à jour, mais les mises à jour ne sont pas envoyées aux participants.  <br/> |
|SendOnlyToAll  <br/> |L’élément de calendrier est mis à jour et la mise à jour de réunion est envoyée à tous les participants, mais n’est pas enregistrée dans le dossier éléments envoyés.  <br/> |
|SendOnlyToChanged  <br/> |L’élément de calendrier est mis à jour et la mise à jour de réunion n’est envoyée qu’aux participants affectés par la modification de la réunion.  <br/> |
|SendToAllAndSaveCopy  <br/> |L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier éléments envoyés.  <br/> |
|SendToChangedAndSaveCopy  <br/> |L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants affectés par la modification de la réunion, et une copie est enregistrée dans le dossier éléments envoyés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans la Banque d’Exchange.  <br/> |
|[ItemChanges](itemchanges.md) <br/> |Contient un tableau d’éléments [ItemChange,](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[UpdateItem Operation](updateitem-operation.md)

