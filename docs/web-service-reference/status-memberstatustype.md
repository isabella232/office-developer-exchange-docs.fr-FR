---
title: Status (MemberStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: L’élément Status fournit des informations sur l’état d’un membre de liste de distribution sur le serveur.
ms.openlocfilehash: 0142ac1fa88c4cc4e513f23bbfad2869e7df32e7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544597"
---
# <a name="status-memberstatustype"></a>Status (MemberStatusType)

**L’élément Status** fournit des informations sur l’état d’un membre de liste de distribution sur le serveur. 
  
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

Le tableau suivant répertorie les valeurs possibles pour **l’élément Status.** 
  
**Valeurs des éléments d’état**

|**Valeur**|**Description**|
|:-----|:-----|
|Non reconnu  <br/> |Les informations de membre ne sont pas valides ou ne sont pas reconnues.  <br/> |
|Normal  <br/> |Les informations de membre d’une liste de distribution sont synchronisées avec l’objet référencé.  <br/> |
|Rétrogradé  <br/> |L’objet référencé n’est pas disponible.  <br/> |
   
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

