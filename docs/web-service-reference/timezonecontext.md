---
title: TimeZoneContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZoneContext
api_type:
- schema
ms.assetid: 573c462b-aa1d-4ba0-8852-e3f48b26873b
description: L’élément TimeZoneContext est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour spécifier la définition de fuseau horaire à utiliser comme valeur par défaut lors de l’affectation du fuseau horaire pour les propriétés DateTime des objets créés, mis à jour et récupérés à l’aide de Exchange Web Services (EWS).
ms.openlocfilehash: a628d4a094e70f1190f2cc0eda8cc4416bc37860
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515172"
---
# <a name="timezonecontext"></a>TimeZoneContext

L’élément **TimeZoneContext** est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour spécifier la définition de fuseau horaire à utiliser comme valeur par défaut lors de l’affectation du fuseau horaire pour les propriétés DateTime des objets créés, mis à jour et récupérés à l’aide de Exchange Web Services (EWS). 
  
```xml
<TimeZoneContext>
   <TimeZoneDefinition/>
</TimeZoneContext>
```

 **TimeZoneContextType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Spécifie les périodes et les transitions qui définissent un fuseau horaire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

