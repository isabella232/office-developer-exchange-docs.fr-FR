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
description: L’élément ShowExternalRecipientCount indique si les consommateurs de l’opération GetMailTips ont afficher les astuces de messagerie qui indiquent le nombre de destinataires externes à laquelle un message est adressé.
ms.openlocfilehash: 1fd3ceb629689c560dc60afe01f0413602f79a0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829491"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

L’élément **ShowExternalRecipientCount** indique si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) ont afficher les astuces de messagerie qui indiquent le nombre de destinataires externes à laquelle un message est adressé. 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Contient des informations de configuration de service pour le service de conseils de messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de cet élément est **la valeur true** si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) doivent afficher les astuces de messagerie qui indiquent le nombre de destinataires externes à laquelle un message est adressé. La valeur est **false** si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) n’ont pas à afficher les astuces de messagerie qui indiquent le nombre de destinataires externes à laquelle un message est adressé. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetMailTips](getmailtips-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

