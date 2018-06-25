---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: L’élément GetServerTimeZones est l’élément racine dans une requête pour récupérer les définitions de fuseau horaire à partir du serveur Exchange.
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756746"
---
# <a name="getservertimezones"></a>GetServerTimeZones

L’élément **GetServerTimeZones** est l’élément racine dans une requête pour récupérer les définitions de fuseau horaire à partir du serveur Exchange. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |Spécifie si l' [opération GetServerTimeZones](getservertimezones-operation.md) renvoie la définition complète ou uniquement le nom et l’identificateur pour chaque fuseau horaire. Cet attribut est facultatif. La valeur par défaut est **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Attribut ReturnFullTimeZoneData

|**Valeur**|**Description**|
|:-----|:-----|
|**valeur True** <br/> |Renvoyer les définitions complètes pour chaque fuseau horaire.  <br/> |
|**False** <br/> |Retourner uniquement le nom et l’identificateur de chaque fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID](ids.md) <br/> |Contient un tableau d’identificateurs de définition de fuseau horaire qui spécifie les définitions de fuseau horaire demandé. Cet élément est facultatif. Si cet élément n’est pas inclus dans la requête [d’opération GetServerTimeZones](getservertimezones-operation.md) , toutes les définitions de fuseau horaire sont disponibles sur le serveur sont renvoyées dans la réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetServerTimeZones](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

