---
title: MessageTrackingReportId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: L’élément MessageTrackingReportId représente le message par son ID de message, l’organisation où le message a été trouvé, le serveur sur lequel le message a été envoyé et un ID interne qui identifie le message de manière unique.
ms.openlocfilehash: 8ed8ddcfe20c9008a208035f2b101fb5241f432d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518259"
---
# <a name="messagetrackingreportid"></a>MessageTrackingReportId

**L’élément MessageTrackingReportId** représente le message par son ID de message, l’organisation où le message a été trouvé, le serveur sur lequel le message a été envoyé et un ID interne qui identifie le message de manière unique. 
  
```XML
<MessageTrackingReportId/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Contient la demande de [l’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) pour récupérer le rapport de suivi des messages complet pour l’ID spécifié.  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contient un résultat de message unique [pour un élément FindMessageTrackingReportResponse.](findmessagetrackingreportresponse.md)  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.
  
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



[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

