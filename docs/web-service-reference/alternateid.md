---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: L’élément AlternateId décrit un identificateur à convertir dans une demande et les résultats d’un identificateur converti dans la réponse.
ms.openlocfilehash: 6346a45b48eb811cac705d8da85dc77e6c18262c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520940"
---
# <a name="alternateid"></a>AlternateId

**L’élément AlternateId** décrit un identificateur à convertir dans une demande et les résultats d’un identificateur converti dans la réponse. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Décrit l’identificateur source dans une [demande d’opération ConvertId](convertid-operation.md) et décrit l’identificateur de destination dans une [réponse d’opération ConvertId.](convertid-operation.md)  <br/> |
|Format  <br/> |Décrit le format source dans une demande [d’opération ConvertId](convertid-operation.md) et décrit le format de destination dans une [réponse d’opération ConvertId.](convertid-operation.md) Le format de destination est décrit par l’attribut **DestinationFormat** de [l’élément ConvertId](convertid.md) dans la demande. Cet attribut est de type **IdFormatType**.  <br/> |
|Boîte aux lettres  <br/> |Décrit l’adresse SMTP (Simple Mail Transfer Protocol) principale de boîte aux lettres qui contient les identificateurs à traduire.  <br/> |
|IsArchive  <br/> |Indique si l’identificateur représente un élément ou un dossier archivé. La valeur **true indique** que l’identificateur représente un élément ou un dossier archivé. Cet attribut est facultatif.  <br/> |
   
#### <a name="format-attribute-values"></a>Formater les valeurs d’attribut

|**Valeur**|**Description**|
|:-----|:-----|
|EwsLegacyId  <br/> |Décrit les identificateurs produits par Exchange Web Services dans la version initiale de Exchange 2007.  <br/> |
|EwsId  <br/> |Décrit les identificateurs produits par Exchange Web Services à partir de Exchange 2007 SP1.  <br/> |
|EntryId  <br/> |Décrit les identificateurs MAPI, comme dans la **PR_ENTRYID** propriété.  <br/> |
|HexEntryId  <br/> |Décrit une représentation codée hexadécimale de la **propriété PR_ENTRYID.** Il s’agit du format des identificateurs d’événements de calendrier de disponibilité.  <br/> |
|StoreId  <br/> |Décrit les Exchange du magasin de données.  <br/> |
|OwaId  <br/> |Décrit un identificateur Outlook Web App.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération ConvertId.](convertid-operation.md)  <br/> |
|[SourceIds](sourceids.md) <br/> |Contient les identificateurs source à convertir.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

**L’élément AlternateId** décrit deux identificateurs, l’identificateur source à convertir dans la demande d’opération [ConvertId](convertid-operation.md) et l’identificateur converti dans l’élément [ConvertIdResponse.](convertidresponse.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

||||
|:-----|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ConvertId](convertid-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Conversion d’identificateurs](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

