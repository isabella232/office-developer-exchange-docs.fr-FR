---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: L’élément FailedMailbox Spécifie le message d’erreur pour une boîte aux lettres ayant échoué sur la recherche.
ms.openlocfilehash: a4f5cd975eba121dd1d8d918b638d34f907588a8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756348"
---
# <a name="failedmailbox"></a>FailedMailbox

L’élément **FailedMailbox** Spécifie le message d’erreur pour une boîte aux lettres ayant échoué sur la recherche. 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 **FailedSearchMailboxType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres (chaîne)](mailbox-string.md) <br/> |Contient un identificateur pour la boîte aux lettres.  <br/> |
|[ErrorCode (int)](errorcode-int.md) <br/> |Spécifie le code d’erreur de la boîte aux lettres qui ont échoué à la recherche.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Représente la raison de l’erreur de validation.  <br/> |
|[IsArchive](isarchive.md) <br/> |Spécifie une valeur de type Boolean qui indique si la boîte aux lettres est une archive.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FailedMailboxes](failedmailboxes.md) <br/> |Spécifie un tableau de boîtes aux lettres ayant échoués.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

