---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: L’élément ConnectionFailureCause spécifie la raison d’une déconnexion d’un appel téléphonique.
ms.openlocfilehash: de2f06ae89577b0141b8555f98dba1671a228d45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543533"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

**L’élément ConnectionFailureCause** spécifie la raison d’une déconnexion d’un appel téléphonique. 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **ConnectionFailureCauseType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Spécifie les informations d’état d’un appel téléphonique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément ConnectionFailureCause.** 
  
**Valeurs des éléments ConnectionFailureCause**

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |L’état de l’appel n’est pas déconnecté ou la raison de la déconnexion n’est pas connue.  <br/> |
|UserBusy  <br/> |La ligne de la partie appelée était occupée.  <br/> |
|NoAnswer  <br/> |La partie appelée n’a pas répondu.  <br/> |
|Indisponible  <br/> |Le numéro de la partie appelée n’était pas disponible.  <br/> |
|Autres  <br/> |Catch-all pour d’autres raisons de déconnexion.  <br/> |
   
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



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

