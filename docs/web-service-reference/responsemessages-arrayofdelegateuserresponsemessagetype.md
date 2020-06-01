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
description: L’élément ResponseMessages contient les messages de réponse pour une demande de gestion des délégués des services Web Exchange.
ms.openlocfilehash: 6b035f4ee46af1750a275e2c61b2cddea06b37a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465456"
---
# <a name="responsemessages-arrayofdelegateuserresponsemessagetype"></a>ResponseMessages (ArrayOfDelegateUserResponseMessageType)

L’élément **ResponseMessages** contient les messages de réponse pour une demande de gestion des délégués des services Web Exchange. 
  
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
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contient des messages de réponse pour les opérations de gestion de délégués.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération AddDelegate](adddelegate-operation.md) .  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération GetDelegate](getdelegate-operation.md) .  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération UpdateDelegate](updatedelegate-operation.md) .  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contient l’État et le résultat d’une demande d' [opération RemoveDelegate](removedelegate-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est utilisé dans l' [opération AddDelegate](adddelegate-operation.md), l’opération [GetDelegate](getdelegate-operation.md), l' [opération UpdateDelegate](updatedelegate-operation.md)et l' [opération RemoveDelegate](removedelegate-operation.md). Les réponses aux opérations de gestion des délégués sont structurées différemment des autres réponses. Les messages de réponse de gestion déléguée sont fortement typés.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération GetDelegate](getdelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)
  
[Opération RemoveDelegate](removedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

