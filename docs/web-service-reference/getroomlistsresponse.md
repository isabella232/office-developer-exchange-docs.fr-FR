---
title: GetRoomListsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomListsResponse
api_type:
- schema
ms.assetid: 8c736f68-1026-496a-b12f-c169c078abd0
description: L’élément GetRoomListsResponse définit la réponse à partir d’une demande d’opération GetRoomLists.
ms.openlocfilehash: b6d7c2baa2861309d72bcbf880eaed2ad0989175
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462942"
---
# <a name="getroomlistsresponse"></a>GetRoomListsResponse

L’élément **GetRoomListsResponse** définit la réponse à partir d’une demande d' [opération GetRoomLists](getroomlists-operation.md) . 
  
- [ResponseMessages](responsemessages.md)
- [GetRoomListsResponse](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 **GetRoomListsResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état de la réponse. <br/><br/>Les valeurs suivantes sont valides pour cet attribut :  <br/><br/>-Réussite  <br/>-AVERTISSEMENT  <br/>-Erreur  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est satisfaite.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités. <br/><br/>Voici des exemples de sources d’avertissements :  <br/><br/>-La banque Exchange est hors connexion pendant le traitement par lots.  <br/>-Le service d’annuaire Active Directory est hors connexion.  <br/>-Les boîtes aux lettres ont été déplacées.  <br/>-La base de données de messages (MDB) est hors connexion.  <br/>-Un mot de passe a expiré.  <br/>-Un quota a été dépassé.  <br/> |
|**Error** <br/> | Décrit une demande qui ne peut pas être satisfaite. <br/><br/>Voici des exemples de sources d’erreurs :  <br/><br/>-Attributs ou éléments non valides  <br/>-Les attributs ou les éléments sont en dehors de la plage  <br/>-Balise inconnue  <br/>-Attribut ou élément non valide dans le contexte  <br/>-Tentative d’accès non autorisée par un client  <br/>-Échec côté serveur en réponse à un appel côté client valide  <br/><br/>  Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/>- |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Cet élément contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[RoomLists](roomlists.md) <br/> |Fournit la liste des adresses de messagerie et des noms d’affichage qui représentent les listes des salles de réunion.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande des services Web Exchange.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetRoomLists](getroomlists-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

