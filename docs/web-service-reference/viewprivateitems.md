---
title: ViewPrivateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ViewPrivateItems
api_type:
- schema
ms.assetid: 80b949ac-440c-4a01-b428-ebafb5b1b802
description: L’élément ViewPrivateItems indique si un utilisateur délégué ou une application cliente est autorisé à afficher des éléments privés dans la boîte aux lettres du principal.
ms.openlocfilehash: fcc63534603ea4cc6e5a7f91569a14c742b10a98
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509314"
---
# <a name="viewprivateitems"></a>ViewPrivateItems

**L’élément ViewPrivateItems** indique si un utilisateur délégué ou une application cliente est autorisé à afficher des éléments privés dans la boîte aux lettres du principal. 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Identifie un délégué unique à ajouter ou à mettre à jour dans une boîte aux lettres.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur **true indique** que le délégué ou le client peut afficher des éléments privés dans la boîte aux lettres du principal. La valeur **false indique** que les éléments privés ne sont pas visibles par un délégué ou un client. 
  
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



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

