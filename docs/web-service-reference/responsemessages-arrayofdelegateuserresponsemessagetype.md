---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: L’élément ResponseMessages contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué.
ms.openlocfilehash: e4b5567f3ded003e9648eb8ebebfadf8f1748d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829193"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

L’élément **ResponseMessages** contient les messages de réponse pour une demande de gestion des Services Web Exchange délégué. 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfDelegateUserResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contient des messages de réponse pour les opérations de gestion de délégué.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’état et les résultats d’une requête [d’opération AddDelegate](adddelegate-operation.md) .  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’état et les résultats d’une demande [d’opération GetDelegate](getdelegate-operation.md) .  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contient l’état et les résultats d’une requête [d’opération UpdateDelegate](updatedelegate-operation.md) .  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contient l’état et les résultats d’une demande [d’opération RemoveDelegate](removedelegate-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est utilisé dans l' [opération AddDelegate](adddelegate-operation.md), l' [opération GetDelegate](getdelegate-operation.md), l' [opération UpdateDelegate](updatedelegate-operation.md)et l' [opération RemoveDelegate](removedelegate-operation.md). Les réponses d’opérations de gestion délégué sont structurées différemment des autres réponses. Les messages de réponse de gestion de délégué sont fortement typées.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération GetDelegate](getdelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)
  
[Opération RemoveDelegate](removedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

