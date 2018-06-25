---
title: String
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: L’élément chaîne représente une chaîne qui est utilisée par les éléments, des contacts, des tâches et des conversations.
ms.openlocfilehash: 66260c7ebcb56049a78c5eddbe057dfa8d61f193
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829607"
---
# <a name="string"></a>String

L’élément **chaîne** représente une chaîne qui est utilisée par les éléments, des contacts, des tâches et des conversations. 
  
```XML
<String/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contient une collection de chaînes qui identifient les catégories appartient un élément dans la boîte aux lettres.  <br/> |
|[Enfants](children.md) <br/> |Contient les noms des enfants d’un contact.  <br/> |
|[Companies](companies.md) <br/> |Représente la collection des sociétés qui sont associés à un contact ou une tâche.  <br/> |
|[Contacts](contacts-ex15websvcsotherref.md) <br/> |Contient une liste des contacts qui sont associés à une tâche.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Contient la liste des catégories pour tous les éléments de conversation dans une boîte aux lettres.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Contient la liste des destinataires d’une conversation regroupée sur une boîte aux lettres.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Contient une liste de tous les expéditeurs des éléments de conversation dans la boîte aux lettres.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Contient une liste de toutes les personnes qui ont envoyé les messages qui sont actuellement non lus dans cette conversation entre tous les dossiers dans la boîte aux lettres.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Contient une liste des classes d’élément qui doit être marqué sur les messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Contient une liste des classifications de message qui doit être marqué sur les messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Contient la liste des destinataires de la conversation. Cet élément est en lecture seule.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Contient une liste de tous les expéditeurs des éléments de conversation dans le dossier actif. Cet élément est en lecture seule.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Contient une liste de toutes les personnes qui ont envoyé les messages qui sont actuellement non lus dans cette conversation dans le dossier actif.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de cet élément est une chaîne qui représente une catégorie, l’enfant d’un contact, une société, un destinataire unique d’une conversation ou un contact qui est associé à une tâche.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[FindConversation Operation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

