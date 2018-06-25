---
title: FindPeopleResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: L’élément FindPeopleResponse spécifie la réponse à une demande de FindPeople.
ms.openlocfilehash: 4f2c2f6069a515d5153ea488b35182d8b35f029f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756417"
---
# <a name="findpeopleresponse"></a>FindPeopleResponse

L’élément **FindPeopleResponse** spécifie la réponse à une demande de **FindPeople** . 
  
```XML
<FindPeopleResponse ResponseClass=" Success | Warning | Error ">
    <People/>
    <TotalNumberOfPeopleInView/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindPeopleResponse>
```

 **FindPeopleResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ResponseClass  <br/> |Spécifie la classe de la réponse.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|Opération réussie  <br/> |Indique la réussite.  <br/> |
|Avertissement  <br/> |Indique un avertissement.  <br/> |
|Erreur  <br/> |Indique une erreur.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Personnes](people.md) <br/> |Spécifie un tableau de données personnage renvoyées à la suite d’une demande **FindPeople** .  <br/> |
|[TotalNumberOfPeopleInView](totalnumberofpeopleinview.md) <br/> |Spécifie le nombre total de personnages stockés sur un serveur qui sont renvoyées par une requête **FindPeople** .  <br/> |
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit des informations d’état sur la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisée et réservée à un usage ultérieur.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations de réponse d’erreur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Spécifie un tableau de messages de réponse.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

