---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: L’élément RemoveOutlookRuleBlob indique s’il faut supprimer l’objet blob règle de Microsoft Outlook.
ms.openlocfilehash: 45336e296c39161704ce6e0d51fba1d2c61797b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829102"
---
# <a name="removeoutlookruleblob"></a>RemoveOutlookRuleBlob

L’élément **RemoveOutlookRuleBlob** indique s’il faut supprimer l’objet blob règle de Microsoft Outlook. 
  
[UpdateInboxRules](updateinboxrules.md)
  
[RemoveOutlookRuleBlob](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |Définit une demande pour mettre à jour les règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** indique que le blob règle Outlook doit être supprimé. Texte la valeur **false** indique que le blob règle Outlook ne doit pas être supprimé. 
  
## <a name="remarks"></a>Remarques

Définissez cet élément à **la valeur true** pour permettre une mise à jour des règles de boîte de réception. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de UpdateInboxRules](updateinboxrules-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

