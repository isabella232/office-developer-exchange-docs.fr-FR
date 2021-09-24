---
title: SyncFolderItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderItemsResponseMessage
api_type:
- schema
ms.assetid: f58e773f-94a7-4729-90f0-ac4c71b4ba59
description: L’élément SyncFolderItemsResponseMessage contient l’état et le résultat d’une demande d’opération SyncFolderItems unique.
ms.openlocfilehash: c11f896c2d9f0dec498a4e2048aa78d17da33d0e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531438"
---
# <a name="syncfolderitemsresponsemessage"></a>SyncFolderItemsResponseMessage

**L’élément SyncFolderItemsResponseMessage** contient l’état et le résultat d’une demande [d’opération SyncFolderItems](syncfolderitems-operation.md) unique. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md)
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
```xml
<SyncFolderItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastItemInRange/>
   <Changes/>
</SyncFolderItemsResponseMessage>
```

 **SyncFolderItemsResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état [d’une réponse d’opération SyncFolderItems.](syncfolderitems-operation.md) <br/><br/>Les valeurs suivantes sont valides pour cet attribut : <br/> <br/>- Réussite  <br/>- Avertissement  <br/>- Erreur  <br/> |
   
#### <a name="responseclass-attribute"></a>Attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est remplie.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants ne peuvent pas être traitées. <br/><br/>Voici quelques exemples de sources d’avertissements :  <br/><br/>- Le magasin Exchange est hors connexion pendant le lot.  <br/>- Les services de domaine Active Directory (AD DS) sont hors connexion.  <br/>- Les boîtes aux lettres ont été déplacées.  <br/>- La base de données de messages (MDB) est hors connexion.  <br/>- Un mot de passe a expiré.  <br/>- Un quota a été dépassé.  <br/> |
|**Erreur** <br/> | Décrit une demande qui ne peut pas être remplie. <br/><br/>Voici quelques exemples de sources d’erreurs :  <br/><br/>- Attributs ou éléments non valides  <br/>- Attributs ou éléments en dehors de la plage  <br/>- Balise inconnue  <br/>- Attribut ou élément non valide dans le contexte  <br/>- Toute tentative d’accès non autorisé par un client  <br/>- Toute défaillance côté serveur en réponse à un appel côté client valide  <br/>  <br/>Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Il contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contient une forme codée en base 64 des données de synchronisation qui est mise à jour après chaque demande réussie. Il est utilisé pour identifier l’état de synchronisation.  <br/> |
|[IncludesLastItemInRange](includeslastiteminrange.md) <br/> |Indique si le dernier élément à synchroniser a été inclus dans la réponse.  <br/> |
|[Modifications (éléments)](changes-items.md) <br/> |Contient un tableau de séquences de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur Exchange serveur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande Exchange services Web.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération SyncFolderItems](syncfolderitems-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

