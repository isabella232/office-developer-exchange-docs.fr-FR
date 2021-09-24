---
title: GetStreamingEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: L’élément GetStreamingEventsResponseMessage contient l’état et le résultat d’une demande d’opération GetStreamingEvents unique.
ms.openlocfilehash: a1af394fa55ab04f42096ebc1c29c879c9cffb9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533426"
---
# <a name="getstreamingeventsresponsemessage"></a>GetStreamingEventsResponseMessage

**L’élément GetStreamingEventsResponseMessage** contient l’état et le résultat d’une demande d’opération [GetStreamingEvents](getstreamingevents-operation.md) unique. 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 **GetStreamingEventsResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état [d’une réponse d’opération GetStreamingEvents.](getstreamingevents-operation.md) <br/><br/>Les valeurs suivantes sont valides pour cet attribut :  <br/><br/>- Réussite  <br/>- Avertissement  <br/>- Erreur  <br/> |
   
#### <a name="responseclass-attribute"></a>Attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|Opération réussie  <br/> |Décrit une demande qui est remplie.  <br/> |
|Avertissement  <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande était en cours de traitement et que les éléments suivants n’ont pas pu être traitées. <br/><br/>Voici quelques exemples de sources d’avertissements :  <br/><br/>- Le magasin Exchange est hors connexion pendant le lot.  <br/>- Les services de domaine Active Directory (AD DS) sont hors connexion.  <br/>- Les boîtes aux lettres ont été déplacées.  <br/>- La base de données de boîtes aux lettres (MDB) est hors connexion.  <br/>- Un mot de passe a expiré.  <br/>- Un quota a été dépassé.  <br/> |
|Erreur  <br/> | Décrit une demande qui ne peut pas être remplie. <br/><br/>Voici quelques exemples de sources d’erreurs :  <br/><br/>- Attributs ou éléments non valides  <br/>- Attributs ou éléments en dehors de la plage  <br/>- Balise inconnue  <br/>- Attribut ou élément non valide dans le contexte  <br/>- Une tentative d’accès non autorisé par un client  <br/>- Une défaillance côté serveur en réponse à un appel côté client valide  <br/><br/>  Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Il contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[Notifications](notifications.md) <br/> |Contient une liste d’informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
|[ErrorSubscriptionIds](errorsubscriptionids.md) <br/> |Contient une liste d’ID d’abonnement non valides.  <br/> |
|[ConnectionStatus](connectionstatus.md) <br/> |Fournit une description texte de l’état d’un abonnement de diffusion en continu.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [GetStreamingEvents](getstreamingevents.md) 
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
- [Opération de GetStreamingEvents](getstreamingevents-operation.md)

