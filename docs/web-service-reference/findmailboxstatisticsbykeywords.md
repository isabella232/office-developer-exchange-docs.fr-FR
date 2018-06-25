---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: L’élément FindMailboxStatisticsByKeywords spécifie une requête pour rechercher des statistiques de boîtes aux lettres par mot clé.
ms.openlocfilehash: e667f13b66e439dca88d73a5e05d74846183928c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756401"
---
# <a name="findmailboxstatisticsbykeywords"></a>FindMailboxStatisticsByKeywords

L’élément **FindMailboxStatisticsByKeywords** spécifie une requête pour rechercher des statistiques de boîtes aux lettres par mot clé. 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 **FindMailboxStatisticsByKeywordsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîtes aux lettres (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) <br/> |Contient un tableau de boîtes aux lettres affectées par la suspension.  <br/> |
|[Mots clés](keywords-ex15websvcsotherref.md) <br/> |Spécifie les mots clés pour une recherche.  <br/> |
|[Language](language.md) <br/> |Contient la langue utilisée pour la requête de recherche.  <br/> |
|[Expéditeurs](senders.md) <br/> |Spécifie un tableau d’adresses SMTP.  <br/> |
|[Destinataires (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Spécifie un tableau de destinataires d’un message.  <br/> |
|[FromDate](fromdate.md) <br/> |Spécifie la date à laquelle le message a été envoyé.  <br/> |
|[ToDate](todate.md) <br/> |Spécifie la date à laquelle le message a été reçu.  <br/> |
|[MessageTypes](messagetypes.md) <br/> |Spécifie un tableau de messages à rechercher.  <br/> |
|[SearchDumpster](searchdumpster.md) <br/> |Spécifie s’il faut rechercher dans les éléments supprimés.  <br/> |
|[IncludePersonalArchive](includepersonalarchive.md) <br/> |Spécifie s’il faut inclure l’archive personnelle dans la recherche.  <br/> |
|[IncludeUnsearchableItems](includeunsearchableitems.md) <br/> |Spécifie s’il faut inclure des éléments qui ne peuvent pas être recherchés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

