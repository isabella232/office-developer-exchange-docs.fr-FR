---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: L’élément ConvertId définit une demande de convertir les identificateurs d’éléments et dossiers entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 956f6464fd9013f9e72d2915f21c3b011d0add5b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755651"
---
# <a name="convertid"></a>ConvertId

L’élément **ConvertId** définit une demande de convertir les identificateurs d’éléments et dossiers entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **ConvertIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DestinationFormat** <br/> |Décrit le format d’identificateur qui est renvoyé pour tous les identificateurs convertis. Le DestinationFormat est décrit par le IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Attribut DestinationFormat

|**Valeur**|**Description**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Représente le format d’identificateur qui est utilisé pour les identificateurs de Services Web Exchange qui sont fournis dans la version initiale d’Exchange 2007.  <br/> |
|**EwsId** <br/> |Représente le format d’identificateur qui est utilisé pour les identificateurs de Services Web Exchange commençant par Exchange Server 2007 SP1.  <br/> |
|**Propriété EntryId** <br/> |Représente l’identificateur MAPI, comme illustré à la propriété PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Représente l’identificateur d’événement disponibilité calendrier. Il s’agit d’une représentation de la propriété PR_ENTRYID codé en hexadécimal.  <br/> |
|**StoreId** <br/> |Représente l’identificateur de la banque Exchange.  <br/> |
|**OwaId** <br/> |Représente le format d’identificateur d’Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contient les identificateurs source à convertir.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ConvertId](convertid-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Conversion des identificateurs](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

