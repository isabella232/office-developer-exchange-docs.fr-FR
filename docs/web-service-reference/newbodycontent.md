---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: L’élément NewBodyContent représente le nouveau contenu du corps d’un message.
ms.openlocfilehash: 48f6a12e0492249d239196ca3be19857e34e0099
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509513"
---
# <a name="newbodycontent"></a>NewBodyContent

**L’élément NewBodyContent** représente le nouveau contenu du corps d’un message. 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**BodyType** <br/> |Représente le contenu réel du corps d'un message.  <br/> |
   
#### <a name="bodytype-attribute"></a>Attribut BodyType

|**Valeur**|**Description**|
|:-----|:-----|
|**HTML** <br/> |Convertit tous les corps au format HTML.  <br/> |
|**Text** <br/> |Convertit tous les corps en texte simple.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Contient une réponse à l’expéditeur d’un élément dans la Exchange store.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contient une réponse à l’expéditeur et à tous les destinataires identifiés d’un élément dans la Exchange store.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contient un élément de la banque Exchange pour transférer à des destinataires.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Représente l'objet de réponse qui est utilisé pour annuler une réunion.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Contient une réponse à un élément de publication. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le nouveau contenu du corps d’un message.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS du serveur Exchange sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

