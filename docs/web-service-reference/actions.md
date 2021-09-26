---
title: Actions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: L’élément Actions représente l’ensemble des actions disponibles pour être prises sur un message lorsque les conditions sont remplies.
ms.openlocfilehash: 7f6608af5b8a9eb2772228a638fc42b9558f1e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546860"
---
# <a name="actions"></a>Actions

**L’élément Actions** représente l’ensemble des actions disponibles pour être prises sur un message lorsque les conditions sont remplies. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AssignCategories](assigncategories.md) <br/> |Représente les catégories qui sont marqués sur les messages électroniques.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifie l’ID du dossier dans qui les éléments de messagerie seront copiés.  <br/> |
|[Supprimer](delete.md) <br/> |Indique si les messages doivent être déplacés vers le dossier Éléments supprimés.  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |Indique les adresses de messagerie vers lesquelles les messages doivent être transmis en tant que pièces jointes.  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |Indique les adresses de messagerie vers lesquelles les messages doivent être transmis.  <br/> |
|[MarkImportance](markimportance.md) <br/> |Spécifie l’importance à marquer sur les messages.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Indique si les messages doivent être marqués comme lus.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifie l’ID du dossier vers qui les éléments de messagerie seront déplacés.  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |Indique si les messages doivent être supprimés définitivement et ne pas être enregistrés dans le dossier Éléments supprimés.  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Indique les adresses de messagerie vers lesquelles les messages doivent être redirigés.  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |Indique les numéros de téléphone mobile vers lesquels une alerte SMS (Short Message Service) doit être envoyée.  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |Indique. ID du message de modèle à envoyer en tant que réponse aux messages entrants.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Indique si les règles suivantes doivent être évaluées.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Représente une règle unique dans la boîte aux lettres d’un utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Conditions](conditions.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

