---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: L’élément ApplyConversationActionResponseMessage contient l’état et les résultats d’une requête d’opération ApplyConversationAction.
ms.openlocfilehash: d8c5571cfc9c2ea6aaf09cb26a0e47e4abfc3f40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755298"
---
# <a name="applyconversationactionresponsemessage"></a>ApplyConversationActionResponseMessage

L’élément **ApplyConversationActionResponseMessage** contient l’état et les résultats d’une requête [d’opération ApplyConversationAction](applyconversationaction-operation.md) .  
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état de la réponse.<br/><br/>Les valeurs suivantes sont valides pour cet attribut :<ul><li>Opération réussie</li><li>Avertissement</li><li>Erreur</li></ul> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs des attributs ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Opération réussie** <br/> |Décrit une demande est remplie.  <br/> |
|**Avertissement** <br/> | Décrit une demande qui n’a pas aboutie. Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant le traite d’un élément dans la demande et les éléments suivants n’ont pas peuvent être traités.<br/><br/>Voici des exemples de sources d’avertissements :<ul><li>La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.</li><li>Services de domaine Active Directory (AD DS) est en mode hors connexion.</li><li>Boîtes aux lettres ont été déplacés.</li><li>La base de données de message (MDB) est en mode hors connexion.</li><li>Un mot de passe a expiré.</li><li>Un quota a été dépassé.</li></ul> |
|**Erreur** <br/> | Décrit une demande ne peut pas être traitée.<br/><br/>Voici des exemples de sources d’erreurs :  <ul><li>Attributs non valides ou des éléments</li><li>Attributs ou éléments qui sont hors de portée</li><li>Une balise inconnue  </li><li>Un attribut ou un élément qui n’est pas valide dans le contexte</li><li>Une tentative d’accès non autorisés par n’importe quel client</li><li>Une défaillance côté serveur en réponse à un appel côté client valid</li></ul>Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisée et réservée à un usage ultérieur. Cet élément contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations de réponse d’erreur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande de Services Web Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Différences entre les versions

Dans les versions d’Exchange commençant par version 15.00.0986.00, l’élément **ApplyConversationActionResponseMessage** est de type **ApplyConversationActionResponseMessageType**. Dans les versions précédentes, l’élément est de type **ResponseMessageType**.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de ApplyConversationAction](applyconversationaction-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

