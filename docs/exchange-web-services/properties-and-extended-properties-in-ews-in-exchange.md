---
title: Les propriétés et les propriétés étendues dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 68623048-060e-4602-b3fa-62617a94cf72
description: Découvrez comment vous pouvez définir et accéder aux propriétés sur les éléments et les dossiers à l’aide d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 0891cf6d6dddf74518fbbc8efbaebdd8eb0c706b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459334"
---
# <a name="properties-and-extended-properties-in-ews-in-exchange"></a>Les propriétés et les propriétés étendues dans EWS dans Exchange

Découvrez comment vous pouvez définir et accéder aux propriétés sur les éléments et les dossiers à l’aide d’EWS dans Exchange.
  
Une boîte aux lettres Exchange contient un grand nombre d’éléments, notamment des messages électroniques, des rendez-vous, des réunions, etc. Ces éléments sont constitués de propriétés ; les propriétés décrivent les éléments. Vous pouvez utiliser les propriétés de l’élément pour effectuer une [recherche](search-and-ews-in-exchange.md), [synchroniser les modifications des éléments](mailbox-synchronization-and-ews-in-exchange.md)et [créer des types de propriétés personnalisées](https://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a). Cet article fournit une vue d’ensemble des propriétés et de la façon dont vous pouvez utiliser les propriétés dans votre application.
  
## <a name="exchange-item-properties"></a>Propriétés d’élément Exchange
<a name="ItemsAreProperties"> </a>

Les éléments et les dossiers dans Exchange sont essentiellement des lignes dans des tableaux. La propriété main qui identifie un élément ou un dossier est son [identificateur EWS](ews-identifiers-in-exchange.md). Bien qu’il existe d’autres propriétés liées à l’identificateur dans la base de données Exchange, pour EWS, l’identificateur EWS agit comme la clé primaire de la collection de propriétés qui décrivent un élément. La propriété de l’identificateur EWS contient deux parties :
  
- Une propriété [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ou [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) qui identifie l’élément 
    
- Une propriété **ChangeKey** qui contient des informations d’État permettant de savoir si un élément ou un dossier a été modifié. 
    
Tous les éléments d’une boîte aux lettres sont stockés dans la même base de données Exchange et utilisent le même schéma de base de données. Les éléments se distinguent par une combinaison de la propriété [ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) , des contraintes de propriété et des couches de logique métier qui influent sur la façon dont elles sont gérées dans la Banque d’informations Exchange. Le tableau 1 illustre la façon dont les propriétés sont appliquées à différents types d’éléments ; dans cet exemple, les éléments de messagerie et de rendez-vous. Les deux éléments ont une valeur pour la propriété [Subject](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) . Toutefois, Notez que la propriété [IsAllDayEvent](https://msdn.microsoft.com/library/29140a64-9d7a-4a14-a10d-c98197c9831b%28Office.15%29.aspx) n’est pas définie sur l’élément email et que la propriété **IsReadReceiptRequested** n’est pas définie sur le rendez-vous. Heureusement, vous n’avez pas besoin de savoir quelles propriétés sont applicables pour chaque classe d’élément ; EWS le gère pour vous. 
  
**Tableau 1. Comparaison des propriétés de rendez-vous et de messagerie**

|**Type d’élément**|**Classe d’élément**|**Subject**|**IsAllDayEvent**|**IsReadReceiptRequested**|
|:-----|:-----|:-----|:-----|:-----|
|E-mail  <br/> |Mn. Note  <br/> |Rapport d’État : projet X terminé  <br/> |VALEURS  <br/> |true  <br/> |
|Rendez-vous  <br/> |Mn. Rendez-vous  <br/> |Réunion contoso Company  <br/> |false  <br/> |VALEURS  <br/> |
   
Le schéma EWS prend en charge de nombreuses contraintes gérées par la base de données Exchange et les couches de logique métier entre EWS et la base de données Exchange. Le schéma EWS applique un ensemble défini de propriétés à chaque type d’élément. Les éléments de base de données Exchange fortement typés fournis par EWS sont les suivants : 
  
- Messages électroniques
    
- Rendez-vous
    
- Contacts
    
- Listes de distribution
    
- Messages de réunion
    
- Demandes de réunion
    
- Réponses aux réunions
    
- Annulations de rendez-vous
    
- Tâches
    
- Publier des éléments
    
Les éléments génériques sont renvoyés par EWS sous forme de messages électroniques. L’API managée EWS implémente tous ces types d’éléments.
  
> [!NOTE]
> Les objets de réponse sont envoyés uniquement par le client au serveur en réponse à des éléments reçus d’autres personnes. Elles n’existent pas dans la base de données Exchange. 
  
## <a name="what-are-properties-in-ews"></a>Qu’est-ce que les propriétés dans EWS ?
<a name="WhatAreEWSProperties"> </a>

Le schéma EWS décrit les données envoyées entre un client EWS et Exchange. Une partie importante du schéma décrit les propriétés d’élément et de dossier auxquelles vous pouvez accéder dans la base de données Exchange. Le schéma EWS décrit la représentation XML des propriétés de base de données Exchange qui sont disponibles pour votre application. Les propriétés réelles, dont les propriétés sont disponibles, le formulaire qu’elles prennent et les valeurs qu’elles renvoient, varient en fonction de ce que vous essayez de faire. Par exemple, la propriété **Body** renverra uniquement les premiers 512 caractères d’une opération **FindItem** , mais l’opération **GetItem** renvoie le texte intégral de l’élément. Bien que la plupart des propriétés soient toutes les deux définissables et récupérables, certaines propriétés ne sont définies que par Exchange. Chaque propriété existe dans le schéma dans un format XML qui reflète la propriété telle qu’elle est stockée dans la base de données Exchange ou est calculé à partir des propriétés stockées dans la base de données Exchange. La propriété **Subject** est un exemple de propriété définissable ; la propriété **UnreadCount** sur un dossier est un exemple de propriété calculée. Un jeu de propriétés principal est commun aux types d’éléments principaux. 
  
Les facteurs suivants déterminent le jeu de propriétés que votre application obtient à partir d’Exchange : 
  
- L’opération que votre application appelle
    
- Forme de la réponse de base
    
- Type d’élément
    
- Les chemins de propriétés spécifiés
    
Il est important de comprendre comment ces différents facteurs affectent les données auxquelles vous pouvez accéder. Comme dans l’exemple de la propriété **Body** mentionnée précédemment, certaines informations sont conditionnellement disponibles en fonction de différents facteurs. La compréhension de ces facteurs peut vous faire gagner du temps en vous aidant à choisir les options appropriées pour accéder aux informations de votre choix. Pour savoir quelles propriétés sont accessibles, vous devrez tester ces facteurs afin de déterminer comment accéder aux propriétés dont votre application a besoin. Cette section explique comment ces différents facteurs affectent les propriétés renvoyées dans les réponses EWS. 
  
### <a name="ews-response-shapes"></a>Formes de réponse EWS

Exchange stocke un grand nombre d’informations sur les éléments. Parfois, votre application n’a pas besoin de toutes ces informations, et dans de nombreux cas, il est préférable de ne pas tout obtenir. Les [formes de réponse EWS](property-sets-and-response-shapes-in-ews-in-exchange.md), également appelées formes de propriétés, indiquent les propriétés qui sont renvoyées à partir du serveur. L’élément fondamental de la forme de réponse est la forme de base. Une forme de base est un conteneur de propriétés prédéfini par défaut pour les éléments fortement typés. L’API managée EWS équivalente à la forme de base est l' [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx). EWS comprend trois formes réponse par défaut.
  
**Tableau 2. Formes de réponse par défaut**

|**Nom de la forme de réponse par défaut**|**Équivalent de l’API managée EWS**|**Description**|
|:-----|:-----|:-----|
|IdOnly  <br/> |Valeur BasePropertySet. IdOnly  <br/> |Seul l’identificateur EWS et la clé de modification sont renvoyés. À moins que le client utilise toutes les propriétés retournées par la AllProperties ou la forme par défaut, utilisez la forme IdOnly et spécifiez des propriétés supplémentaires en utilisant le chemin d’accès de la propriété défini sur la classe **PropertySet** . La plupart des applications doivent utiliser la forme de réponse IdOnly avec des propriétés supplémentaires spécifiées. Cela permet de réduire la quantité de données inutilisées demandées par les clients.  <br/> |
|Par défaut  <br/> |N/A  <br/> |Ensemble de propriétés standard pour le type d’élément. Utilisez uniquement cette forme de réponse si votre application utilise toutes les propriétés.  <br/> |
|AllProperties  <br/> |Valeur BasePropertySet. FirstClassProperties  <br/> |Un plus grand ensemble de propriétés que la forme par défaut. Bien que le nom le indique, cette option ne renvoie pas toutes les propriétés d’un élément. Ce jeu de propriétés renvoie les propriétés que les applications clientes utilisent le plus souvent. Si vous avez besoin de propriétés supplémentaires, vous pouvez les demander par leur chemin d’accès à la propriété.  <br/> Si votre application n’utilise pas toutes les propriétés renvoyées avec cette forme de réponse, utilisez la forme de réponse IdOnly avec des propriétés supplémentaires spécifiées.  <br/> |
   
De nombreuses opérations EWS renvoient des éléments et leurs propriétés. Quelles que soient les formes de réponse que vous spécifiez, différentes opérations peuvent renvoyer des jeux de propriétés différents. Différents types d’éléments renvoient également différentes propriétés, en fonction de l’opération et de la forme de la réponse spécifiée. Les opérations suivantes utilisent des formes réponse pour identifier les propriétés à renvoyer.
  
**Tableau 3. Opérations qui utilisent des formes réponse**

|**Opération EWS**|**Méthode d'API managée EWS**|
|:-----|:-----|
|[GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |
|[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |[Méthode Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |
|[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |[Méthode Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService. BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |
|[FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. FindConversation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |
|[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |[Méthode Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |
|[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |[Méthode Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |
|[FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Non implémenté.  <br/> |
|[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. ResolveNames](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. SearchMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> [Méthode ExchangeService. BeginSearchMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsearchmailboxes%28v=exchg.80%29.aspx) <br/> |
|[Opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. Opérationsyncfolderhierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Méthode ExchangeService. SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
Les formes de propriétés constituent une méthode rudimentaire pour identifier les propriétés que vous souhaitez que votre application renvoie. Toutefois, dans certains cas, votre application a besoin d’un ensemble plus précis de propriétés spécifiques. Pour ce faire, vous pouvez utiliser le chemin d’accès à la propriété.
  
### <a name="choose-properties-by-their-property-path"></a>Choisir les propriétés par leur chemin d’accès de propriété

Un chemin d’accès de propriété EWS est des métadonnées qui permettent d’identifier les propriétés dans une demande ou une réponse. 
  
**Tableau 4. Types de chemins de propriétés**

|**Type de chemin de propriété**|**Type de schéma**|**Implémentation de l’API managée EWS**|**Description**|
|:-----|:-----|:-----|:-----|
|FieldUri  <br/> |PathToUnindexedFieldType  <br/> |Types qui héritent de [ServiceObjectSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobjectschema%28v=exchg.80%29.aspx).  <br/> |Chemin d’accès de la propriété le plus courant. Les chemins de propriété FieldUri sont spécifiés sur un objet **PropertySet** dans l’API managée EWS. La plupart des propriétés EWS peuvent être spécifiées par le chemin d’accès de la propriété FieldUri. Cette description est décrite par le UnindexedFieldURIType dans le schéma EWS.  <br/> Le code XML de la propriété FieldUri se présente comme suit :  <br/> ```XML<FieldURI FieldURI="item:Subject"/>```Le chemin d’accès de cette propriété est l’équivalent de ItemSchema. Subject dans l’API managée EWS.  <br/> |
|IndexedFieldUri  <br/> |PathToIndexedFieldType  <br/> |Types qui héritent de [ItemSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx).  <br/> |Identifie les propriétés de dictionnaire qui nécessitent un index de propriété pour spécifier la valeur à renvoyer. Utilisez ce chemin d’accès lorsqu’une propriété peut avoir plusieurs valeurs. Cette description est décrite par la propriété **DictionaryURIType** dans le schéma EWS. Les chemins de propriété **DictionaryURIType** sont spécifiés sur un objet **PROPERTYSET** dans l’API managée EWS.  <br/> Le code XML de la propriété IndexedFieldUri se présente comme suit :  <br/> ```XML<IndexedFieldURI FieldURI="contacts:PhysicalAddress:Street FieldIndex="Home"/>```|
|ExtendedFieldUri  <br/> |PathToExtendedFieldType  <br/> |[ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Identifie une définition de propriété étendue qui identifie des propriétés personnalisées ou non schématisées sur des éléments.  <br/> Le code XML de la propriété ExtendedFieldUri se présente comme suit :  <br/> ```XML<ExtendedFieldURI> PropertyTag="0x1234" PropertyType="Integer" />```|
|ExceptionFieldUri  <br/> |ExceptionFieldURI  <br/> |[ServiceResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) <br/> |Spécifie les propriétés qui sont associées à une erreur dans une réponse EWS. Cette description est décrite par le type **ExceptionPropertyURIType** dans le schéma EWS. Cela se produit uniquement dans l’élément **messagexml** des réponses d’erreur qui se produit lorsque vous utilisez des périodicités de calendrier.  <br/> |
   
Pour une meilleure pratique, lorsque vous demandez des propriétés, utilisez la forme de base IdOnly ([BasePropertySet. IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) dans l’API managée EWS), puis demandez uniquement les propriétés dont votre application a besoin en spécifiant les chemins d’accès des propriétés. 
  
### <a name="schematized-properties"></a>Propriétés schématisées

La plupart des propriétés dont votre client EWS a besoin sont décrites par le schéma EWS. Les définitions de dossiers et de types d’éléments principaux, qui contiennent les définitions de propriétés, se trouvent dans le schéma types. xsd. Les types de schéma suivants contiennent les définitions de propriétés pour la plupart des objets que vous pouvez utiliser.
  
**Tableau 5. Types de schéma contenant des définitions de propriétés**

|**Type de schéma EWS**|**Équivalent du type d’API managée EWS**|**Définit le...**|
|:-----|:-----|:-----|
|**ItemType** <br/> |[Classe d’élément](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) <br/> |Propriété du type d’élément de base. Ce type peut être créé à partir d’un client, mais n’est jamais retourné par Exchange. Exchange renvoie un objet MessageType pour tous les objets génériques.  <br/> |
|**MessageType** <br/> |[Classe EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |Propriété de l’objet message électronique et jeu de propriétés pour tous les objets génériques.  <br/> |
|**CalendarItemType** <br/> |[Classe de rendez-vous](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés d’élément de calendrier ; Cela inclut les rendez-vous uniques et périodiques.  <br/> |
|**ContactItemType** <br/> |[Classe contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés d’élément de contact.  <br/> |
|**DistributionListType** <br/> |[Classe ContactGroup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de liste de distribution personnelle.  <br/> |
|**MeetingMessageType** <br/> |[Classe MeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingmessage%28v=exchg.80%29.aspx) <br/> |Propriété de type de message de réunion définie.  <br/> |
|**MeetingRequestMessageType** <br/> |[Classe propriété meetingrequest](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest%28v=exchg.80%29.aspx) <br/> |Propriété de type de demande de réunion définie.  <br/> |
|**MeetingResponseMessageType** <br/> |[Classe MeetingResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingresponse%28v=exchg.80%29.aspx) <br/> |Propriété de type réponse de réunion définie.  <br/> |
|**MeetingCancellationMessageType** <br/> |[Classe MeetingCancellation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingcancellation%28v=exchg.80%29.aspx) <br/> |Propriété du type d’annulation de réunion définie.  <br/> |
|**TaskType** <br/> |[Classe de tâche](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |Propriété Task type définie.  <br/> |
|**PostItemType** <br/> |[Classe PostItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |Propriété de type PostItem définie.  <br/> |
|**FolderType** <br/> |[Classe Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |Propriété de type de dossier définie.  <br/> |
|**CalendarFolderType** <br/> |[Classe CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type SearchFolder.  <br/> |
|**ContactsFolderType** <br/> |[Classe ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |Propriété de type ContactsFolder définie.  <br/> |
|**SearchFolderType** <br/> |[Classe SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |Jeu de propriétés de type SearchFolder.  <br/> |
|**TasksFolderType** <br/> |[Classe TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |Propriété de type TasksFolder définie.  <br/> |
|**UserConfigurationType** <br/> |[Classe UserConfiguration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration%28v=exchg.80%29.aspx) <br/> |Propriété de type UserConfiguration définie.  <br/> |
   
Bien que les propriétés du schéma EWS soient suffisantes pour de nombreuses applications, vous ne pouvez pas implémenter certains scénarios à l’aide uniquement des éléments décrits dans le schéma. Pour ces scénarios, vous pouvez étendre les propriétés. 
  
### <a name="extended-properties-aka-non-schematized-properties"></a>Propriétés étendues (propriétés non schématisées)

Les propriétés étendues vous permettent de créer des propriétés personnalisées, qui vous permettent d’accéder à des propriétés sur des éléments et des dossiers de la Banque d’Exchange qui ne sont pas définis dans le schéma EWS. Vous pouvez les utiliser pour accéder aux propriétés de dossier et d’élément MAPI native dans la base de données Exchange. Vous pouvez utiliser les propriétés étendues pour accéder à toutes les propriétés schématisées, car dans les coulisses, ces propriétés schématisées ne sont rien de plus que les propriétés MAPI dans la base de données Exchange. 
  
Le type de schéma PathToExtendedFieldType, situé dans le schéma types. xsd, définit le code XML qui représente une propriété étendue. Ce type de schéma définit l’élément [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) dans les instances XML ; en d’autres termes, elle définit le code XML qui est envoyé entre le service et le client. Le type de schéma ExtendedPropertyType définit à la fois l’élément [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) et la valeur ou le tableau de valeurs qu’une propriété étendue contient. Le tableau suivant montre le mappage approximatif de la propriété étendue XML et son implémentation sur les éléments de l’API managée EWS. 
  
**Tableau 6. Extended Property XML tel qu’implémenté dans l’API managée EWS**

|**Implémentation de l’API managée EWS**|**Éléments qu’elle contient**|**Éléments sur lesquels elle est mappée**|
|:-----|:-----|:-----|
|[Propriété Item. ExtendedProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |Collection de propriétés étendues sur un élément.  <br/> |Une ou plusieurs instances de propriétés étendues sur un élément.  <br/> |
|[Classe ExtendedProperty](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedproperty%28v=exchg.80%29.aspx) <br/> |Définition et valeurs de la propriété étendue.  <br/> |Type de schéma ExtendedPropertyType.  <br/> |
|[Classe ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Définition de propriété étendue.  <br/> |Type de schéma PathToExtendedFieldType.  <br/> |
   
Si vous souhaitez en savoir plus sur l’utilisation des propriétés étendues dans votre application, vous pouvez explorer les exemples de code suivants : 
  
- [MFCMapi](http://mfcmapi.codeplex.com/)
    
- [Exchange 2013 : mise en service des en-têtes X personnalisés par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Exchange 2013 : accéder à une propriété par sa balise de propriété](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-719875ac)
    
- [Exchange 2013 : accéder à une propriété nommée par son identificateur](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-02dbe22f)
    
- [Exchange 2013 : accéder à une propriété nommée par son nom](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-6556e183)
    
- [Exchange 2013 : accéder à une propriété par le GUID et le nom d’un jeu de propriétés](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-4021f971)
    
- [Exchange 2013 : créer des propriétés étendues personnalisées par programme](https://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)
    
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Mise en service des en-têtes x à l’aide d’EWS dans Exchange](how-to-provision-x-headers-by-using-ews-in-exchange.md)
    
- [Erreurs liées aux propriétés EWS](ews-property-related-errors.md)
    
## <a name="see-also"></a>Voir aussi


- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [MFCMapi](http://mfcmapi.codeplex.com/)
    

