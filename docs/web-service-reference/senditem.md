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
description: L’élément SendItem est l’élément racine dans une demande d’envoi d’un élément dans la Banque d’Exchange.
ms.openlocfilehash: 28f0d484dd079146c998cb7317bd2d80c6739e19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530564"
---
# <a name="senditem"></a>SendItem

L’élément **SendItem** est l’élément racine dans une demande d’envoi d’un élément dans la Banque d’Exchange. 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **SendItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |Identifie si une copie de l’élément envoyé est enregistrée. L’action enregistrer dépend de la valeur de **SaveItemToFolder** et de la présence ou non d’un élément [SavedItemFolderId](saveditemfolderid.md) dans la demande. Cet élément est obligatoire.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Attribut SaveItemToFolder

|**Valeur**|**Description**|
|:-----|:-----|
|**a** <br/> |Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément est enregistré dans le dossier éléments envoyés. Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, l’élément est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId](saveditemfolderid.md)  <br/> |
|**true** <br/> |Si l’élément [SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément n’est pas enregistré. Si l’élément [SavedItemFolderId](saveditemfolderid.md) est présent, une réponse d’erreur est renvoyée avec un élément [ResponseCode](responsecode.md) qui contient la valeur **ErrorInvalidSendItemSaveSettings** .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans la Banque d’Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Si un élément du dossier éléments envoyés est envoyé, l’élément envoyé est supprimé et une copie est placée dans le dossier éléments envoyés.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SendItem](senditem-operation.md)

