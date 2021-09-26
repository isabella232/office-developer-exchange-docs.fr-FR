---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: L’élément MimeContent contient le flux MIME ASCII d’un objet qui est représenté au format base64Binary et prend en charge [RFC2045].
ms.openlocfilehash: 43040f241008010620ff4f1018cc5410a7a00e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542070"
---
# <a name="mimecontent"></a>MimeContent

**L’élément MimeContent** contient le flux MIME ASCII d’un objet qui est représenté au format base64Binary et prend en charge [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**CharacterSet** <br/> |Si elle est définie, la valeur de cet attribut est ignorée par le serveur.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[CalendarItem](calendaritem.md)  |  [Contact](contact.md)  |  [DistributionList](distributionlist.md)  |  [Élément](item.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [Message](message-ex15websvcsotherref.md)  |  [RemoveItem](removeitem.md)  |  [Tâche](task.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente un flux MIME base64Binary est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le contenu du message passe par les trois niveaux d’encodage suivants avant d’être stocké dans la **valeur MimeContent** : 
  
1. Texte du message : il s’agit du codage du corps, tel que iso-2022-jp pour les caractères japonais.
    
2. Flux MIME — Codage ASCII du texte du message pour l’élément **MimeContent** ou codage UTF8 du texte du message pour l’élément [MimeContentUTF8.](mimecontentutf8.md) 
    
3. Document XML — Il s’agit toujours du flux ASCII codé en base 64 du flux MIME, où des caractères tels que « ' ' , qui sont significatifs pour XML, sont masqués dans les parseurs \< XML.
    
Chaque niveau est indépendant du niveau qui le précède.
  
**L’élément MimeContent** peut contenir les mêmes données que les autres propriétés renvoyées avec un élément. 
  
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

