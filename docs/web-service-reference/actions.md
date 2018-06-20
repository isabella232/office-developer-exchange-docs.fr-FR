---
title: Actions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: L’élément Actions représente l’ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755156"
---
# <a name="actions"></a>Actions

L’élément **Actions** représente l’ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies. 
  
[Règle (RuleType)](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 **RuleActionsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AssignCategories](assigncategories.md) <br/> |Représente les catégories qui sont marqués dans les messages électroniques.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifie l’ID du dossier qui sont copiées dans les éléments de courrier électronique.  <br/> |
|[Supprimer](delete.md) <br/> |Indique si les messages doivent être déplacés vers le dossier éléments supprimés.  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |Indique les adresses de messagerie à laquelle les messages sont transmis en tant que pièces jointes.  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |Indique les adresses de messagerie à laquelle les messages doivent être transférés.  <br/> |
|[MarkImportance](markimportance.md) <br/> |Spécifie l’importance qui doit être marqué sur les messages.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Indique si les messages doivent être marqués comme étant en lecture.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifie l’ID du dossier qui seront déplacées vers des éléments de courrier électronique.  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |Indique si les messages doivent être définitivement supprimés et non enregistré dans le dossier éléments supprimés.  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Indique les adresses de messagerie à laquelle les messages doivent être redirigé.  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |Indique les numéros de téléphone mobile à laquelle une alerte Service SMS (Short Message) doit être envoyé.  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |Indique. ID de modèle de message qui doit être envoyé en réponse aux messages entrants.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Indique si les règles suivantes doivent être évaluées.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Représente une règle de boîte aux lettres d’un utilisateur unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Conditions](conditions.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

