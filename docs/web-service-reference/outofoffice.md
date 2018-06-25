---
title: OutOfOffice
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: L’élément OutOfOffice représente le message de réponse et un délai d’expiration pour l’envoi du message de réponse.
ms.openlocfilehash: 4e1e06ee332c44aeba03e1343c8c3258a2c9631e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828675"
---
# <a name="outofoffice"></a>OutOfOffice

L’élément **OutOfOffice** représente le message de réponse et un délai d’expiration pour l’envoi du message de réponse. 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

 **OutOfOfficeMailTip**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ReplyBody](replybody.md) <br/> |Contient un message d’absence du bureau (OOF) et la langue utilisée pour le message.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> |Contient la durée de l’état d’absence du bureau est activé si l’élément [OofState](oofstate.md) est défini sur planifiée.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Les infos-courrier](mailtips.md) <br/> |Représente les valeurs pour les différents types d’astuces de la messagerie.  <br/> |
   
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
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

