---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: L’élément GetItemResponseMessage contient l’état et le résultat d’une demande d’opération GetItem unique.
ms.openlocfilehash: 3c931a6d7df91e4e90bfd0a69dc4816ee71a0aad
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521960"
---
# <a name="getitemresponsemessage"></a>GetItemResponseMessage

**L’élément GetItemResponseMessage** contient l’état et le résultat d’une demande d’opération [GetItem](getitem-operation.md) unique. 
  
- [GetItemResponse](getitemresponse.md) 
- [ResponseMessages](responsemessages.md)
- [GetItemResponseMessage](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

**ItemInfoResponseMessageType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état d’une [réponse d’opération GetItem.](getitem-operation.md) <br/><br/>Les valeurs suivantes sont valides pour cet attribut :<br/><br/>- Réussite<br/>- Avertissement<br/>- Erreur |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est remplie.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite pendant le traitement d’un élément de la demande et que les éléments suivants n’ont pas pu être traitées.<br/><br/>Voici quelques exemples de sources d’avertissements :<br/><br/>- Le magasin Exchange est hors connexion pendant le lot.<br/>- Les services de domaine Active Directory (AD DS) sont hors connexion.<br/>- Les boîtes aux lettres sont déplacées.<br/>- MDB est hors connexion.<br/>- Le mot de passe a expiré.  <br/>- Le quota est dépassé. |
|**Erreur** <br/> | Décrit une demande qui ne peut pas être remplie.<br/><br/>Voici quelques exemples de sources d’erreurs :<br/><br/>- Attributs ou éléments non valides<br/>- Attributs ou éléments en dehors de la plage<br/>- Balise inconnue<br/>- Attribut ou élément non valide dans le contexte<br/>- Tentative d’accès non autorisé par un client<br/>- Défaillance côté serveur en réponse à un appel côté client valide<br/><br/>Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md) |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Il contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[Items](items.md) <br/> |Contient un tableau d’éléments renvoyés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [GetItem](getitem.md)
- [Opération GetItem](getitem-operation.md)

