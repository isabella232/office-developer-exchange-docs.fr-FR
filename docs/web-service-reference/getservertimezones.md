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
description: L’élément GetServerTimeZones est l’élément racine dans une demande pour récupérer des définitions de fuseau horaire à partir du serveur Exchange.
ms.openlocfilehash: 797e4543c94b0628242bcf544fe9a735ebaa5a63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460938"
---
# <a name="getservertimezones"></a>GetServerTimeZones

L’élément **GetServerTimeZones** est l’élément racine dans une demande pour récupérer des définitions de fuseau horaire à partir du serveur Exchange. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |Indique si l' [opération GetServerTimeZones](getservertimezones-operation.md) renvoie la définition complète ou uniquement le nom et l’identificateur de chaque fuseau horaire. Cet attribut est facultatif. La valeur par défaut est **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Attribut ReturnFullTimeZoneData

|**Valeur**|**Description**|
|:-----|:-----|
|**a** <br/> |Renvoyer les définitions complètes de chaque fuseau horaire.  <br/> |
|**true** <br/> |Ne renvoyer que le nom et l’identificateur de chaque fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Codes](ids.md) <br/> |Contient un tableau d’identificateurs de définition de fuseau horaire qui spécifie les définitions de fuseau horaire demandées. Cet élément est facultatif. Si cet élément n’est pas inclus dans la demande d' [opération GetServerTimeZones](getservertimezones-operation.md) , toutes les définitions de fuseau horaire qui sont disponibles sur le serveur sont renvoyées dans la réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetServerTimeZones](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

