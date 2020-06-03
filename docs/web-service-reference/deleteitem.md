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
description: L’élément DeleteItem définit une demande de suppression d’un élément d’une boîte aux lettres dans la Banque d’Exchange.
ms.openlocfilehash: ed13ee32b487f49740aed80e8705257d3e2e6938
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529202"
---
# <a name="deleteitem"></a>DeleteItem

L’élément **DeleteItem** définit une demande de suppression d’un élément d’une boîte aux lettres dans la Banque d’Exchange. 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 **DeleteItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DeleteType** <br/> |Indique comment un élément est supprimé. Cet attribut est obligatoire.  <br/> |
|**SendMeetingCancellations** <br/> |Indique si la suppression d’un élément de calendrier est communiquée aux participants. Cet attribut est requis lorsque des éléments de calendrier sont supprimés. Cet attribut est facultatif si les éléments autres que du calendrier sont supprimés.  <br/> |
|**AffectedTaskOccurrences** <br/> |Indique si une instance de tâche ou une tâche maître est supprimée par une [opération DeleteItem](deleteitem-operation.md). Cet attribut est requis lors de la suppression des tâches. Cet attribut est facultatif lorsque des éléments autres que des tâches sont supprimés.  <br/> |
|**SuppressReadReceipts** <br/> |Indique si les confirmations de lecture pour l’élément supprimé sont supprimées. La valeur de texte **true**indique que les confirmations de lecture sont supprimées. La valeur **false** indique que les confirmations de lecture sont envoyées à l’expéditeur. Cet attribut est facultatif.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleteType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |Un élément est définitivement supprimé de la Banque.  <br/> |
|SoftDelete  <br/> |Un élément est déplacé vers la benne si la benne est activée.  <br/> |
|MoveToDeletedItems  <br/> |Un élément est déplacé vers le dossier Éléments supprimés.  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Attribut SendMeetingCancellations

|**Valeur**|**Description**|
|:-----|:-----|
|SendToNone  <br/> |Un élément de calendrier est supprimé sans envoyer de message d’annulation.  <br/> |
|SendOnlyToAll  <br/> |Un élément de calendrier est supprimé et un message d’annulation est envoyé à tous les participants.  <br/> |
|SendToAllAndSaveCopy  <br/> |Un élément de calendrier est supprimé et un message d’annulation est envoyé à tous les participants. Une copie du message d’annulation est enregistrée dans le dossier éléments envoyés.  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Attribut AffectedTaskOccurrences

|**Valeur**|**Description**|
|:-----|:-----|
|AllOccurrences  <br/> |Une demande de suppression d’élément supprime la tâche principale, et par conséquent toutes les tâches périodiques qui sont associées à la tâche principale.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Une demande de suppression d’élément supprime uniquement les occurrences spécifiques d’une tâche.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contient un tableau d’éléments, d’éléments d’occurrences et d’éléments principaux périodiques à supprimer d’une boîte aux lettres dans la Banque d’Exchange. L' [opération DeleteItem](deleteitem-operation.md) peut être effectuée sur n’importe quel type d’élément.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment de la fin d’un appel de service Web, la base de données a déplacé l’élément dans le dossier éléments supprimés ou a définitivement supprimé l’élément de la base de données Exchange. Ce comportement est le même pour MicrosoftExchange Server 2007 et Exchange Server 2010. 
  
L’option **SoftDelete** fonctionne différemment pour différentes versions cibles d’Exchange. **SoftDelete** pour Exchange 2007 définit un bit sur l’élément qui indique à la base de données Exchange que l’élément sera déplacé vers le dossier de la benne à un moment indéterminé à l’avenir. **SoftDelete** pour Exchange 2010 déplace immédiatement l’élément vers la benne. **SoftDelete** n’est pas une option de suppression de dossier. Les recherches de parcours **SoftDelete** pour les éléments et les dossiers ne renverront aucun résultat. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Updateitemresponse](deleteitemresponse.md)  
- [Opération DeleteItem](deleteitem-operation.md)

