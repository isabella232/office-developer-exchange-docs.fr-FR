---
title: ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 9684c22c-29d4-4f7f-befc-8cd41da56d38
description: L’élément ConvertId définit une demande de conversion des identificateurs d’élément et de dossier entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: fe7d46697ba72ba6458136541488f5cd498169f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545558"
---
# <a name="convertid"></a>ConvertId

**L’élément ConvertId** définit une demande de conversion des identificateurs d’élément et de dossier entre les formats Exchange pris en charge. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
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
|**DestinationFormat** <br/> |Décrit le format d’identificateur qui sera renvoyé pour tous les identificateurs convertis. DestinationFormat est décrit par IdFormatType.  <br/> |
   
#### <a name="destinationformat-attribute"></a>Attribut DestinationFormat

|**Valeur**|**Description**|
|:-----|:-----|
|**EwsLegacyId** <br/> |Représente le format d’identificateur utilisé pour les identificateurs Exchange Web Services fournis dans la version initiale de Exchange 2007.  <br/> |
|**EwsId** <br/> |Représente le format d’identificateur utilisé pour les identificateurs Exchange Services Web à partir de Exchange Server 2007 SP1.  <br/> |
|**EntryId** <br/> |Représente l’identificateur MAPI, comme dans la PR_ENTRYID propriété.  <br/> |
|**HexEntryId** <br/> |Représente l’identificateur d’événement de calendrier de disponibilité. Il s’agit d’une représentation codée hexadécimale de la propriété PR_ENTRYID.  <br/> |
|**StoreId** <br/> |Représente l’identificateur Exchange store.  <br/> |
|**OwaId** <br/> |Représente le format Outlook’identificateur Web Access.  <br/> |
   
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
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ConvertId](convertid-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Conversion d’identificateurs](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

