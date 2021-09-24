---
title: BccRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: L’élément BccRecipient représente un destinataire qui reçoit une copie carbone non voyante ( Bcc) d’un message électronique.
ms.openlocfilehash: 178606d9c27becbf6fea5e7a9a694fb67feadc49
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526864"
---
# <a name="bccrecipient"></a>BccRecipient

**L’élément BccRecipient représente** un destinataire qui reçoit une copie carbone non voyante ( Bcc) d’un message électronique. 
  
```XML
<BccRecipient>true | false</BccRecipient>
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
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contient des informations pour un événement unique pour un destinataire.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Cet élément peut être **vrai** ou **faux**. La valeur **true indique** que le destinataire est en copie carbone non voyante ; Une valeur false **indique** que le destinataire n’est pas en copie carbone non voyante. 
  
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



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

