---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: L’élément SendItem est l’élément racine d’une demande d’envoi d’un élément dans Exchange store.
ms.openlocfilehash: 2d1613451e7f876f0b612a3249570412e40b4764
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521619"
---
# <a name="senditem"></a>SendItem

**L’élément SendItem** est l’élément racine d’une demande d’envoi d’un élément dans Exchange store. 
  
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
|**SaveItemToFolder** <br/> |Indique si une copie de l’élément envoyé est enregistrée. L’action d’enregistrer dépend de la valeur de **SaveItemToFolder** et de la présence d’un élément [SavedItemFolderId](saveditemfolderid.md) dans la demande. Cet élément est obligatoire.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>SaveItemToFolder, attribut

|**Valeur**|**Description**|
|:-----|:-----|
|**true** <br/> |Si [l’élément SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément est enregistré dans le dossier Éléments envoyés. Si [l’élément SavedItemFolderId](saveditemfolderid.md) est présent, l’élément est enregistré dans le dossier spécifié par l’élément [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
|**false** <br/> |Si [l’élément SavedItemFolderId](saveditemfolderid.md) n’est pas présent, l’élément n’est pas enregistré. Si [l’élément SavedItemFolderId](saveditemfolderid.md) est présent, une réponse d’erreur est renvoyée avec un élément [ResponseCode](responsecode.md) qui contient la valeur **ErrorInvalidSendItemSaveSettings.**  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contient les identités uniques des éléments, des éléments d’occurrence et des éléments maîtres périodiques utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Exchange store.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifie le dossier cible pour les opérations qui update, send et create items in the Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Si un élément du dossier Éléments envoyés est envoyé, l’élément envoyé est supprimé et une copie de celui-ci est mise dans le dossier Éléments envoyés.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SendItem](senditem-operation.md)

