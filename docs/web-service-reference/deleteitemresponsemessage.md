---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: L’élément DeleteItemResponseMessage contient l’état et le résultat d’une demande d’opération DeleteItem unique.
ms.openlocfilehash: 86a1556ecd6043078b9daa1a98c0c5b8e3c7c386
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545390"
---
# <a name="deleteitemresponsemessage"></a>DeleteItemResponseMessage

**L’élément DeleteItemResponseMessage** contient l’état et le résultat d’une demande [d’opération DeleteItem](deleteitem-operation.md) unique. 
  
- [DeleteItemResponse](deleteitemresponse.md) 
- [ResponseMessages](responsemessages.md)  
- [DeleteItemResponseMessage](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 **DeleteItemResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état [d’une réponse d’opération DeleteItem.](deleteitem-operation.md)<br/><br/>Les valeurs suivantes sont valides pour cet attribut :<br/><br/>- Réussite  <br/>- Avertissement  <br/>- Erreur  <br/> |
   
#### <a name="responseclass-attribute"></a>Attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est remplie.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande était en cours de traitement et que les éléments suivants n’ont pas pu être traitées.<br/><br/>Voici quelques exemples de sources d’avertissements :<br/><br/>- Le magasin Exchange est hors connexion pendant le lot.  <br/>- Les services de domaine Active Directory (AD DS) sont hors connexion.  <br/>- Les boîtes aux lettres sont déplacées.  <br/>- La base de données de messages (MDB) est déconnectée.  <br/>- Un mot de passe a expiré.  <br/>- Un quota est dépassé.  <br/> |
|**Erreur** <br/> | Décrit une demande qui ne peut pas être remplie.<br/><br/>Voici quelques exemples de sources d’erreurs :<br/><br/>- Attributs ou éléments non valides  <br/>- Attributs ou éléments en dehors de la plage  <br/>- Balise inconnue  <br/>- Attribut ou élément non valide dans le contexte  <br/>- Une tentative de client de définir le niveau de journalisation des erreurs au-dessus du niveau maximal autorisé par l’administrateur  <br/>- Une tentative de client de définir le niveau d’échec de gravité en dessous du niveau par défaut spécifié par l’administrateur  <br/>- Tentative d’accès non autorisé par un client  <br/>- Défaillance côté serveur en réponse à un appel côté client valide<br/><br/>  Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Il contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
### <a name="version-differences"></a>Différences entre les versions

Dans les versions de Exchange à partir de la build 15.00.0986.00, l’élément **DeleteItemResponseMessage** est de type **DeleteItemResponseMessageType**. Dans les versions précédentes, l’élément est de type **ResponseMessageType**.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération DeleteItem](deleteitem-operation.md)
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Suppression d’éléments (Exchange Web Services)](https://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

