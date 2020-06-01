---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: L’élément ConvertIdResponseMessage contient l’État et le résultat d’une demande d’opération ConvertId.
ms.openlocfilehash: cd0154f87390be3516ced4be53f5371d4a348c49
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456219"
---
# <a name="convertidresponsemessage"></a>ConvertIdResponseMessage

L’élément **ConvertIdResponseMessage** contient l’État et le résultat d’une demande d' [opération ConvertId](convertid-operation.md) . 
  
- [ConvertIdResponse](convertidresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ConvertIdResponseMessage](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 **ConvertIdResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état d’une réponse d' [opération ConvertId](convertid-operation.md) .<br/><br/>Les valeurs suivantes sont valides pour cet attribut :<br/><br/>-Réussite  <br/>-AVERTISSEMENT  <br/>-Erreur  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est satisfaite.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été entièrement traitée ou pour laquelle un résultat inattendu s’est produit.  <br/> |
|**Error** <br/> | Décrit une demande qui ne peut pas être satisfaite.<br/><br/>Voici des exemples de sources d’erreurs :  <br/><br/>-Attributs ou éléments non valides  <br/>-Les attributs ou les éléments qui sont en dehors de la plage  <br/>-Balise inconnue  <br/>-Un attribut ou un élément qui n’est pas valide dans le contexte  <br/>-Une tentative d’accès non autorisée par un client  <br/>-Un échec côté serveur en réponse à un appel côté client valide<br/><br/>Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Cet élément contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[AlternateId](alternateid.md) <br/> |Décrit un identificateur converti dans la réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande des services Web Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Un message de réponse par identificateur converti est renvoyé. L’élément [AlternateId](alternateid.md) sera absent de la réponse si un code de réponse d’erreur est renvoyé, 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange 2010 sur lequel le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ConvertId](convertid-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

