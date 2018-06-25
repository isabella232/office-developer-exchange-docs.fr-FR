---
title: GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 4a24ff79-f1ae-43a1-9ac2-49baf3eaa173
description: L’élément GetMailTips représente les destinataires et les types d’astuces de la messagerie à récupérer.
ms.openlocfilehash: aad3b3d9dd578d0c92bf7d48ee8b78b58c63e23d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756669"
---
# <a name="getmailtips"></a>GetMailTips

L’élément **GetMailTips** représente les destinataires et les types d’astuces de la messagerie à récupérer. 
  
```XML
<GetMailTips>
   <SendingAs/>
   <Recipients/>
   <MailTipsRequested/>
</GetMailTips>
```

 **GetMailTipsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SendingAs](sendingas.md) <br/> |Contient une adresse de messagerie qu’un utilisateur tente d’envoyer en tant que.  <br/> |
|[Destinataires (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |Contient une liste de destinataires pour vérifier les astuces de la messagerie.  <br/> |
|[MailTipsRequested](mailtipsrequested.md) <br/> |Contient les types de conseils de messagerie demandées à partir du service.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

