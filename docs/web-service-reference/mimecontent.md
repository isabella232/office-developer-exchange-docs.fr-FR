---
title: Lamimecontent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: L’élément Lamimecontent contient le flux MIME ASCII d’un objet représenté au format base64Binary et prend en charge [RFC2045].
ms.openlocfilehash: 039ef1245d48e4cf13141970921dd210f4bd7d06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530435"
---
# <a name="mimecontent"></a>Lamimecontent

L’élément **lamimecontent** contient le flux MIME ASCII d’un objet représenté au format base64Binary et prend en charge [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**CharacterSet** <br/> |Si ce paramètre est défini, la valeur de cet attribut est ignorée par le serveur.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[CalendarItem](calendaritem.md)  |  [Contact](contact.md)  |  [DistributionList](distributionlist.md)  |  [Élément](item.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [MeetingMessage](meetingmessage.md)  |  [Propriété meetingrequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [Message](message-ex15websvcsotherref.md)  |  [RemoveItem](removeitem.md)  |  [Tâche](task.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente un flux MIME base64Binary est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le contenu du message passe par les trois niveaux d’encodage suivants avant d’être stocké dans la valeur **lamimecontent** : 
  
1. Texte du message — il s’agit du codage de corps, tel que ISO-2022-JP pour les caractères japonais.
    
2. Flux MIME : il s’agit du codage ASCII du texte du message pour l’élément **lamimecontent** ou le codage UTF8 du texte du message pour l’élément [MimeContentUTF8](mimecontentutf8.md) . 
    
3. Document XML : il s’agit toujours du flux ASCII encodé en base64 du flux MIME, où les caractères tels que « \< », qui sont significatifs en XML, sont masqués dans les analyseurs XML.
    
Chaque niveau est indépendant du niveau qui le précède.
  
L’élément **lamimecontent** peut contenir les mêmes données que d’autres propriétés renvoyées avec un élément. 
  
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

