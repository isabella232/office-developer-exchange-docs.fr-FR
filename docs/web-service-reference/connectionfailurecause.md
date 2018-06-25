---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: L’élément ConnectionFailureCause spécifie la raison d’une déconnexion d’un appel téléphonique.
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755542"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

L’élément **ConnectionFailureCause** spécifie la raison d’une déconnexion d’un appel téléphonique. 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **ConnectionFailureCauseType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Spécifie les informations d’état pour un appel téléphonique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **ConnectionFailureCause** . 
  
**Valeurs des éléments ConnectionFailureCause**

|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |État d’appel n’est pas déconnecté ou la raison de déconnexion n’est pas connue.  <br/> |
|UserBusy  <br/> |La ligne de la partie appelée était occupée.  <br/> |
|NoAnswer  <br/> |La personne appelée ne répond pas.  <br/> |
|Unavailable  <br/> |Le numéro appelé n’était pas disponible.  <br/> |
|Other  <br/> |Fourre-tout pour d’autres raisons de déconnexion.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

