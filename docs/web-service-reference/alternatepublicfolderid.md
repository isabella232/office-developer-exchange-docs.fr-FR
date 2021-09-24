---
title: AlternatePublicFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternatePublicFolderId
api_type:
- schema
ms.assetid: 0a4dc1cc-959e-4b93-aa3a-3020ca8b8a02
description: L’élément AlternatePublicFolderId décrit un identificateur de dossier public à convertir dans un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7c4471c0c1e3e1eee3b47eba42f924340891c777
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525357"
---
# <a name="alternatepublicfolderid"></a>AlternatePublicFolderId

**L’élément AlternatePublicFolderId** décrit un identificateur de dossier public à convertir dans un autre format d’identificateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
- [ConvertId](convertid.md)
  
- [SourceIds](sourceids.md)
  
- [AlternatePublicFolderId](alternatepublicfolderid.md)
  
```xml
<AlternatePublicFolderId FolderId="" Format="" />
```

 **AlternatePublicFolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|FolderId  <br/> |Contient l’identificateur de dossier public à convertir. Cet attribut est obligatoire.  <br/> |
|Format  <br/> |Identifie le format qui décrit l’identificateur de dossier public à convertir. Cet attribut est obligatoire.  <br/> |
   
#### <a name="format-attribute"></a>Attribut Format

|**Valeur**|**Description**|
|:-----|:-----|
|EwsLegacyId  <br/> |Décrit les identificateurs produits par Exchange Web Services dans la version initiale de Exchange 2007.  <br/> |
|EwsId  <br/> |Décrit les identificateurs produits par Exchange Web Services à partir de Exchange 2007 SP1.  <br/> |
|EntryId  <br/> |Décrit les identificateurs MAPI, comme dans la PR_ENTRYID propriété.  <br/> |
|HexEntryId  <br/> |Décrit une représentation codée hexadécimale de la propriété PR_ENTRYID. Il s’agit du format des identificateurs d’événements de calendrier de disponibilité.  <br/> |
|StoreId  <br/> |Décrit les Exchange du magasin de données.  <br/> |
|OwaId  <br/> |Décrit un identificateur Outlook Web Access.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SourceIds](sourceids.md) <br/> |Contient les identificateurs source à convertir. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
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
- [Conversion d’identificateurs](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

