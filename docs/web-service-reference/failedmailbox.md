---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: L’élément FailedMailbox spécifie le message d’erreur pour une boîte aux lettres qui a échoué lors de la recherche.
ms.openlocfilehash: 404084bc342eb555db61c4216e936bee6ced9c36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461960"
---
# <a name="failedmailbox"></a>FailedMailbox

L’élément **FailedMailbox** spécifie le message d’erreur pour une boîte aux lettres qui a échoué lors de la recherche. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Mailbox (String)](mailbox-string.md) <br/> |Contient un identificateur pour la boîte aux lettres.  <br/> |
|[ErrorCode (int)](errorcode-int.md) <br/> |Spécifie le code d’erreur de la boîte aux lettres ayant échoué à la recherche.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Représente la raison de l’erreur de validation.  <br/> |
|[IsArchive](isarchive.md) <br/> |Spécifie une valeur de type Boolean qui indique si la boîte aux lettres est une archive.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FailedMailboxes](failedmailboxes.md) <br/> |Spécifie un tableau des boîtes aux lettres ayant échoué.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

