---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: L’élément RecipientTrackingEvent contient des informations pour un événement unique pour un destinataire.
ms.openlocfilehash: 30d9cd4ca075fda9607b191f576cac1b7a529988
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525762"
---
# <a name="recipienttrackingevent"></a>RecipientTrackingEvent

**L’élément RecipientTrackingEvent** contient des informations pour un événement unique pour un destinataire. 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 **RecipientTrackingEventType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Date (MessageTracking)](date-messagetracking.md) <br/> |Cet élément est obligatoire.  <br/> |
|[Destinataire](recipient.md) <br/> |Cet élément est obligatoire.  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |Cet élément est obligatoire.  <br/> |
|[EventDescription](eventdescription.md) <br/> |Cet élément est obligatoire.  <br/> |
|[EventData](eventdata.md) <br/> |Cet élément est facultatif.  <br/> |
|[Server (MessageTracking)](server-messagetracking.md) <br/> |Cet élément est obligatoire.  <br/> |
|[InternalId](internalid.md) <br/> |Cet élément est obligatoire.  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |Cet élément est facultatif.  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |Cet élément est facultatif.  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |Cet élément est facultatif.  <br/> |
|[RootAddress](rootaddress.md) <br/> |Cet élément est facultatif.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Contient une liste d’un ou plusieurs événements de suivi pour un destinataire.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
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

