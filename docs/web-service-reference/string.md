---
title: Chaîne
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: L’élément String représente une chaîne utilisée par des éléments, des contacts, des tâches et des conversations.
ms.openlocfilehash: dd85cae34ddf829f00660c8b87feb9331505183c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509293"
---
# <a name="string"></a>Chaîne

**L’élément String** représente une chaîne utilisée par des éléments, des contacts, des tâches et des conversations. 
  
```XML
<String/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contient une collection de chaînes qui identifient les catégories appartenant à un élément de la boîte aux lettres.  <br/> |
|[Enfants](children.md) <br/> |Contient les noms des enfants d’un contact.  <br/> |
|[Companies](companies.md) <br/> |Représente la collection d’entreprises associées à un contact ou à une tâche.  <br/> |
|[Contacts](contacts-ex15websvcsotherref.md) <br/> |Contient une liste de contacts associés à une tâche.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Contient la liste des catégories pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Contient la liste des destinataires d’une conversation regroupée dans une boîte aux lettres.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Contient une liste de tous les expéditeurs d’éléments de conversation dans la boîte aux lettres.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Contient une liste de toutes les personnes qui ont envoyé des messages actuellement non lus dans cette conversation dans tous les dossiers de la boîte aux lettres.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Contient une liste des classes d’éléments qui doivent être marqués sur les messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Contient une liste des classifications de messages qui doivent être marqués sur les messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Contient la liste des destinataires de la conversation. Cet élément est en lecture seule.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Contient une liste de tous les expéditeurs d’éléments de conversation dans le dossier actuel. Cet élément est en lecture seule.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Contient une liste de toutes les personnes qui ont envoyé des messages actuellement non lus dans cette conversation dans le dossier actuel.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur textuelle de cet élément est une chaîne qui représente une catégorie, l’enfant d’un contact, une société, un destinataire unique d’une conversation ou un contact associé à une tâche.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindConversation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

