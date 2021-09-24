---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: L’élément ReminderMessageData spécifie les données dans un message de rappel.
ms.openlocfilehash: d916e1526f11795efa54cdf186d606bc293656e0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512449"
---
# <a name="remindermessagedata"></a>ReminderMessageData

**L’élément ReminderMessageData** spécifie les données dans un message de rappel. 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 **ReminderMessageDataType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ReminderText](remindertext.md)  |  [Emplacement](location.md)  |  [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md)  |  [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md)  |  [AssociatedCalendarItemId](associatedcalendaritemid.md)
  
### <a name="parent-elements"></a>Éléments parents

[Message](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Les versions de Exchange commençant par le numéro de build 15.00.0913.09 peuvent inclure l’élément **AssociatedCalendarItemId** en tant qu’élément enfant de l’élément **ReminderMessageData.** 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Message](message-ex15websvcsotherref.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

