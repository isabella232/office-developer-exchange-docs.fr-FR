---
title: MaxRecipientsPerGetMailTipsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: L’élément MaxRecipientsPerGetMailTipsRequest indique le nombre maximal de destinataires qui peuvent être transmis à l’opération GetMailTips.
ms.openlocfilehash: cec343182b364fce040d5e32928cbeb569a22124
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468403"
---
# <a name="maxrecipientspergetmailtipsrequest"></a>MaxRecipientsPerGetMailTipsRequest

L’élément **MaxRecipientsPerGetMailTipsRequest** indique le nombre maximal de destinataires qui peuvent être transmis à l' [opération GetMailTips](getmailtips-operation.md).
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Contient les informations de configuration de service pour le service de conseils de messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est un entier qui représente le nombre maximal de destinataires pouvant être transmis à l' [opération GetMailTips](getmailtips-operation.md).
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetMailTips](getmailtips-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

