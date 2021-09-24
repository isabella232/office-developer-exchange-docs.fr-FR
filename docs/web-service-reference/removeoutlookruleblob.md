---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: L’élément RemoveOutlookRuleBlob indique s’il faut supprimer le blob de règle Outlook Microsoft.
ms.openlocfilehash: 92fd4e22ce0551c7922036e68fc0c6822a006b89
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525595"
---
# <a name="removeoutlookruleblob"></a>RemoveOutlookRuleBlob

**L’élément RemoveOutlookRuleBlob** indique s’il faut supprimer le blob de règle Outlook Microsoft. 
  
[UpdateInboxRules](updateinboxrules.md)
  
[RemoveOutlookRuleBlob](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
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
|[UpdateInboxRules](updateinboxrules.md) <br/> |Définit une demande de mise à jour des règles de boîte de réception dans une boîte aux lettres du magasin de serveurs.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** indique que le blob Outlook règle de messagerie doit être supprimé. Une valeur de texte **false** indique que le blob de la règle Outlook ne doit pas être supprimé. 
  
## <a name="remarks"></a>Remarques

Définissez cet élément sur **true pour** autoriser une mise à jour de règle de boîte de réception. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de UpdateInboxRules](updateinboxrules-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

