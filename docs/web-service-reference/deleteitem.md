---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: L’élément DeleteItem définit une demande de suppression d’un élément d’une boîte aux lettres dans Exchange store.
ms.openlocfilehash: aa421de447126a22c1f01b3a0dc7498ff5b74a65
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528886"
---
# <a name="deleteitem"></a>DeleteItem

**L’élément DeleteItem** définit une demande de suppression d’un élément d’une boîte aux lettres dans Exchange store. 
  
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
|**DeleteType** <br/> |Décrit comment un élément est supprimé. Cet attribut est obligatoire.  <br/> |
|**SendMeetingCancellations** <br/> |Indique si une suppression d’élément de calendrier est communiquée aux participants. Cet attribut est requis lorsque des éléments de calendrier sont supprimés. Cet attribut est facultatif si les éléments non-calendrier sont supprimés.  <br/> |
|**AffectedTaskOccurrences** <br/> |Indique si une instance de tâche ou un maître de tâche est supprimé par une [opération DeleteItem](deleteitem-operation.md). Cet attribut est requis lorsque les tâches sont supprimées. Cet attribut est facultatif lorsque des éléments autres que des tâches sont supprimés.  <br/> |
|**SuppressReadReceipts** <br/> |Indique si les reçus de lecture de l’élément supprimé sont supprimés. Une valeur de texte **true**, indique que les reçus de lecture sont supprimés. La valeur **false** indique que les reçus de lecture sont envoyés à l’expéditeur. Cet attribut est facultatif.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleteType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |Un élément est définitivement supprimé du magasin.  <br/> |
|SoftDelete  <br/> |Un élément est déplacé vers la benne si la benne est activée.  <br/> |
|MoveToDeletedItems  <br/> |Un élément est déplacé vers le dossier Éléments supprimés.  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Attribut SendMeetingCancellations

|**Valeur**|**Description**|
|:-----|:-----|
|SendToNone  <br/> |Un élément de calendrier est supprimé sans envoyer de message d’annulation.  <br/> |
|SendOnlyToAll  <br/> |Un élément de calendrier est supprimé et un message d’annulation est envoyé à tous les participants.  <br/> |
|SendToAllAndSaveCopy  <br/> |Un élément de calendrier est supprimé et un message d’annulation est envoyé à tous les participants. Une copie du message d’annulation est enregistrée dans le dossier Éléments envoyés.  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Attribut AffectedTaskOccurrences

|**Valeur**|**Description**|
|:-----|:-----|
|AllOccurrences  <br/> |Une demande de suppression d’élément supprime la tâche maître et, par conséquent, toutes les tâches périodiques associées à la tâche maître.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Une demande de suppression d’élément supprime uniquement des occurrences spécifiques d’une tâche.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contient un tableau d’éléments, d’éléments d’occurrence et d’éléments maîtres périodiques à supprimer d’une boîte aux lettres dans Exchange magasin. [L’opération DeleteItem](deleteitem-operation.md) peut être effectuée sur n’importe quel type d’élément.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment où un appel de service Web se termine, la base de données a déplacé l’élément vers le dossier Éléments supprimés ou supprimé définitivement de la base de données Exchange. Ce comportement est le même pour MicrosoftExchange Server 2007 et Exchange Server 2010. 
  
**L’option SoftDelete fonctionne** différemment pour les différentes versions cibles de Exchange. **SoftDelete** pour Exchange 2007 définit un bit sur l’élément qui indique à la base de données Exchange que l’élément sera déplacé vers le dossier de benne à un moment indéterminé à l’avenir. **SoftDelete pour** Exchange 2010 déplace immédiatement l’élément vers la benne. **SoftDelete n’est** pas une option de suppression de dossier. Les recherches de traversée **SoftDelete** pour les éléments et les dossiers ne retournent aucun résultat. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [DeleteItemResponse](deleteitemresponse.md)  
- [Opération DeleteItem](deleteitem-operation.md)

