---
title: CreateManagedFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolderResponseMessage
api_type:
- schema
ms.assetid: a72eefc3-ef0b-4b44-a74b-e6907b5b5f68
description: L’élément CreateManagedFolderResponseMessage contient l’État et le résultat d’une seule demande d’opération CreateManagedFolder.
ms.openlocfilehash: 03ebcaeb79b2fac20882d2cea3d1e24b42dd472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467703"
---
# <a name="createmanagedfolderresponsemessage"></a>CreateManagedFolderResponseMessage

L’élément **CreateManagedFolderResponseMessage** contient l’État et le résultat d’une seule demande d' [opération CreateManagedFolder](createmanagedfolder-operation.md) . 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
  
```xml
<CreateManagedFolderResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CreateManagedFolderResponseMessage>
```

**FolderInfoResponseMessageType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Décrit l’état d’une réponse d' [opération CreateManagedFolder](createmanagedfolder-operation.md) .<br/><br/>Les valeurs suivantes sont valides pour cet attribut :<br/><br/>-Réussite  <br/>-AVERTISSEMENT  <br/>-Erreur  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|**Success** <br/> |Décrit une demande qui est satisfaite.  <br/> |
|**Warning** <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite lors du traitement d’un élément dans la demande et que les éléments suivants n’ont pas pu être traités.<br/><br/>Voici des exemples de sources d’avertissements :<br/><br/>-La banque Exchange est hors connexion pendant le traitement par lots.  <br/>-Les services de domaine Active Directory (AD DS) sont hors connexion.  <br/>-Les boîtes aux lettres sont déplacées.  <br/>-La base de données de messages (MDB) est hors connexion.  <br/>-Un mot de passe a expiré.  <br/>-Un quota est dépassé.  <br/> |
|**Error** <br/> | Décrit une demande qui ne peut pas être satisfaite.<br/><br/>Voici des exemples de sources d’erreurs :  <br/><br/>-Attributs ou éléments non valides  <br/>-Les attributs ou les éléments sont en dehors de la plage  <br/>-Balise inconnue  <br/>-Attribut ou élément non valide dans le contexte  <br/>-Tentative d’accès non autorisée par un client  <br/>-Échec côté serveur en réponse à un appel côté client valide<br/><br/>  Vous trouverez des informations sur l’erreur dans les éléments [ResponseCode](responsecode.md) et [MessageText](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et est réservé à une utilisation ultérieure. Il contient une valeur de 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
|[Dossiers](folders-ex15websvcsotherref.md) <br/> |Contient un tableau de dossiers gérés créés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contient les messages de réponse pour une demande des services Web Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération CreateManagedFolder](createmanagedfolder-operation.md)
- [Référence EWS pour Exchange](ews-reference-for-exchange.md) 
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

