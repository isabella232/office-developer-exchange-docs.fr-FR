---
title: Les propriétés et les propriétés étendues dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 68623048-060e-4602-b3fa-62617a94cf72
description: Découvrez comment vous pouvez définir et accéder aux propriétés sur les éléments et les dossiers à l’aide de EWS dans Exchange.
ms.openlocfilehash: 0c01d9bd21cbef0a3536c8dbd85e192199b7b8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755066"
---
# <a name="properties-and-extended-properties-in-ews-in-exchange"></a>Les propriétés et les propriétés étendues dans EWS dans Exchange

Découvrez comment vous pouvez définir et accéder aux propriétés sur les éléments et les dossiers à l’aide de EWS dans Exchange.
  
Une boîte aux lettres Exchange contient un grand nombre d’éléments, y compris les messages électroniques, rendez-vous, réunions et ainsi de suite. Ces éléments sont composés de propriétés. les propriétés décrivent les éléments. Vous pouvez utiliser les propriétés de l’élément pour effectuer une [recherche](search-and-ews-in-exchange.md), [synchroniser les modifications de l’élément](mailbox-synchronization-and-ews-in-exchange.md)et [créer des types de propriété personnalisée](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a). Cet article fournit une vue d’ensemble de propriétés et comment vous pouvez utiliser les propriétés dans votre application.
  
## <a name="exchange-item-properties"></a>Propriétés de l’élément Exchange
<a name="ItemsAreProperties"> </a>

Éléments et les dossiers dans Exchange sont essentiellement des lignes de tableaux. La propriété principale qui identifie un élément ou un dossier est son [identificateur EWS](ews-identifiers-in-exchange.md). Bien que les autres propriétés de l’identificateur dans la base de données Exchange, pour EWS, l’identificateur EWS joue le rôle de la clé primaire de la collection de propriétés qui décrivent un élément. La propriété identificateur EWS comprend deux parties :
  
