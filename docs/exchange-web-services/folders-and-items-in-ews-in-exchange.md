---
title: Dossiers et éléments dans les services EWS d’Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d8cf6fa-85a4-45ac-8165-e4d3ab92594e
description: Découvrez les dossiers et éléments de boîte aux lettres et comment votre API managées ou votre client EWS représente les.
ms.openlocfilehash: a3358844f2317c9b0462456ff7d2f38442c98ee3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754802"
---
# <a name="folders-and-items-in-ews-in-exchange"></a>Dossiers et éléments dans les services EWS d’Exchange

Découvrez les dossiers et éléments de boîte aux lettres et comment votre API managées ou votre client EWS représente les.
  
Les dossiers sont l’élément organisationnel d’une boîte aux lettres Exchange. Les dossiers peuvent contenir des éléments de boîte aux lettres, telles que les messages électroniques, contacts, rendez-vous, réunions et tâches, ou ils peuvent contenir d’autres dossiers. Exchange comprend les différents types de dossiers, mais les types de dossiers sont similaires. La principale différence entre eux est le type d’élément qu’ils contiennent.
  
Éléments, toutefois, ont types uniques. Chaque type d’élément dispose d’un ensemble différent de propriétés ou du schéma pour le définir. Dans cet article, aborder les types de dossiers et éléments qui sont disponibles et les différences entre eux.

<a name="bk_folders"> </a>

## <a name="folders"></a>Dossiers

