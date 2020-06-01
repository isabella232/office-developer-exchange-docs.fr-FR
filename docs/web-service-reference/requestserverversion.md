---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: L’élément RequestServerVersion contient les informations de contrôle de version qui identifient la version de schéma à cibler pour une demande.
ms.openlocfilehash: c4ae59a03c812d21153e4338734185d933d914ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468319"
---
# <a name="requestserverversion"></a>RequestServerVersion

L’élément **RequestServerVersion** contient les informations de contrôle de version qui identifient la version de schéma à cibler pour une demande. 
  
```XML
<RequestServerVersion Version=""/>
```

 **ExchangeVersionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Version  <br/> |Décrit la version à cibler pour la demande. Cet attribut est requis lorsque la version du serveur cible est une version d’Exchange commençant par Exchange Server 2010.  <br/> |
   
#### <a name="version-attribute-values"></a>Valeurs d’attribut de version

|**Valeur**|**Description**|
|:-----|:-----|
|Exchange2007  <br/> |Ciblez les fichiers de schéma pour la version initiale d’Exchange 2007.  <br/> |
|Exchange2007_SP1  <br/> |Ciblez les fichiers de schéma pour Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2) et Exchange 2007 Service Pack 3 (SP3).  <br/> |
|Exchange2010  <br/> |Ciblez les fichiers de schéma pour Exchange 2010.  <br/> |
|Exchange2010_SP1  <br/> |Ciblez les fichiers de schéma pour Exchange 2010 Service Pack 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Ciblez les fichiers de schéma pour Exchange 2010 Service Pack 2 (SP2) et Exchange 2010 Service Pack 3 (SP3).  <br/> |
|Exchange2013  <br/> |Ciblez les fichiers de schéma pour Exchange 2013.  <br/> |
|Exchange2013_SP1  <br/> |Ciblez les fichiers de schéma pour Exchange 2013 Service Pack 1 (SP1).  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

L’élément **RequestServerVersion** se trouve dans l’en-tête SOAP. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Demandes de contrôle de version](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

