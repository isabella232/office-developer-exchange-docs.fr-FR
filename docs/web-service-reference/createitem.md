---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: L’élément CreateItem définit une demande pour créer un élément dans la banque d’informations Exchange.
ms.openlocfilehash: 9453323bff07749f5852dae75284c61c0895adb6
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353125"
---
# <a name="createitem"></a>CreateItem

L’élément **CreateItem** définit une demande pour créer un élément dans la banque d’informations Exchange. 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

**CreateItemType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|Attribut|Description|
|:-----|:-----|
|**MessageDisposition** <br/> |Décrit comment l’élément est traité après sa création. L’attribut est requis pour les messages électroniques. Cet attribut est uniquement applicable aux messages électroniques.  <br/> |
|**SendMeetingInvitations** <br/> |Décrit comment les demandes de réunion sont gérés après leur création. Cet attribut est requis pour les éléments de calendrier.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Attribut MessageDisposition

|Valeur|Description|
|:-----|:-----|
|SaveOnly  <br/> |L’élément de message est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId](saveditemfolderid.md) . Messages peuvent être envoyés ultérieurement à l’aide de l' [opération SendItem](senditem-operation.md). Un identificateur d’élément est retourné dans la réponse. Identificateurs d’éléments ne sont pas renvoyées pour les types d’éléments à l’exception des éléments de message. Cela inclut des objets de réponse.  <br/> |
|SendOnly  <br/> |L’élément est envoyé, mais aucune copie n’est enregistrée dans le dossier éléments envoyés. Un identificateur d’élément n’est pas retourné dans la réponse.<br/><br/>**Remarque**: **CreateItem** ne prend pas en charge l’accès délégué lorsque l’option SendOnly est utilisée, car un dossier de destination ne peut pas être spécifié avec cette option. La solution de contournement consiste à créer l’élément, obtenir l’identificateur d’élément et ensuite utiliser l’opération SendItem pour envoyer l’élément.           |
|SendAndSaveCopy  <br/> |L’élément est envoyé et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) . Un identificateur d’élément n’est pas retourné dans la réponse.<br/><br/>**Remarque**: les demandes de réunion ne sont pas enregistrés dans le dossier identifié par la propriété [SavedItemFolderId](saveditemfolderid.md) . Du calendrier, uniquement l’enregistrement emplacement des éléments de calendrier peut être spécifié par la propriété **SavedItemFolderId** . Vous ne pouvez pas contrôler où une demande de réunion élément est enregistrée. Seuls les éléments associés sont copiés et enregistrés dans le dossier identifié par la propriété **SavedItemFolderId** .           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Attribut SendMeetingInvitations

|Valeur|Description|
|:-----|:-----|
|SendToNone  <br/> |Si l’élément est une demande de réunion, il est enregistré sous la forme d’un élément de calendrier, mais pas envoyé.  <br/> |
|SendOnlyToAll  <br/> |La demande de réunion est envoyée à tous les participants, mais n’est pas enregistrée dans le dossier éléments envoyés.  <br/> |
|SendToAllAndSaveCopy  <br/> |La demande de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|Élément|Description|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifie le dossier cible où un nouvel élément peut être créé. Si l’attribut **MessageDisposition** est défini à SendOnly, un message créé est uniquement envoyé. Le message n’est pas placé dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|[Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contient un tableau d’éléments à créer dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [CreateItemResponse](createitemresponse.md)  
- [Opération CreateItem](createitem-operation.md)
- [Création de Messages électroniques](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [Creating Contacts (Exchange Web Services)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Création de tâches](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [Création de rendez-vous](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

