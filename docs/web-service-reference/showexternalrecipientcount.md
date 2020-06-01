---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: L’élément ShowExternalRecipientCount indique si les consommateurs de l’opération GetMailTips doivent afficher des conseils de courrier électronique qui indiquent le nombre de destinataires externes auxquels un message est adressé.
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460469"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

L’élément **ShowExternalRecipientCount** indique si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) doivent afficher des conseils de courrier électronique qui indiquent le nombre de destinataires externes auxquels un message est adressé. 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 **Boolean**
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

La valeur texte de cet élément est **true** si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) doivent afficher des conseils de courrier électronique qui indiquent le nombre de destinataires externes auxquels un message est adressé. La valeur est **false** si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) n’ont pas besoin d’afficher des conseils de courrier qui indiquent le nombre de destinataires externes auxquels un message est adressé. 
  
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

