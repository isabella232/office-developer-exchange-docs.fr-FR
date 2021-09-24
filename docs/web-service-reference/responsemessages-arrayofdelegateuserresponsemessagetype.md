---
title: ResponseMessages (ArrayOfDelegateUserResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 14819975-ce54-4f0e-9f90-d4b275895ea0
description: L’élément ResponseMessages contient les messages de réponse pour une demande Exchange gestion des délégués des services Web.
ms.openlocfilehash: aa90d2572679ecf3e5d99cc55731d388e083ff01
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525566"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

**L’élément ResponseMessages** contient les messages de réponse pour une demande Exchange gestion des délégués des services Web. 
  
```
<ResponseMessages>
   <DelegateUserResponseMessageType/>
</ResponseMessages>
```

 **ArrayOfDelegateUserResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contient des messages de réponse pour les opérations de gestion des délégués.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’état et le résultat d’une [demande d’opération AddDelegate.](adddelegate-operation.md)  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’état et le résultat d’une [demande d’opération GetDelegate.](getdelegate-operation.md)  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contient l’état et le résultat d’une [demande d’opération UpdateDelegate.](updatedelegate-operation.md)  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contient l’état et le résultat [d’une demande d’opération RemoveDelegate.](removedelegate-operation.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est utilisé dans [l’opération AddDelegate](adddelegate-operation.md), l’opération [GetDelegate](getdelegate-operation.md), l’opération [UpdateDelegate](updatedelegate-operation.md)et [l’opération RemoveDelegate](removedelegate-operation.md). Les réponses aux opérations de gestion des délégués sont structurées différemment des autres réponses. Les messages de réponse de gestion des délégués sont fortement typés.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle serveur d’accès au client installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération GetDelegate](getdelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)
  
[Opération RemoveDelegate](removedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

