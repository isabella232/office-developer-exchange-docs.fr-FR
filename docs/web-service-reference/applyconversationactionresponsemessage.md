---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: L’élément ApplyConversationActionResponseMessage contient l’état et les résultats d’une demande d’opération ApplyConversationAction.
ms.openlocfilehash: 81378c822a473d969035f46f34ffca8939d7059d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522046"
---
# <a name="applyconversationactionresponsemessage"></a>ApplyConversationActionResponseMessage

**L’élément ApplyConversationActionResponseMessage** contient l’état et les résultats d’une demande d’opération [ApplyConversationAction.](applyconversationaction-operation.md)  
  
- [ApplyConversationActionResponse](applyconversationactionresponse.md)
- [ResponseMessages](responsemessages.md)
- [ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 **ApplyConversationActionResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état de la réponse.<br/><br/>Les valeurs suivantes sont valides pour cet attribut :<ul><li>Opération réussie</li><li>Avertissement</li><li>Erreur</li></ul> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est remplie.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande était en cours de traitement et que les éléments suivants n’ont pas pu être traitées.<br/><br/>Voici quelques exemples de sources d’avertissements :<ul><li>Le magasin Exchange est hors connexion pendant le lot.</li><li>Les services de domaine Active Directory (AD DS) sont hors connexion.</li><li>Les boîtes aux lettres ont été déplacées.</li><li>La base de données de messages (MDB) est hors connexion.</li><li>Un mot de passe a expiré.</li><li>Un quota a été dépassé.</li></ul> |
|**Erreur** <br/> | Décrit une demande qui ne peut pas être remplie.<br/><br/>Voici quelques exemples de sources d’erreurs :  <ul><li>Attributs ou éléments non valides</li><li>Attributs ou éléments en dehors de la plage</li><li>Balise inconnue  </li><li>Attribut ou élément non valide dans le contexte</li><li>Une tentative d’accès non autorisé par un client</li><li>Défaillance côté serveur en réponse à un appel côté client valide</li></ul>Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé pour une utilisation ultérieure. Cet élément contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Différences entre les versions

Dans les versions de Exchange à partir de la build 15.00.0986.00, l’élément **ApplyConversationActionResponseMessage** est de type **ApplyConversationActionResponseMessageType**. Dans les versions précédentes, l’élément est de type **ResponseMessageType**.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de ApplyConversationAction](applyconversationaction-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

