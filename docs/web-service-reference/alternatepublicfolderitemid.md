---
title: AlternatePublicFolderItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternatePublicFolderItemId
api_type:
- schema
ms.assetid: a67df9b9-8fdb-42de-b9c5-8377b71fa3d9
description: L’élément AlternatePublicFolderItemId décrit un identificateur d’élément de dossier public à convertir dans un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 11a9fafec78a9bd14e4d98982fd38954d45e4d1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464769"
---
# <a name="alternatepublicfolderitemid"></a>AlternatePublicFolderItemId

L’élément **AlternatePublicFolderItemId** décrit un identificateur d’élément de dossier public à convertir dans un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderItemId](alternatepublicfolderitemid.md)
  
```xml
<AlternatePublicFolderItemId FolderId="" Format="" ItemId=""/>
```

 **AlternatePublicFolderItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|FolderId  <br/> |Identifie le dossier public qui contient l’élément de dossier public. Cet attribut est obligatoire.  <br/> |
|Format  <br/> |Identifie le format qui décrit l’identificateur d’élément de dossier public à convertir. Cet attribut est obligatoire.  <br/> |
|ItemId  <br/> |Identifier l’élément de dossier public à convertir. Cet attribut est obligatoire.  <br/> |
   
#### <a name="format-attribute-values"></a>Valeurs de l’attribut format

|**Valeur**|**Description**|
|:-----|:-----|
|EwsLegacyId  <br/> |Décrit les identificateurs générés par les services Web Exchange dans la version initiale d’Exchange 2007.  <br/> |
|EwsId  <br/> |Décrit les identificateurs générés par les services Web Exchange à partir d’Exchange 2007 SP1.  <br/> |
|Entrée  <br/> |Décrit les identificateurs MAPI, comme dans la propriété PR_ENTRYID.  <br/> |
|HexEntryId  <br/> |Décrit une représentation codée en hexadécimal de la propriété PR_ENTRYID. Il s’agit du format des identificateurs d’événements de calendrier de disponibilité.  <br/> |
|StoreId  <br/> |Décrit les identificateurs de banque d’Exchange.  <br/> |
|OwaId  <br/> |Décrit un identificateur Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contient les identificateurs source à convertir. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ConvertId](convertid-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Conversion des identificateurs](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

