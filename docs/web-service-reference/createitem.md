---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: L’élément CreateItem définit une demande de création d’un élément dans Exchange store.
ms.openlocfilehash: 7276b88bd3b90edc68d7ac8fd4a7646324eadb61
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526497"
---
# <a name="createitem"></a>CreateItem

**L’élément CreateItem** définit une demande de création d’un élément dans Exchange store. 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

**CreateItemType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|Attribut|Description|
|:-----|:-----|
|**MessageDisposition** <br/> |Décrit comment l’élément sera géré après sa création. L’attribut est requis pour les messages électroniques. Cet attribut s’applique uniquement aux messages électroniques.  <br/> |
|**SendMeetingInvitations** <br/> |Décrit comment les demandes de réunion sont gérées après leur création. Cet attribut est requis pour les éléments de calendrier.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Attribut MessageDisposition

|Valeur|Description|
|:-----|:-----|
|SaveOnly  <br/> |L’élément de message est enregistré dans le dossier spécifié par [l’élément SavedItemFolderId.](saveditemfolderid.md) Les messages peuvent être envoyés ultérieurement à l’aide de [l’opération SendItem](senditem-operation.md). Un identificateur d’élément est renvoyé dans la réponse. Les identificateurs d’élément ne sont renvoyés pour aucun type d’élément à l’exception des éléments de message. Cela inclut les objets de réponse.  <br/> |
|SendOnly  <br/> |L’élément est envoyé, mais aucune copie n’est enregistrée dans le dossier Éléments envoyés. Un identificateur d’élément n’est pas renvoyé dans la réponse.<br/><br/>**REMARQUE**: **CreateItem ne prend** pas en charge l’accès délégué lorsque l’option SendOnly est utilisée, car un dossier de destination ne peut pas être spécifié avec cette option. La solution consiste à créer l’élément, à obtenir l’identificateur de l’élément, puis à utiliser l’opération SendItem pour envoyer l’élément.           |
|SendAndSaveCopy  <br/> |L’élément est envoyé et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId.](saveditemfolderid.md) Un identificateur d’élément n’est pas renvoyé dans la réponse.<br/><br/>**REMARQUE**: les demandes de réunion ne sont pas enregistrées dans le dossier identifié par la [propriété SavedItemFolderId.](saveditemfolderid.md) Pour les calendriers, seul l’emplacement d’enregistrer des éléments de calendrier peut être spécifié par la **propriété SavedItemFolderId.** Vous ne pouvez pas contrôler l’endroit où un élément de demande de réunion est enregistré. Seuls les éléments de calendrier associés sont copiés et enregistrés dans le dossier identifié par la **propriété SavedItemFolderId.**           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Attribut SendMeetingInvitations

|Valeur|Description|
|:-----|:-----|
|SendToNone  <br/> |Si l’élément est une demande de réunion, il est enregistré en tant qu’élément de calendrier, mais n’est pas envoyé.  <br/> |
|SendOnlyToAll  <br/> |La demande de réunion est envoyée à tous les participants, mais n’est pas enregistrée dans le dossier Éléments envoyés.  <br/> |
|SendToAllAndSaveCopy  <br/> |La demande de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|Élément|Description|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifie le dossier cible dans lequel un nouvel élément peut être créé. Si **l’attribut MessageDisposition** est définie sur SendOnly, un message créé sera envoyé uniquement. Le message ne sera pas placé dans le dossier identifié par l’élément [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
|[Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contient un tableau d’éléments à créer dans le dossier identifié par [l’élément SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [CreateItemResponse](createitemresponse.md)  
- [Opération CreateItem](createitem-operation.md)
- [Création de messages électroniques](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [Creating Contacts (Exchange Web Services)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Création de tâches](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [Création de rendez-vous](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

