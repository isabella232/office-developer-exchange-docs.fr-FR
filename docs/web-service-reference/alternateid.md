---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: L’élément AlternateId décrit un identificateur pour convertir dans une requête et les résultats d’un identificateur converti dans la réponse.
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755196"
---
# <a name="alternateid"></a>AlternateId

L’élément **AlternateId** décrit un identificateur pour convertir dans une requête et les résultats d’un identificateur converti dans la réponse. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Décrit l’identificateur source dans une requête [d’opération ConvertId](convertid-operation.md) et l’identificateur de destination dans une réponse de [l’opération ConvertId](convertid-operation.md) .  <br/> |
|Format  <br/> |Décrit le format source dans une requête [d’opération ConvertId](convertid-operation.md) et le format de destination dans une réponse de [l’opération ConvertId](convertid-operation.md) . Le format de destination est décrit par l’attribut **DestinationFormat** de l’élément [ConvertId](convertid.md) dans la demande. Cet attribut est de type **IdFormatType**.  <br/> |
|Boîte aux lettres  <br/> |Décrit l’adresse SMTP Simple Mail Transfer Protocol () principal de la boîte aux lettres qui contient les identificateurs à traduire.  <br/> |
|IsArchive  <br/> |Indique si l’identificateur représente un élément archivée ou un dossier. La valeur **true** indique que l’identificateur représente un élément archivée ou un dossier. Cet attribut est facultatif.  <br/> |
   
#### <a name="format-attribute-values"></a>Valeurs d’attribut de format

|**Valeur**|**Description**|
|:-----|:-----|
|EwsLegacyId  <br/> |Décrit les identificateurs qui sont générées par les Services Web Exchange dans la version initiale d’Exchange 2007.  <br/> |
|EwsId  <br/> |Décrit les identificateurs qui sont générées par les Services Web Exchange commençant par Exchange 2007 SP1.  <br/> |
|Propriété EntryId  <br/> |Décrit les identificateurs MAPI, comme illustré à la propriété **PR_ENTRYID** .  <br/> |
|HexEntryId  <br/> |Décrit une représentation de la propriété **PR_ENTRYID** codé en hexadécimal. Il s’agit du format des identificateurs d’événement de calendrier de disponibilité.  <br/> |
|StoreId  <br/> |Décrit les identificateurs de banque Exchange.  <br/> |
|OwaId  <br/> |Décrit un identificateur d’Outlook Web App.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération ConvertId](convertid-operation.md) .  <br/> |
|[SourceIds](sourceids.md) <br/> |Contient les identificateurs source à convertir.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

L’élément **AlternateId** décrit deux identificateurs, l’identificateur de source doit être convertie dans la requête [d’opération ConvertId](convertid-operation.md) et l’identificateur converti dans l’élément [ConvertIdResponse](convertidresponse.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

||||
|:-----|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |Faux  <br/> |Faux  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ConvertId](convertid-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Conversion des identificateurs](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

