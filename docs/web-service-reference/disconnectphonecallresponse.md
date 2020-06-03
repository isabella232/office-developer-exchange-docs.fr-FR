---
title: DisconnectPhoneCallResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCallResponse
api_type:
- schema
ms.assetid: 05041799-5b81-4b87-ada8-ce6c506ffe01
description: L’élément DisconnectPhoneCallResponse contient l’État et le résultat d’une seule requête DisconnectPhoneCall.
ms.openlocfilehash: 6c0696a1d9ab3242920d051b409105644a6b03aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458445"
---
# <a name="disconnectphonecallresponse"></a>DisconnectPhoneCallResponse

L’élément **DisconnectPhoneCallResponse** contient l’État et le résultat d’une seule requête **DisconnectPhoneCall** . 
  
```xml
<DisconnectPhoneCallResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DisconnectPhoneCallResponse>
```

 **DisconnectPhoneCallResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état de la réponse.<br/><br/>Les valeurs suivantes sont valides pour cet attribut :  <br/><br/>-Réussite  <br/>-AVERTISSEMENT  <br/>-Erreur  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est satisfaite.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.<br/><br/>Voici des exemples de sources d’avertissements :<br/><br/>-La banque Exchange est hors connexion pendant le traitement par lots.  <br/>-Les services de domaine Active Directory (AD DS) sont hors connexion.  <br/>-Les boîtes aux lettres ont été déplacées.  <br/>-La base de données de messages (MDB) est hors connexion.  <br/>-Un mot de passe a expiré.  <br/>-Un quota a été dépassé.  <br/> |
|**Error** <br/> | Décrit une demande qui ne peut pas être satisfaite.<br/><br/>Voici des exemples de sources d’erreurs :  <br/><br/>-Attributs ou éléments non valides  <br/>-Les attributs ou les éléments qui sont en dehors de la plage  <br/>-Balise inconnue  <br/>-Un attribut ou un élément qui n’est pas valide dans le contexte  <br/>-Une tentative d’accès non autorisée par un client  <br/>-Un échec côté serveur en réponse à un appel côté client valide<br/><br/>  Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Cet élément contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

