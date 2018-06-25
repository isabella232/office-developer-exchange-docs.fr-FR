---
title: SourceIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SourceIds
api_type:
- schema
ms.assetid: 0043abd5-ba9c-4d67-8832-325f32bf7651
description: L’élément SourceIds contient les identificateurs source à convertir.
ms.openlocfilehash: c9ee9fd01367f714e1cb3770e2be5161cb45d98f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829522"
---
# <a name="sourceids"></a>SourceIds

L’élément **SourceIds** contient les identificateurs source à convertir. 
  
[ConvertId](convertid.md)
  
[SourceIds](sourceids.md)
  
```xml
<SourceIds>
   <AlternateId/>
   <AlternatePublicFolderId/>
   <AlternatePublicFolderItemId/>
</SourceIds>
```

 **NonEmptyArrayOfAlternateIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AlternateId](alternateid.md) <br/> |Décrit un identificateur d’élément ou le dossier à convertir.  <br/> |
|[AlternatePublicFolderId](alternatepublicfolderid.md) <br/> |Décrit un identificateur de dossier public à convertir.  <br/> |
|[AlternatePublicFolderItemId](alternatepublicfolderitemid.md) <br/> |Décrit un identificateur d’élément de dossier public à convertir.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConvertId](convertid.md) <br/> |Définit une demande de convertir les identificateurs d’éléments et dossiers entre les formats Exchange pris en charge.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute le serveur Exchange qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ConvertId](convertid-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Conversion des identificateurs](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

