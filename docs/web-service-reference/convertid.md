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
description: L’élément ConvertId définit une demande de conversion des identificateurs d’élément et de dossier entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d421baf1f29fb59a8c6eb2b09e1fa0e8a38ffaa4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452537"
---
# <a name="convertid"></a>ConvertId

L’élément **ConvertId** définit une demande de conversion des identificateurs d’élément et de dossier entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ConvertId DestinationFormat="">
   <SourceIds/>
</ConvertId>
```

 **ConvertIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DestinationFormat** <br/> |Décrit le format d’identificateur qui sera renvoyé pour tous les identificateurs convertis. Le DestinationFormat est décrit par le IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Attribut DestinationFormat

|**Valeur**|**Description**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Représente le format d’identificateur utilisé pour les identificateurs de services Web Exchange fournis dans la version initiale d’Exchange 2007.  <br/> |
|**EwsId** <br/> |Représente le format d’identificateur utilisé pour les identificateurs de services Web Exchange à partir d’Exchange Server 2007 SP1.  <br/> |
|**Entrée** <br/> |Représente l’identificateur MAPI, comme dans la propriété PR_ENTRYID.  <br/> |
|**HexEntryId** <br/> |Représente l’identificateur d’événement de calendrier de disponibilité. Il s’agit d’une représentation codée en hexadécimal de la propriété PR_ENTRYID.  <br/> |
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ConvertId](convertid-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Conversion des identificateurs](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

