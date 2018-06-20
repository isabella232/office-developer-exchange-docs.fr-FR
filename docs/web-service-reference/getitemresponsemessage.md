---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: L’élément GetItemResponseMessage contient l’état et les résultats d’une demande d’opération GetItem unique.
ms.openlocfilehash: 0c8527258d4637ede053e189dfb918b910c859d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756668"
---
# <a name="getitemresponsemessage"></a>GetItemResponseMessage

L’élément **GetItemResponseMessage** contient l’état et les résultats d’une seule demande [GetItem operation](getitem-operation.md) . 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état d’une réponse [GetItem operation](getitem-operation.md) . <br/><br/>Les valeurs suivantes sont valides pour cet attribut :<br/><br/>-Réussite<br/>-Avertissement<br/>-Erreur |
   
#### <a name="responseclass-attribute-values"></a>Valeurs des attributs ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Opération réussie** <br/> |Décrit une demande est remplie.  <br/> |
|**Avertissement** <br/> | Décrit une demande qui n’a pas aboutie. Un message d’avertissement peut être renvoyée si une erreur s’est produite pendant un élément dans la demande a été traité et les éléments suivants n’ont pas peuvent être traitées.<br/><br/>Voici des exemples de sources pour les avertissements :<br/><br/>-La banque d’informations Exchange est en mode hors connexion pendant le traitement par lots.<br/>-Services de domaine actives Directory (AD DS) est en mode hors connexion.<br/>-Boîtes aux lettres sont déplacées.<br/>-MDB est en mode hors connexion.<br/>-Le mot de passe a expiré.  <br/>-Quota est dépassé. |
|**Erreur** <br/> | Décrit une demande ne peut pas être traitée.<br/><br/>Voici des exemples de sources d’erreurs :<br/><br/>-Non valide attributs ou éléments<br/>-Attributs ou éléments hors limites<br/>-Balise inconnue<br/>-Attribut ou un élément non valide dans le contexte<br/>-Accès non autorisé a tenté par n’importe quel client<br/>Échec du côté serveur en réponse à un appel côté client valid<br/><br/>Vous trouverez plus d’informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) . |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique qui a rencontré la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisés et est réservé à un usage ultérieur. Il contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations de réponse d’erreur.  <br/> |
|[Items](items.md) <br/> |Contient un tableau d’éléments renvoyés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande de Services Web Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [GetItem](getitem.md)
- [GetItem Operation](getitem-operation.md)

