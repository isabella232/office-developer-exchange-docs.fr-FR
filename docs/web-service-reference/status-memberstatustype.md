---
title: État (MemberStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: L’élément Status fournit des informations sur l’état d’un membre de la liste de distribution sur le serveur.
ms.openlocfilehash: bfa0c349d6af51c1b2238c9749d2656541d31906
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465463"
---
# <a name="status-memberstatustype"></a>État (MemberStatusType)

L’élément **Status** fournit des informations sur l’état d’un membre de la liste de distribution sur le serveur. 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 **MemberStatusType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Membre](member-ex15websvcsotherref.md) <br/> |Représente un membre d’une liste de distribution.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **Status** . 
  
**Valeurs de l’élément Status**

|**Valeur**|**Description**|
|:-----|:-----|
|Non reconnu  <br/> |Les informations de membre ne sont pas valides ou ne sont pas reconnues.  <br/> |
|Normal  <br/> |Les informations sur les membres d’une liste de distribution sont synchronisées avec l’objet référencé.  <br/> |
|Rétrogradé  <br/> |L’objet référencé n’est pas disponible.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

