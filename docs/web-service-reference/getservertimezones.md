---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: L’élément GetServerTimeZones est l’élément racine d’une demande de récupération des définitions de fuseau horaire à partir Exchange serveur.
ms.openlocfilehash: b710334e5778f8bc27ba7ac07c6bf9c2e2d3392e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533538"
---
# <a name="getservertimezones"></a>GetServerTimeZones

**L’élément GetServerTimeZones est** l’élément racine d’une demande de récupération des définitions de fuseau horaire à partir Exchange serveur. 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |Spécifie si [l’opération GetServerTimeZones](getservertimezones-operation.md) renvoie la définition complète ou uniquement le nom et l’identificateur de chaque fuseau horaire. Cet attribut est facultatif. La valeur par défaut est **true**.  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>Attribut ReturnFullTimeZoneData

|**Valeur**|**Description**|
|:-----|:-----|
|**true** <br/> |Renvoyer les définitions complètes de chaque fuseau horaire.  <br/> |
|**false** <br/> |Renvoyer uniquement le nom et l’identificateur de chaque fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID](ids.md) <br/> |Contient un tableau d’identificateurs de définition de fuseau horaire qui spécifie les définitions de fuseau horaire demandées. Cet élément est facultatif. Si cet élément n’est pas inclus dans la demande d’opération [GetServerTimeZones,](getservertimezones-operation.md) toutes les définitions de fuseau horaire disponibles sur le serveur sont renvoyées dans la réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetServerTimeZones](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

