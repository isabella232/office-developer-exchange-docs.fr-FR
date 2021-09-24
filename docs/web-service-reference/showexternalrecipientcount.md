---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: L’élément ShowExternalRecipientCount indique si les consommateurs de l’opération GetMailTips doivent afficher des conseils de messagerie qui indiquent le nombre de destinataires externes pour lesquels un message est adressé.
ms.openlocfilehash: 30615dcb1091dff01cf13679e3e1ed68c8b25af9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539099"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

**L’élément ShowExternalRecipientCount** indique si les consommateurs de l’opération [GetMailTips](getmailtips-operation.md) doivent afficher des conseils de messagerie qui indiquent le nombre de destinataires externes pour lesquels un message est adressé. 
  
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
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Contient des informations de configuration de service pour le service d’info-courrier.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur textuelle de cet élément est **true** si les consommateurs de l’opération [GetMailTips](getmailtips-operation.md) doivent afficher des conseils de messagerie qui indiquent le nombre de destinataires externes pour lesquels un message est adressé. La valeur est **false** si les consommateurs de l’opération [GetMailTips](getmailtips-operation.md) n’ont pas besoin d’afficher des infos-courrier qui indiquent le nombre de destinataires externes pour lesquels un message est adressé. 
  
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