Tous les dossiers dérivent de la même classe de base ou type de base, la classe de [dossier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) dans l’API managée EWS ou le type de [dossier](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans EWS. La figure suivante illustre les classes d’API managées et les types EWS. 
  
**La figure 1. Classes de dossier API managées et les types de dossiers EWS**

![Illustration présentant les classes qui dérivent de la classe de dossier de l’API managée EWS, ainsi que les types qui dérivent du type de dossier EWS, qui sont nommés CalendarFolder, ContactsFolder, SearchFolder et TasksFolder.](media/Ex2013_Folder_OverviewTypes.png)
  
La principale différence entre les types de dossier et chacune des classes de dossier est que vous pouvez uniquement créer un certain type d’élément dans chaque type de dossier. Comment le client affiche des informations dans un dossier sont une des autres différences. Par exemple, Exchange vous permet de créer un rendez-vous dans le dossier calendrier. Vous pouvez déplacer des autres types d’éléments dans le dossier calendrier après leur création, mais Outlook ne les affiche. Outlook affiche uniquement les éléments de calendrier telles que des rendez-vous et réunions dans le dossier calendrier, [même si un autre type d’élément existe dans le dossier](folders-and-items-in-ews-in-exchange.md#bk_item). 
  
**Le tableau 1. Classes de dossier API managées et les types de dossiers EWS**

|**Classe de l’API managée EWS**|**Type EWS**|**Valeur de la classe FolderClass**|**Contient**|**Remarques**|
|:-----|:-----|:-----|:-----|:-----|
|[Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |ERREUR. Remarque  <br/> |Messages électroniques ou des dossiers.  <br/> | Il s’agit de la classe de dossier générique ou d’un type pour les dossiers d’API managées [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) suivants et EWS [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) : <ul><li>  Racine (sous-arborescence IPM)</li><li>NonIpmSubtree</li><li>Inbox</li><li>Éléments supprimés</li><li>Brouillons</li><li>Journal</li><li>Remarques  </li><li>La boîte d’envoi</li><li>Éléments envoyés</li><li>Dossier de message</li><li>Courrier indésirable</li><li>Messagerie vocale</li></ul> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |ERREUR. Rendez-vous  <br/> |Rendez-vous et réunions.  <br/> |Lorsqu’un utilisateur répond à une demande de réunion, le rendez-vous est ajouté à l' API managée EWS [WellKnownFolderName.Calendar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) ou [DistinguishedFolderId.CalendarFolder](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) de des EWS uniquement. Ce sont les seuls dossiers qui prennent en charge l’interaction de demandes de réunion et les réponses automatique.  <br/><br/>Cette classe d’un dossier ou un type de dossier prend en charge les vues de calendrier pour renvoyer des rendez-vous et réunions en fonction des dates de début et une date de fin à l’aide de la méthode API managées [Folder.FindItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) et la classe [CalendarView](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) ou la [FindItem EWS ](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)opération et l’élément [CalendarView](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .  <br/> |
|[ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |ERREUR. Contact  <br/> |Listes de distribution et des contacts.  <br/> |Aucun.  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |ERREUR. Remarque  <br/> |Contenu est déterminé par une restriction ou un filtre. Dossiers de recherche n’ont pas de sous-dossiers.  <br/> |Les éléments qui répondent aux critères de recherche ne sont pas réellement contenus dans le dossier de recherche ; au lieu de cela, ils se trouvent ailleurs dans la boîte aux lettres.  <br/> Pour vous assurer que les dossiers de recherche sont disponibles dans Outlook, les créer dans le dossier de recherche.  <br/> |
|[Dossier tâches](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[Dossier tâches](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |ERREUR. Tâche  <br/> |Contient des éléments de travail à effectuer.  <br/> |Aucun.  <br/> |
   
### <a name="folder-structure"></a>Structure de dossiers

Dossiers fournissent une structure de boîte aux lettres. Cela inclut la sous-arborescence IPM, appelés à la partie supérieure de banque d’informations dans EWS, où la plupart des utilisateurs interagissent avec leur boîte aux lettres, ainsi que les dossiers système qui ne voient jamais la plupart des utilisateurs, qui se trouvent dans la sous-arborescence Non-IPM ou racine dans EWS. La figure suivante montre la structure de dossiers d’un utilisateur et indique les dossiers pour les éléments de l’utilisateur et qui sont des dossiers système.
  
**La figure 2. Élément et le système de dossiers dans une boîte aux lettres**

![Illustration présentant les dossiers système à la racine, ce qui comprend les favoris, l’outil de recherche, les données de disponibilité, la partie supérieure de la banque d’informations et bien plus encore. La partie supérieure de la banque d’informations contient les dossiers des utilisateurs, dont leurs calendriers, leurs contacts, etc.](media/Ex2013_Folder_OverviewSampleHierarchy.png)
  
### <a name="well-known-folders"></a>Dossiers connus

Les dossiers dans une boîte aux lettres, certains sont des dossiers spéciaux. Ils correspondent aux dossiers connus dans l’API managée EWS, ou des dossiers uniques dans EWS. Certains de ces dossiers ont des restrictions sur le nom du dossier où ils se trouvent dans la structure de dossiers et si elles peuvent être supprimés. Autres dossiers (non spécial) « génériques » n’ont pas les mêmes restrictions. Il est important pour vous familiariser avec les dossiers suivants connus ou uniques, car elles sont la racine système, utilisateur et les dossiers de recherche et sont appliquent à la plupart des implémentations. 
  
**Le tableau 2. Dossiers connus et uniques principaux**

|**Nom convivial**|**Valeurs d’API managées **WellKnownFolderName****|**Valeurs **DistinguishedFolderId** EWS**|**Description**|
|:-----|:-----|:-----|:-----|
|Racine (Non-IPM sous-arborescence)  <br/> |WellKnownFolderName.Root  <br/> |DistinguishedFolderId.root  <br/> |Contient le dossier racine d’une boîte aux lettres, également connu sous la sous-arborescence Non-IPM. Ce dossier n’a pas de parent, et vous ne pouvez pas déplacer, copier, renommer ou supprimer. Chaque banque de messages ne contient qu’un seul dossier racine.  <br/> |
|Haut de la banque d’informations (sous-arborescence IPM)  <br/> |WellKnownFolderName.MsgFolderRoot  <br/> |DistinguishedFolderId.msgfolderroot  <br/> |Contient la boîte de réception et d’autres dossiers de l’utilisateur.  <br/> |
|Finder (dossiers de recherche)  <br/> |WellKnownFolderName.SearchFolders  <br/> |DistinguishedFolderId.searchfolders.  <br/> |Contient des dossiers de recherche sont visibles dans Outlook.  <br/> |
   
Pour obtenir une liste complète des valeurs de propriété d’API managées [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.wellknownfoldername%28v=exchg.80%29.aspx) , voir l’énumération [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) . Pour obtenir une liste complète des valeurs EWS **DistinguishedFolderId** , voir [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx).
  
### <a name="folder-properties"></a>Propriétés de dossier

Dans l’API managée EWS, les [Propriétés de dossier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder_properties%28v=exchg.80%29.aspx) sont dérivées de la classe de [dossier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) de base. Et dans les services EWS, tous les dossiers utilisent les éléments du dossier qui sont disponibles sur le type de [dossier](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) . La plupart des propriétés associés à des dossiers et éléments sont simple (ID du dossier parent, nom complet et ainsi de suite), mais nécessitent quelques explications supplémentaires. 
  
Les restrictions suivantes s’appliquent à la propriété API managées [Folder.FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=EXCHG.80%29.aspx) ou l’élément EWS [classe FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) : 
  
- Si set, la valeur de l’élément ou la propriété doit correspondre à la classe dérivée ou le type du dossier. Par exemple, la propriété de la **classe FolderClass** ou l’élément ne peut pas indiquer que le dossier est un dossier de Contacts lors de la classe ou le type du dossier indique le dossier est un dossier de calendrier. 
    
- Vous pouvez soit [créer des dossiers](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) d’un type spécifique sans définir la propriété de la **classe FolderClass** ou d’un élément, ou vous pouvez créer un dossier avec le type de dossier générique et spécifier la propriété de la **classe FolderClass** ou d’un élément. Les deux options créent le même résultat. 
    
- Une fois que vous définissez la valeur de la **classe FolderClass** en créant un type spécifique d’un dossier ou en définissant la propriété de la **classe FolderClass** ou l’élément lui-même, vous ne pouvez pas le modifier. Par exemple, vous ne pouvez pas modifier une défaillance de page. Remarque le dossier à une défaillance de page. Dossier de contacts. Vous pouvez, toutefois, le modifier à une défaillance de page. Dossier Note.Contoso. 
    
- N’importe quelle valeur de la **classe FolderClass** qui n’utilise pas un des préfixes prédéfinis est traitée comme une défaillance de page. Dossier Notes. Par exemple, une valeur de la **classe FolderClass** de IAmAFolderClass est traitée comme une défaillance de page. Dossier Notes. 
    
La valeur de classe de dossier est extensible. Cela signifie que la **classe FolderClass** par défaut répertoriée dans le tableau 1 est traitée comme des préfixes et que vous pouvez ajouter des valeurs personnalisées. Par exemple, vous pouvez créer un dossier avec une valeur de **classe FolderClass** de l’erreur. Contact.Contoso et il est traité comme un dossier Contacts. 
  
Vous pouvez déterminer ce que le client dispose sur les dossiers, tels que des autorisations suppriment, lire et modifier, à l’aide de la propriété API managées [Folder.EffectiveRights](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.effectiverights%28v=EXCHG.80%29.aspx) ou l’élément EWS [EffectiveRights](http://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) . 
  
### <a name="public-folders"></a>Dossiers publics

Les dossiers publics sont conçus pour un accès partagé et offrent un moyen simple et efficace de collecter, organiser et partager des informations avec d’autres personnes de votre groupe de travail ou d’une organisation. Vous pouvez également utiliser des dossiers publics pour archiver le contenu de groupe de distribution. Pour obtenir des informations détaillées sur les dossiers publics, voir [accéder aux dossiers publics avec EWS dans Exchange](public-folder-access-with-ews-in-exchange.md).

<a name="bk_hiddenfolders"> </a>

### <a name="hidden-folders"></a>Dossiers cachés

Tous les dossiers créés à la racine de la boîte aux lettres Exchange sont masquées et vous pouvez utiliser les API managées EWS pour masquer des dossiers sous le haut de la banque d’informations supplémentaires. Pour plus d’informations sur les dossiers cachés, voir [utilisation des dossiers cachés à l’aide de EWS dans Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md). 

<a name="bk_hiddenfolders"> </a>

### <a name="search-folders"></a>Dossiers de recherche

Dossiers de recherche sont à l’instar des dossiers standard, sauf qu’elles possèdent une propriété ou élément qui définit le filtre de recherche. Vous pouvez créer des dossiers de recherche dans n’importe quel dossier dans une boîte aux lettres Exchange, et vous les créez de la même manière que vous créez un autre dossier. Toutefois, pour un dossier de recherche apparaisse dans Outlook, Outlook Web App ou Outlook Live, objets [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) que vous créez à l’aide de l’API managée EWS doivent se trouver dans le dossier [WellKnownFolderName.SearchFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) les types que vous créez à l’aide de EWS doivent se trouver dans le dossier [DistinguishedFolderId.SearchFolders](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Si le dossier de recherche est créé dans un autre emplacement, il est toujours disponible et vous pouvez l’afficher dans des applications clientes personnalisées. 

<a name="bk_item"> </a>

## <a name="items"></a>Éléments

EWS dans Exchange utilise les **éléments** pour représenter des messages électroniques individuels, rendez-vous, réunions, contacts, listes de distribution, tâches, billets et autres éléments, dans une boîte aux lettres. Les éléments sont que soit fortement typée, ce qui signifie qu’ils possèdent une classe associée spécifique ou schéma ou éléments pas fortement typées, également appelé génériques. Éléments génériques sont des objets [d’éléments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) dans les types d’API managées et [élément](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) dans EWS. Les éléments courants comme les messages électroniques, contacts, listes de distribution, billets et tâches sont fortement typées, et vous pouvez définir des propriétés schématisées spécifiques ou des éléments sur les. 
  
**Le tableau 3. Éléments fortement typées**

|**Type d’élément API managées**|**Élément EWS**|
|:-----|:-----|
|[Rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |[DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) <br/> |
|[EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Objet postItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |[Objet postItem](http://msdn.microsoft.com/library/7727ed84-9591-4a1c-bb04-12129926499b%28Office.15%29.aspx) <br/> |
|[Tâche](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Tâche](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
API managée EWS fortement typées éléments dériver de la classe [d’élément de](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx) base. Toutefois, vous travaillez généralement avec un des types dérivés répertoriés dans le tableau 3 et non à la classe de **l’élément** directement. Lorsque vous travaillez avec la classe [ItemCollection](http://msdn.microsoft.com/en-us/library/dd634001%28v=EXCHG.80%29.aspx) , toutefois, vous pouvez travailler avec des instances de la classe de **l’élément** . Dans ce cas, vous devez implémenter la logique qui détermine le type d’élément dans le magasin qui représente l’instance de la classe de **l’élément** . Pour travailler avec cet élément, vous devez lier à l’élément à l’aide d’une instance de la classe qui représente l’élément. 
  
### <a name="items-in-folders"></a>Éléments dans les dossiers

Certains dossiers ont des restrictions sur les types d’éléments qu’ils renferment. Il s’agit des restrictions de la base de données de boîtes aux lettres Exchange s’applique aux dossiers, pas les limitations d’affichage client. 
  
**Le tableau 4. Élément restrictions pour les dossiers**

|**Classe du dossier des API gérée EWS**|**Type de dossier EWS**|**Restriction**|
|:-----|:-----|:-----|
|[Classe de dossier de base](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer des objets d’API managées [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) et objets [PostItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) , ou EWS [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) types ou **PostItem** , dans les dossiers génériques. Vous pouvez déplacer des autres types d’éléments dans des dossiers génériques, mais le client ne peut pas les afficher.  <br/> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer des nouveaux objets de l' API managée EWS [rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) et EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) types dans le dossier calendrier. Vous pouvez déplacer des autres types d’éléments dans le dossier calendrier, mais le client ne peut pas les afficher.  <br/> |
|[ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer des nouveaux objets de l’API managée EWS [Contact](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) et [ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) ou types EWS [Contact](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) ou [DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) types dans le dossier Contacts. Vous pouvez déplacer des autres types d’éléments dans le dossier Contacts, mais le client ne peut pas afficher les  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |Aucune restriction. Éléments ne se trouvent pas réellement dans le dossier de recherche ; ils se trouvent ailleurs dans la boîte aux lettres.  <br/> |
|[Dossier tâches](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[Dossier tâches](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer des nouveaux objets de l' API managée EWS [tâche](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) ou types EWS [tâche](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) dans le dossier tâches. Vous pouvez déplacer des autres types d’éléments dans le dossier tâches, mais le client ne peut pas afficher les  <br/> |

<a name="bk_upgrading"> </a>

## <a name="upgrading-from-earlier-product-versions"></a>Mise à niveau à partir de versions antérieures du produit

Dossiers sont pour l’essentiel restés inchangés dans les versions antérieures et en cours. Notez que les versions antérieures d’Exchange utilisent les dossiers gérés pour effectuer la gestion des enregistrements de messagerie (MRM). Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2013 utiliser des stratégies de rétention pour MRM. Vous pouvez la [mise à niveau des dossiers à utiliser des stratégies de rétention gérés](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.150%29.aspx). 
  
Éléments n’ont pas changé dans les versions antérieures et en cours.

<a name="bk_inthissection"> </a>

## <a name="in-this-section"></a>In this section

- [Utilisation de dossiers à l’aide de EWS dans Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Utilisation de dossiers cachés à l’aide de EWS dans Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)
    
- [Travailler avec des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    
- [Supprimer des éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Exporter et importer des éléments à l’aide de EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)   
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)   
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

