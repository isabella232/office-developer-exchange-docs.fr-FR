---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: L’élément GetDelegate définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e31d6bd4f4387094beb467fcc4dff31ca7ec5d62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756571"
---
# <a name="getdelegate"></a>GetDelegate

L’élément **GetDelegate** définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 **GetDelegateType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**IncludePermissions** <br/> |Indique si la réponse contient les paramètres d’autorisation pour chaque utilisateur délégué.  <br/> |
   
#### <a name="includepermissions-attribute-values"></a>Valeurs des attributs IncludePermissions

|**Valeur**|**Description**|
|:-----|:-----|
|**True** <br/> |Déléguer l’utilisateur en plus des informations utilisateur délégué retourné dans l’élément [UserId](userid.md) les autorisations sont renvoyées.  <br/> |
|**False** <br/> |Informations [UserId](userid.md) sont renvoyées.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie la boîte aux lettres de l’entité de sécurité.  <br/> |
|[ID utilisateur](userids.md) <br/> |Contient un tableau d’utilisateurs délégué à obtenir à partir de la boîte aux lettres d’un utilisateur principal. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetDelegate](getdelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

