---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: L’élément MimeContentUTF8 contient le flux MIME UTF-8 d’un objet qui est représenté au format Base64Binary et prend en charge l’internationalisation des adresses de messagerie et [RFC6530].
ms.openlocfilehash: f0ab38368d3a18be38f63c86183a238e2fd0a474
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540754"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

**L’élément MimeContentUTF8** contient le flux MIME UTF-8 d’un objet qui est représenté au format Base64Binary et prend en charge l’internationalisation des adresses de messagerie et [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

Une valeur de texte qui représente un flux MIME base64binary est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le contenu du message passe par les trois niveaux d’encodage suivants avant d’être stocké dans la valeur **MimeContentUTF8** : 
  
1. Texte du message : il s’agit du codage du corps, tel que iso-2022-jp pour les caractères japonais.
    
2. Flux MIME : il s’agit du codage UTF8 du texte du message pour l’élément **MimeContentUTF8** ou du codage ASCII du texte du message pour l’élément [MimeContent.](mimecontent.md) 
    
3. Document XML — Il s’agit toujours du flux ASCII codé en base 64 du flux MIME, où des caractères tels que « ' ' , qui sont significatifs pour XML, sont masqués dans les parseurs \< XML.
    
Chaque niveau est indépendant du niveau qui le précède.
  
**L’élément MimeContentUTF8** peut contenir les mêmes données que les autres propriétés renvoyées avec un élément. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
### <a name="version-differences"></a>Différences entre les versions

Cet élément est disponible dans les versions de Exchange à partir de la build 15.00.0986.00.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

