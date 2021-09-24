---
title: ResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: L’élément ResponseMessage fournit des informations descriptives sur l’état de réponse d’une seule entité au sein d’une demande.
ms.openlocfilehash: 21db84698b693fc97c67285c8ca89da028b4e59b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516371"
---
# <a name="responsemessage"></a>ResponseMessage

**L’élément ResponseMessage** fournit des informations descriptives sur l’état de réponse d’une seule entité dans une demande. 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 **ResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ResponseClass** <br/> | Représente l’état de la réponse. <br/><br/>Les valeurs suivantes sont valides pour cet attribut :  <br/><br/>- Réussite  <br/>- Avertissement  <br/>- Erreur  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Valeurs d’attribut ResponseClass

|**Valeur**|**Description**|
|:-----|:-----|
|Opération réussie  <br/> |Décrit une demande qui est remplie.  <br/> |
|Avertissement  <br/> | Décrit une demande qui n’a pas été traitée. Un avertissement peut être renvoyé si une erreur s’est produite alors qu’un élément de la demande était en cours de traitement et que les éléments suivants n’ont pas pu être traitées. <br/><br/>Voici quelques causes possibles des avertissements :  <br/><br/>- Le magasin Exchange est hors connexion pendant le lot.  <br/>- Le service d’annuaire Active Directory est hors connexion.  <br/>- Les boîtes aux lettres sont déplacées.  <br/>- La base de données de messages (MDB) est hors connexion.  <br/>- Un mot de passe a expiré.  <br/>- Un quota est dépassé.  <br/> |
|Erreur  <br/> | Décrit une demande qui ne peut pas être remplie. <br/><br/>Les causes possibles des erreurs sont les suivantes :  <br/><br/>- Attributs ou éléments non valides  <br/>- Attributs ou éléments en dehors de la plage  <br/>- Balise inconnue  <br/>- Attribut ou élément non valide dans le contexte  <br/>- Tentative d’accès non autorisé par un client  <br/>- Défaillance côté serveur en réponse à un appel côté client valide  <br/> <br/> Des informations sur l’erreur se trouvent dans les éléments [ResponseCode](responsecode.md) et [MessageText.](messagetext.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Actuellement inutilisé et réservé à une utilisation ultérieure. Il contient la valeur 0.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fournit des informations supplémentaires sur la réponse aux erreurs.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Contient les informations de libre/occupé d’un utilisateur de boîte aux lettres unique. <br/> <br/> Voici l’expression XPath 2.0 à cet élément : <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[SuggestionsResponse](suggestionsresponse.md) <br/> |Contient des informations de réponse et des données de suggestion pour les suggestions de réunion demandées.  <br/><br/> Voici l’expression XPath 2.0 à cet élément :<br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contient les résultats de la réponse et les paramètres d’absence du travail d’un utilisateur.  <br/><br/> Voici l’expression XPath 2.0 à cet élément :  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[SetUserOofSettingsResponse](setuseroofsettingsresponse.md) <br/> |Contient le résultat d’une tentative de message [SetUserOofSettingsRequest.](setuseroofsettingsrequest.md) <br/> <br/> Voici l’expression XPath 2.0 à cet élément :  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Remarques

Le type **ResponseMessageType** est commun à toutes les Exchange des services Web. Le type **ResponseMessageType** est étendu par les types complexes suivants : 
  
- **ApplyConversationActionResponseMessageType**
    
- **AttachmentInfoResponseMessageType**
    
- **DeleteAttachmentResponseMessageType**
    
- **DeleteItemResponseMessageType**
    
- **ExpandDLResponseMessageType**
    
- **FindFolderResponseMessageType**
    
- **FindItemResponseMessageType**
    
- **FolderInfoResponseMessageType**
    
- **GetEventsResponseMessageType**
    
- **ItemInfoResponseMessageType**
    
- **ResolveNamesResponseMessageType**
    
- **SubscribeResponseMessageType**
    
- **SendNotificationResponseMessageType**
    
- **SyncFolderHierarchyResponseMessageType**
    
- **SyncFolderItemsResponseMessageType**
    
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
### <a name="version-differences"></a>Différences entre les versions

Les types **ApplyConversationActionResponseMessage** et **DeleteItemResponseMessageType** ont été introduits dans Exchange build 15.00.0986.00. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)
- [Opération GetUserOofSettings](getuseroofsettings-operation.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

