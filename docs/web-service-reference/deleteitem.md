---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: L’élément DeleteItem définit une demande pour supprimer un élément d’une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755874"
---
# <a name="deleteitem"></a>DeleteItem

L’élément **DeleteItem** définit une demande pour supprimer un élément d’une boîte aux lettres dans la banque d’informations Exchange. 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 **DeleteItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DeleType** <br/> |Décrit comment un élément est supprimé. Cet attribut est requis.  <br/> |
|**SendMeetingCancellations** <br/> |Indique si une suppression de l’élément calendrier est communiquée aux participants. Cet attribut est requis lorsque des éléments de calendrier sont supprimés. Cet attribut est facultatif si les éléments de calendrier non sont supprimés.  <br/> |
|**AffectedTaskOccurrences** <br/> |Indique si une instance de tâche ou d’un masque de tâche est supprimé par une [opération DeleteItem](deleteitem-operation.md). Cet attribut est requis lorsque les tâches sont supprimées. Cet attribut est facultatif lors d’une tâche non sont supprimés.  <br/> |
|**SuppressReadReceipts** <br/> |Indique si les confirmations de lecture de l’élément supprimé sont supprimées. Une valeur de texte de **la valeur true**, indique que les confirmations de lecture sont supprimées. La valeur **false** indique que les confirmations de lecture sont envoyées à l’expéditeur. Cet attribut est facultatif.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |Un élément est définitivement supprimé de la banque.  <br/> |
|SoftDelete  <br/> |Un élément est déplacé vers la benne si la benne est activé.  <br/> |
|MoveToDeletedItems  <br/> |Un élément est déplacé vers le dossier éléments supprimés.  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Attribut SendMeetingCancellations

|**Valeur**|**Description**|
|:-----|:-----|
|SendToNone  <br/> |Un élément de calendrier est supprimé sans envoyer un message d’annulation.  <br/> |
|SendOnlyToAll  <br/> |Suppression d’un élément de calendrier et un message d’annulation est envoyé à tous les participants.  <br/> |
|SendToAllAndSaveCopy  <br/> |Suppression d’un élément de calendrier et un message d’annulation est envoyé à tous les participants. Une copie du message l’annulation est enregistrée dans le dossier éléments envoyés.  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Attribut AffectedTaskOccurrences

|**Valeur**|**Description**|
|:-----|:-----|
|AllOccurrences  <br/> |Une requête d’élément delete Supprime la tâche principale et par conséquent, toutes les tâches périodiques qui sont associés à la tâche principale.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Une requête d’élément delete Supprime uniquement des occurrences spécifiques d’une tâche.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemId](itemids.md) <br/> |Contient un tableau d’éléments, des éléments d’occurrence et des éléments de gabarit périodiques pour supprimer une boîte aux lettres dans la banque d’informations Exchange. L' [opération DeleteItem](deleteitem-operation.md) peuvent être effectuées sur n’importe quel type d’élément.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment où un appel au service Web est terminée, la base de données a déplacé l’élément vers le dossier éléments supprimés ou définitivement supprimé l’élément de la base de données Exchange. Ce comportement est la même valeur MicrosoftExchange Server 2007 et Exchange Server 2010. 
  
L’option **SoftDelete** fonctionne différemment pour cible différentes versions d’Exchange. **SoftDelete** pour Exchange 2007 définit un bit sur l’élément qui indique à la base de données Exchange qui est déplacée vers l’élément de la benne de dossier à un moment indéterminé, à l’avenir. **SoftDelete** pour Exchange 2010 déplace immédiatement l’élément à la benne. **SoftDelete** n’est pas une option de suppression du dossier. **SoftDelete** des recherches de traversée du contenu pour les éléments et les dossiers ne renvoie aucun résultat. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [DeleteItemResponse](deleteitemresponse.md)  
- [Opération DeleteItem](deleteitem-operation.md)