- Une propriété [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ou [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) qui identifie l’élément 
    
- Modification d’une propriété **ChangeKey** qui contient des informations d’état sur si un élément ou un dossier 
    
Tous les éléments dans une boîte aux lettres sont stockés dans la même base de données Exchange et utilisent le même schéma de base de données. Éléments sont distinguent par une combinaison de la propriété [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) , contraintes de la propriété et les couches de logique métier qui affectent la façon dont ils sont gérés dans l’échange de stocker. Le tableau 1 présente la façon dont les propriétés sont appliquées entre les différents types d’éléments ; Dans cet exemple, le courrier électronique et rendez-vous les éléments. Les deux éléments ont la valeur de la propriété [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) . Mais, notez que la propriété [IsAllDayEvent](http://msdn.microsoft.com/library/29140a64-9d7a-4a14-a10d-c98197c9831b%28Office.15%29.aspx) n’est pas définie sur l’élément de courrier électronique et que la propriété **IsReadReceiptRequested** n’est pas définie sur le rendez-vous. Heureusement, vous n’avez pas besoin de connaître les propriétés qui sont applique à chaque classe de l’élément ; EWS gère pour vous. 
  
**Le tableau 1. Comparaison des propriétés de rendez-vous et au courrier électronique**

|**Type d’élément**|**Classe de l’élément**|**Objet**|**IsAllDayEvent**|**IsReadReceiptRequested**|
|:-----|:-----|:-----|:-----|:-----|
|Courier électronique  <br/> |IPM. Remarque  <br/> |Rapport d’état : effectuer de projet X  <br/> |NULL  <br/> |true  <br/> |
|Rendez-vous  <br/> |IPM.Appointment  <br/> |Réunion de la société Contoso  <br/> |false  <br/> |NULL  <br/> |
   
Le schéma EWS prend en charge la plupart des contraintes gérées par la base de données Exchange et les couches de logique métier entre EWS et la base de données Exchange. Le schéma EWS s’applique défini un ensemble de propriétés pour chaque type d’élément. Les éléments de base de données d’Exchange fortement typées fournies par EWS sont les suivantes : 
  
- Messages électroniques
    
- Rendez-vous
    
- Contacts
    
- Listes de distribution
    
- Messages de réunion
    
- Demandes de rendez-vous
    
- Demandes de réunion
    
- Annulations de rendez-vous
    
- Tâches
    
- Publier des éléments
    
Éléments génériques sont renvoyées par EWS en tant que messages électroniques. L’API managée EWS implémente tous ces types d’éléments.
  
> [!NOTE]
> Objets de réponse sont envoyées uniquement par le client au serveur en réponse à des éléments provenant d’autres personnes. Ils n’existent pas dans la base de données Exchange. 
  
## <a name="what-are-properties-in-ews"></a>Que sont les propriétés dans les services EWS ?
<a name="WhatAreEWSProperties"> </a>

Le schéma EWS décrit les données échangées entre un client EWS et un Exchange. Une grande partie du schéma décrit les propriétés d’élément et le dossier que vous pouvez accéder à la base de données Exchange. Le schéma EWS décrit la représentation XML des propriétés de base de données Exchange qui sont disponibles pour votre application. Les propriétés, les propriétés sont disponibles, ils forme prendre et les valeurs qu’elles renvoient, varient en fonction de ce que vous essayez de faire. Par exemple, la propriété **Body** renvoie uniquement les premiers 512 caractères dans une opération **FindItem** , mais l’opération **GetItem** renvoie le texte complet de l’élément. Bien que la plupart des propriétés sont définies et récupérables, certaines propriétés sont définies uniquement par Exchange. Chaque propriété existe dans le schéma au format XML que soit reflète la propriété qu’il est stocké dans la base de données Exchange ou est calculé à partir des propriétés stockées dans la base de données Exchange. La propriété **Subject** est un exemple d’une propriété définissable ; la propriété **UnreadCount** sur un dossier est un exemple d’une propriété calculée. Un ensemble de propriétés sont courants pour les types d’éléments principaux. 
  
Les facteurs suivants déterminent que la propriété la valeur que votre application obtient à partir d’Exchange : 
  
- L’opération qui appelle votre application
    
- La forme de base de réponse
    
- Le type d’élément
    
- Les chemins d’accès de la propriété spécifiée
    
Il est important de comprendre comment ces différents facteurs qui affectent les données que vous pouvez accéder. Comme avec l’exemple de la propriété **Body** mentionnée plus haut, certaines informations sont disponibles conditionnellement en fonction de différents facteurs. Compréhension de ces facteurs peuvent gagner du temps en vous permettant de choisir les options appropriées pour accéder aux informations que vous souhaitez. Pour découvrir les propriétés qui sont accessibles, vous devez tester ces facteurs pour déterminer comment accéder aux propriétés nécessaires à votre application. Cette section décrit comment ces différents facteurs qui affectent les propriétés retournées dans les réponses EWS. 
  
### <a name="ews-response-shapes"></a>Formes d’intervention EWS

Exchange enregistre une grande quantité d’informations sur les éléments. Parfois, votre application ne doit pas toutes ces informations, et dans de nombreux cas, il est préférable de ne pas tout. [Formes d’intervention EWS](property-sets-and-response-shapes-in-ews-in-exchange.md), également appelée formes de propriété, indiquez les propriétés retournées à partir du serveur. L’élément principal de la forme de réponse est la forme de base. Une forme de base est un conteneur des propriétés prédéfinies par défaut pour les éléments fortement typées. L’équivalent d’API managées de la forme de base est la [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx). EWS inclut trois formes de réponse par défaut.
  
**Le tableau 2. Formes de réponse par défaut**

|**Nom de forme de réponse par défaut**|**Équivalent de l’API managée EWS**|**Description**|
|:-----|:-----|:-----|
|IdOnly  <br/> |Valeur BasePropertySet.IdOnly  <br/> |Uniquement les identificateur EWS et modifier la clé sont renvoyées. Sauf si le client utilise toutes les propriétés renvoyées par la forme AllProperties ou par défaut, utilisez la forme IdOnly et spécifier des propriétés supplémentaires en utilisant le chemin d’accès de la propriété définie sur la classe **PropertySet** . La plupart des applications doivent utiliser la forme de réponse IdOnly avec les propriétés supplémentaires spécifiées. Cela réduit la quantité de données inutilisées demandées par les clients.  <br/> |
|Default (Défaut)  <br/> |S/O  <br/> |Un ensemble de propriétés standards pour le type d’élément. Utilisez uniquement cette forme de réponse si votre application utilise toutes les propriétés.  <br/> |
|AllProperties  <br/> |Valeur BasePropertySet.FirstClassProperties  <br/> |Un plus grand ensemble de propriétés à la forme par défaut. Bien que le nom l’indique, cette option ne retourne toutes les propriétés sur un élément. Ce jeu de propriétés renvoie les propriétés des applications clientes plus souvent utilisent. Si vous avez besoin des propriétés supplémentaires, vous pouvez leur demander par leur chemin d’accès de la propriété.  <br/> Si votre application n’utilise pas toutes les propriétés renvoyées avec cette forme de réponse, utilisez la forme de réponse IdOnly avec les propriétés supplémentaires spécifiées.  <br/> |
   
De nombreuses opérations EWS renvoient des éléments et leurs propriétés. Les formes de réponse que vous spécifiez, indépendamment de différentes opérations peuvent renvoyer des jeux de propriétés différentes. Différents types d’éléments aussi renvoyer des propriétés différentes, en fonction de l’opération et la forme de réponse spécifié. Les opérations suivantes les formes d’intervention permet d’identifier les propriétés à renvoyer.
  
**Le tableau 3. Opérations qui utilisent des formes de réponse**

|**Opération EWS**|**Méthode d'API managée EWS**|
|:-----|:-----|
|[GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |
|[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |[Méthode Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |
|[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |[Méthode Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |
|[FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |
|[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |[Méthode Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |
|[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |[Méthode Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Non implémenté.  <br/> |
|[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.ResolveNames](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.SearchMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService.BeginSearchMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsearchmailboxes%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
Formes de propriété sont une élémentaire de façon à identifier les propriétés que vous souhaitez que votre application pour renvoyer. Toutefois, votre application doit parfois, un ensemble de propriétés spécifiques plus précis. Pour ce faire, vous pouvez utiliser le chemin d’accès de la propriété.
  
### <a name="choose-properties-by-their-property-path"></a>Sélectionnez les propriétés par leur chemin d’accès de la propriété

Un chemin d’accès de la propriété EWS est métadonnées qui sert à identifier les propriétés dans une demande ou une réponse. 
  
**Le tableau 4. Types de propriétés de chemin d’accès**

|**Type de chemin d’accès de propriété**|**Type de schéma**|**Implémentation de l’API managée EWS**|**Description**|
|:-----|:-----|:-----|:-----|
|FieldUri  <br/> |PathToUnindexedFieldType  <br/> |Types qui héritent de [ServiceObjectSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobjectschema%28v=exchg.80%29.aspx).  <br/> |Le chemin d’accès de la propriété les plus courants. Chemins d’accès de la propriété FieldUri sont spécifiés dans un objet **PropertySet** dans l’API managée EWS. La plupart des propriétés EWS peut être spécifié par le chemin d’accès de la propriété FieldUri. Ceci est décrit par le UnindexedFieldURIType dans le schéma EWS.  <br/> Le chemin d’accès de la propriété FieldUri XML ressemble à ceci :  <br/> ```XML<FieldURI FieldURI="item:Subject"/>```Ce chemin d’accès de la propriété est l’équivalent de ItemSchema.Subject dans l’API managée EWS.  <br/> |
|IndexedFieldUri  <br/> |PathToIndexedFieldType  <br/> |Types qui héritent de [ItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx).  <br/> |Identifie les propriétés de dictionnaire qui nécessitent un index de propriété pour spécifier la valeur à renvoyer. Utilisez ce chemin d’accès lorsqu’une propriété peut avoir plusieurs valeurs. Ceci est décrit par la propriété **DictionaryURIType** dans le schéma EWS. Chemins d’accès de la propriété **DictionaryURIType** sont spécifiés dans un objet **PropertySet** dans l’API managée EWS.  <br/> Le chemin d’accès de la propriété IndexedFieldUri XML ressemble à ceci :  <br/> ```XML<IndexedFieldURI FieldURI="contacts:PhysicalAddress:Street FieldIndex="Home"/>```|
|ExtendedFieldUri  <br/> |PathToExtendedFieldType  <br/> |[ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Identifie une définition de la propriété étendue qui identifie les propriétés personnalisées ou non schématisé sur les éléments.  <br/> Le chemin d’accès de la propriété ExtendedFieldUri XML ressemble à ceci :  <br/> ```XML<ExtendedFieldURI> PropertyTag="0x1234" PropertyType="Integer" />```|
|ExceptionFieldUri  <br/> |ExceptionFieldURI  <br/> |[ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) <br/> |Spécifie les propriétés qui sont associées à une erreur dans une réponse EWS. Ceci est décrit par le type de **ExceptionPropertyURIType** dans le schéma EWS. Cela se produit uniquement dans l’élément **MessageXml** de réponses d’erreur qui se produisent lorsque vous travaillez avec des périodicités de calendrier.  <br/> |
   
Meilleure pratique, lorsque vous demandez des propriétés, utilisez la forme de base IdOnly ([BasePropertySet.IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) dans l’API managée EWS), puis demandez uniquement les propriétés de votre application a besoin en spécifiant les chemins d’accès de la propriété. 
  
### <a name="schematized-properties"></a>Propriétés schématisées

La plupart des propriétés qui a besoin de votre client EWS est décrits dans le schéma EWS. Le dossier principal et les définitions de type d’élément qui contient les définitions de propriétés, sont trouvent dans le schéma types.xsd. Les types de schémas suivants contiennent les définitions de propriété pour la plupart des objets que vous pouvez utiliser.
  
**Tableau 5. Types de schémas qui contiennent des définitions de propriétés**

|**Type de schéma EWS**|**Équivalent de type API managées**|**Définit le...**|
|:-----|:-----|:-----|
|**ItemType** <br/> |[Classe de l’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) <br/> |Propriété de type d’élément de base définie. Ce type peut être créé à partir d’un client, mais n’est jamais retourné par Exchange. Exchange renvoie un objet MessageType pour tous les objets génériques.  <br/> |
|**MessageType** <br/> |[Classe EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de l’objet de message et la propriété pour tous les objets génériques de messagerie.  <br/> |
|**CalendarItemType** <br/> |[Classe de rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |Propriété d’élément de calendrier défini ; Cela inclut les rendez-vous uniques et périodiques.  <br/> |
|**ContactItemType** <br/> |[Classe de contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés d’élément de contact.  <br/> |
|**DistributionListType** <br/> |[Classe ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de liste de distribution personnelle.  <br/> |
|**MeetingMessageType** <br/> |[Classe MeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingmessage%28v=exchg.80%29.aspx) <br/> |Propriété de type de réunion défini.  <br/> |
|**MeetingRequestMessageType** <br/> |[Classe MeetingRequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type de demande de réunion.  <br/> |
|**MeetingResponseMessageType** <br/> |[Classe MeetingResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingresponse%28v=exchg.80%29.aspx) <br/> |Propriété de type de réponse de réunion défini.  <br/> |
|**MeetingCancellationMessageType** <br/> |[Classe MeetingCancellation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingcancellation%28v=exchg.80%29.aspx) <br/> |Valeur de la propriété type de l’annulation de réunion.  <br/> |
|**TaskType** <br/> |[Classe de tâche](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type de tâche.  <br/> |
|**PostItemType** <br/> |[PostItem, classe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type PostItem.  <br/> |
|**FolderType** <br/> |[Classe d’un dossier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés du type de dossier.  <br/> |
|**CalendarFolderType** <br/> |[Classe CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type SearchFolder.  <br/> |
|**ContactsFolderType** <br/> |[Classe ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type ContactsFolder.  <br/> |
|**SearchFolderType** <br/> |[Classe SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type SearchFolder.  <br/> |
|**TasksFolderType** <br/> |[Classe du dossier tâches](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type dossier tâches.  <br/> |
|**UserConfigurationType** <br/> |[Classe UserConfiguration](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type UserConfiguration.  <br/> |
   
Alors que les propriétés dans le schéma EWS suffisent pour de nombreuses applications, vous ne peut pas implémenter quelques scénarios à l’aide d’uniquement ce qui est décrit dans le schéma. Pour ces scénarios, vous pouvez les propriétés étendues. 
  
### <a name="extended-properties-aka-non-schematized-properties"></a>Propriétés étendues (également appelées propriétés non schématisé)

Les propriétés étendues permettent de créer des propriétés personnalisées, qui vous permettent d’accéder aux propriétés d’éléments et des dossiers dans la banque d’informations Exchange qui ne sont pas définis dans le schéma EWS. Vous pouvez utiliser les pour accéder native MAPI élément et le dossier des propriétés dans la base de données Exchange. Vous pouvez utiliser les propriétés étendues pour accéder à toutes les propriétés schématisées, car dans les coulisses, ces propriétés schématisées sont tout simplement des propriétés MAPI dans la base de données Exchange. 
  
Le type de schéma PathToExtendedFieldType, situé dans le schéma types.xsd, définit le code XML qui représente une propriété étendue. Ce type de schéma définit l’élément [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) dans les instances XML ; en d’autres termes, elle définit le code XML qui est envoyé entre le service et le client. Le type de schéma ExtendedPropertyType définit l’élément [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) et la valeur ou tableau de valeurs qui contient une propriété étendue. Le tableau suivant montre le mappage de la propriété étendue XML approximatif et son implémentation sur des éléments de l’API managée EWS. 
  
**Le tableau 6. Propriété étendue XML telle qu’implémentée dans l’API managée EWS**

|**Implémentation de l’API managée EWS**|**Ce qu’elle contient**|**Qu’il correspond à**|
|:-----|:-----|:-----|
|[Propriété Item.ExtendedProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |Une collection de propriétés étendues sur un élément.  <br/> |Une ou plusieurs instances de propriétés étendues sur un élément.  <br/> |
|[Classe ExtendedProperty](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedproperty%28v=exchg.80%29.aspx) <br/> |La définition de la propriété étendue et les valeurs.  <br/> |Le type de schéma ExtendedPropertyType.  <br/> |
|[Classe ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Une définition de la propriété étendue.  <br/> |Le type de schéma PathToExtendedFieldType.  <br/> |
   
Si vous souhaitez en savoir plus sur la façon dont vous pouvez utiliser les propriétés étendues dans votre application, vous pouvez explorer les exemples de code suivants : 
  
- [MFCMapi](http://mfcmapi.codeplex.com/)
    
- [Exchange 2013 : Mettre en service les en-têtes X personnalisés par programme](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Exchange 2013 : Accéder à une propriété sa balise de propriété](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-719875ac)
    
- [Exchange 2013 : Accéder à une propriété nommée par son identificateur](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-02dbe22f)
    
- [Exchange 2013 : Accéder à une propriété nommée par son nom](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-6556e183)
    
- [Exchange 2013 : Accéder à un nom et le GUID du jeu à la propriété](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-4021f971)
    
- [Exchange 2013 : Créer des propriétés étendues par programme](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)
    
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Mettre en service les en-têtes x à l’aide de EWS dans Exchange](how-to-provision-x-headers-by-using-ews-in-exchange.md)
    
- [Erreurs liées à la propriété EWS](ews-property-related-errors.md)
    
## <a name="see-also"></a>Voir aussi


- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [MFCMapi](http://mfcmapi.codeplex.com/)
    

