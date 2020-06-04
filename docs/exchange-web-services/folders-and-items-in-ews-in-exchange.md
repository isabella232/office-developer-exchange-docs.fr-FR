---
title: Dossiers et éléments dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 9d8cf6fa-85a4-45ac-8165-e4d3ab92594e
description: Découvrez les dossiers et les éléments de boîte aux lettres, ainsi que la façon dont votre API managée EWS ou votre client EWS les désigne.
localization_priority: Priority
ms.openlocfilehash: 5e206d6973d148c6f70a17a8e7891bf3de7c1533
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455992"
---
# <a name="folders-and-items-in-ews-in-exchange"></a>Dossiers et éléments dans EWS dans Exchange

Découvrez les dossiers et les éléments de boîte aux lettres, ainsi que la façon dont votre API managée EWS ou votre client EWS les désigne.
  
Les dossiers sont l’élément d’organisation d’une boîte aux lettres Exchange. Les dossiers peuvent contenir des éléments de boîte aux lettres, tels que des messages électroniques, des contacts, des rendez-vous, des réunions et des tâches, ou ils peuvent contenir d’autres dossiers. Exchange comprend différents types de dossiers, mais les types de dossiers sont similaires. La principale différence entre elles est le type d’élément qu’elles contiennent.
  
Toutefois, les éléments ont des types uniques. Chaque type d’élément dispose d’un ensemble de propriétés ou de schéma différent pour le définir. Dans cet article, nous allons étudier les types de dossiers et d’éléments disponibles, ainsi que les différences qui existent entre eux.

<a name="bk_folders"> </a>

## <a name="folders"></a>Folders

Les dossiers dérivent tous de la même classe de base ou du même type de base, de la classe de [dossier](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) dans l’API managée EWS ou du type de [dossier](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) dans EWS. La figure suivante illustre les classes de l’API managée EWS et les types EWS. 
  
**Figure 1. Classes de dossier d’API managée EWS et types de dossiers EWS**

![Illustration présentant les classes qui dérivent de la classe de dossier de l’API managée EWS, ainsi que les types qui dérivent du type de dossier EWS, qui sont nommés CalendarFolder, ContactsFolder, SearchFolder et TasksFolder.](media/Ex2013_Folder_OverviewTypes.png)
  
La principale différence entre les classes de dossiers et les types de dossiers réside dans le fait que vous ne pouvez créer qu’un certain type d’élément dans chaque type de dossier. Une autre différence réside dans la façon dont le client affiche les informations dans un dossier. Par exemple, Exchange vous permet de créer des rendez-vous dans le dossier calendrier. Vous pouvez déplacer d’autres types d’éléments dans le dossier calendrier après les avoir créés, mais Outlook ne les affiche pas. Outlook affiche uniquement les éléments de calendrier tels que les rendez-vous et les réunions dans le dossier calendrier, [même si un autre type d’élément existe dans le dossier](folders-and-items-in-ews-in-exchange.md#bk_item). 
  
**Tableau 1. Classes de dossier d’API managée EWS et types de dossiers EWS**

|**Classe d’API managée EWS**|**Type EWS**|**Valeur FolderClass**|**Contains**|**Remarques**|
|:-----|:-----|:-----|:-----|:-----|
|[Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |Page. Note  <br/> |Messages électroniques ou dossiers.  <br/> | Il s’agit de la classe ou du type de dossier générique pour les dossiers [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) d’API managée EWS et les dossiers EWS [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) suivants : <ul><li>  Racine (sous-arborescence IPM)</li><li>NonIpmSubtree</li><li>Boîte de réception</li><li>Éléments supprimés</li><li>Brouillons</li><li>Journal</li><li>Notes  </li><li>Boîte d'envoi</li><li>Éléments envoyés</li><li>Dossier de messages</li><li>Courrier indésirable</li><li>Messagerie vocale</li></ul> |
|[CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](https://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |Page. Rendez-vous  <br/> |Rendez-vous et réunions.  <br/> |Lorsqu’un utilisateur répond à une demande de réunion, le rendez-vous est ajouté à l’API managée EWS [WellKnownFolderName. Calendar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) ou au EWS [DistinguishedFolderId. CalendarFolder](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) uniquement. Il s’agit des seuls dossiers qui prennent en charge l’interaction automatique avec les demandes de réunion et les réponses.  <br/><br/>Ce type de classe de dossier ou de dossier prend en charge l’utilisation des affichages de calendrier pour renvoyer des rendez-vous et des réunions en fonction d’une date de début et d’une date de fin à l’aide de la méthode [Folder. FindItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) et de la classe [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , ou de l’opération EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) et de l’élément [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .  <br/> |
|[ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](https://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |Page. Prenez  <br/> |Contacts et listes de distribution.  <br/> |Aucun.  <br/> |
|[SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |Page. Note  <br/> |Le contenu est déterminé par une restriction ou un filtre. Les dossiers de recherche n’ont pas de sous-dossiers.  <br/> |Les éléments qui répondent aux critères de recherche ne sont pas réellement contenus dans le dossier de recherche ; au lieu de cela, ils se trouvent ailleurs dans la boîte aux lettres.  <br/> Pour vous assurer que les dossiers de recherche sont disponibles dans Outlook, créez-les dans le dossier Finder.  <br/> |
|[TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](https://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |Page. Tâche  <br/> |Contient les éléments de travail à terminer.  <br/> |Aucun.  <br/> |
   
### <a name="folder-structure"></a>Structure de dossiers

Les dossiers fournissent une structure de boîte aux lettres. Cela inclut la sous-arborescence IPM, appelée la partie supérieure de la Banque d’informations dans EWS, dans laquelle la plupart des utilisateurs interagissent avec leur boîte aux lettres, ainsi que les dossiers système que la plupart des utilisateurs ne voient pas, qui se trouvent dans la sous-arborescence non IPM ou dans EWS. La figure suivante illustre la structure de dossiers d’un utilisateur et indique les dossiers qui concernent les éléments de l’utilisateur et ceux qui sont des dossiers système.
  
**Figure 2. Dossiers d’éléments et système dans une boîte aux lettres**

![Illustration présentant les dossiers système à la racine, ce qui comprend les favoris, l’outil de recherche, les données de disponibilité, la partie supérieure de la banque d’informations et bien plus encore. La partie supérieure de la banque d’informations contient les dossiers des utilisateurs, dont leurs calendriers, leurs contacts, etc.](media/Ex2013_Folder_OverviewSampleHierarchy.png)
  
### <a name="well-known-folders"></a>Dossiers bien connus

Parmi les dossiers d’une boîte aux lettres, certains sont des dossiers spéciaux. Elles correspondent à des dossiers connus dans l’API managée EWS ou des dossiers uniques dans EWS. Certains de ces dossiers ont des restrictions sur le nom du dossier, où ils se trouvent dans la structure de dossiers, et s’ils peuvent être supprimés. Les autres dossiers « génériques » (non spéciaux) n’ont pas les mêmes restrictions. Il est important de vous familiariser avec les dossiers connus ou distingués suivants, car il s’agit des dossiers système, utilisateur et de recherche racine, et s’appliquent à la plupart des implémentations. 
  
**Tableau 2. Dossiers principaux connus et uniques**

|**Nom convivial**|**Valeurs **WellKnownFolderName** de l’API MANAGÉe EWS**|**Valeurs **DISTINGUISHEDFOLDERID** EWS**|**Description**|
|:-----|:-----|:-----|:-----|
|Root (sous-arborescence non IPM)  <br/> |WellKnownFolderName. root  <br/> |DistinguishedFolderId. root  <br/> |Contient le dossier racine d’une boîte aux lettres, également appelé sous-arborescence non IPM. Ce dossier n’a pas de parent et vous ne pouvez pas le déplacer, le copier, le renommer ou le supprimer. Chaque magasin de messages contient un seul dossier racine.  <br/> |
|Partie supérieure de la Banque d’informations (sous-arborescence IPM)  <br/> |WellKnownFolderName.MsgFolderRoot  <br/> |DistinguishedFolderId.msgfolderroot  <br/> |Contient la boîte de réception et les autres dossiers utilisateur.  <br/> |
|Finder (dossiers de recherche)  <br/> |WellKnownFolderName. SearchFolders  <br/> |DistinguishedFolderId. SearchFolders.  <br/> |Contient les dossiers de recherche visibles dans Outlook.  <br/> |
   
Pour obtenir la liste complète des valeurs de propriété [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.wellknownfoldername%28v=exchg.80%29.aspx) de l’API managée EWS, voir l’énumération [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) . Pour obtenir la liste complète des valeurs **DISTINGUISHEDFOLDERID** EWS, voir [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx).
  
### <a name="folder-properties"></a>Propriétés des dossiers

Dans l’API managée EWS, les [Propriétés de dossier](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder_properties%28v=exchg.80%29.aspx) sont toutes dérivées de la classe de [dossier](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) de base. Et dans EWS, tous les dossiers utilisent les éléments de dossier qui sont disponibles sur le type de [dossier](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) . La plupart des propriétés et des éléments liés aux dossiers sont simples (ID de dossier parent, nom d’affichage, etc.), mais quelques explications supplémentaires sont nécessaires. 
  
Les avertissements suivants s’appliquent à la propriété de l’API managée EWS [. FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=EXCHG.80%29.aspx) ou à l’élément [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) EWS : 
  
- Si ce paramètre est défini, la valeur de la propriété ou de l’élément doit être conforme à la classe dérivée ou au type du dossier. Par exemple, la propriété ou l’élément **FolderClass** ne peut pas indiquer que le dossier est un dossier de contacts tandis que la classe ou le type du dossier indique que le dossier est un dossier de calendrier. 
    
- Vous pouvez [créer des dossiers](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) d’un type spécifique sans définir la propriété ou l’élément **FolderClass** , ou vous pouvez créer un dossier avec le type de dossier générique et spécifier la propriété ou l’élément **FolderClass** . Les deux options créent le même résultat. 
    
- Après avoir défini la valeur **FolderClass** en créant un type spécifique de dossier ou en définissant la propriété **FolderClass** ou l’élément lui-même, vous ne pouvez pas la modifier. Par exemple, vous ne pouvez pas modifier un IPF. Note dossier en une erreur de page non valide. Dossier de contacts. Toutefois, vous pouvez le remplacer par un IPF. Dossier note. contoso. 
    
- Toute valeur **FolderClass** qui n’utilise pas l’un des préfixes prédéfinis est traitée comme une erreur de page non valide. Dossier de notes. Par exemple, une valeur **FolderClass** de IAmAFolderClass est traitée comme une erreur de page non valide. Dossier de notes. 
    
La valeur de la classe Folder est extensible. Cela signifie que les valeurs **FolderClass** par défaut répertoriées dans le tableau 1 sont traitées comme des préfixes et que vous pouvez ajouter des valeurs personnalisées. Par exemple, vous pouvez créer un dossier avec une valeur **FolderClass** de IPF. Contact. contoso et il est traité comme un dossier de contacts. 
  
Vous pouvez déterminer les autorisations dont dispose le client sur les dossiers, telles que supprimer, lire et modifier, à l’aide de la propriété [Folder. EffectiveRights](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.effectiverights%28v=EXCHG.80%29.aspx) de l’API managée EWS ou de l’élément [EffectiveRights](https://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) EWS. 
  
### <a name="public-folders"></a>Dossiers publics

Les dossiers publics sont conçus pour assurer un accès partagé et offrir une manière simple et efficace de collecter, d’organiser et de partager des informations avec d’autres personnes dans votre groupe de travail ou votre organisation. Vous pouvez également utiliser des dossiers publics pour archiver le contenu du groupe de distribution. Pour obtenir des informations détaillées sur les dossiers publics, consultez la rubrique [Public Folder Access with EWS in Exchange](public-folder-access-with-ews-in-exchange.md).

<a name="bk_hiddenfolders"> </a>

### <a name="hidden-folders"></a>Dossiers cachés

Tous les dossiers créés par Exchange à la racine de la boîte aux lettres sont masqués et vous pouvez utiliser l’API managée EWS ou EWS pour masquer les autres dossiers sous la Banque d’informations. Pour plus d’informations sur les dossiers masqués, consultez la rubrique utilisation [de dossiers masqués à l’aide d’EWS dans Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md). 

<a name="bk_hiddenfolders"> </a>

### <a name="search-folders"></a>Dossiers de recherche

Les dossiers de recherche sont identiques aux dossiers ordinaires, à la seule différence qu’ils ont une propriété ou un élément qui définit le filtre de recherche. Vous pouvez créer des dossiers de recherche dans n’importe quel dossier d’une boîte aux lettres Exchange et les créer de la même manière que vous créez un autre dossier. Toutefois, pour qu’un dossier de recherche apparaisse dans Outlook, Outlook Web App ou Outlook Live, les objets [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) que vous créez à l’aide de l’API managée EWS doivent se trouver dans le dossier [WellKnownFolderName. SearchFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) , et les types [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) que vous créez à l’aide d’EWS doivent se trouver dans le dossier [DistinguishedFolderId. SearchFolders](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Si le dossier de recherche est créé à un autre emplacement, il est toujours disponible et vous pouvez l’afficher dans les applications clientes personnalisées. 

<a name="bk_item"> </a>

## <a name="items"></a>Éléments

EWS dans Exchange utilise des **éléments** pour représenter des messages électroniques individuels, des rendez-vous, des réunions, des contacts, des listes de distribution, des tâches, des publications et d’autres éléments, dans une boîte aux lettres. Les éléments sont fortement typés, ce qui signifie qu’ils ont une classe ou un schéma associé spécifique, ou ne sont pas fortement typés, également appelés éléments génériques. Les éléments génériques sont des objets [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) dans l’API managée EWS et les types d' [éléments](https://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) dans EWS. Les éléments communs, tels que les messages électroniques, les contacts, les listes de distribution, les publications et les tâches, sont fortement typés, et vous pouvez définir des propriétés schématisées spécifiques ou des éléments sur ceux-ci. 
  
**Tableau 3. Éléments fortement typés**

|**Type d’élément d’API managée EWS**|**Élément d’élément EWS**|
|:-----|:-----|
|[Rendez-vous](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contact](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[ContactGroup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |[DistributionList](https://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) <br/> |
|[EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[PostItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |[PostItem](https://msdn.microsoft.com/library/7727ed84-9591-4a1c-bb04-12129926499b%28Office.15%29.aspx) <br/> |
|[Task](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Task](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
API managée EWS les éléments fortement typés dérivent de la classe d' [élément](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx) de base. Toutefois, vous utilisez généralement l’un des types dérivés figurant dans le tableau 3, et non directement avec la classe d' **élément** . Toutefois, lorsque vous utilisez la classe [ItemCollection](https://msdn.microsoft.com/library/dd634001%28v=EXCHG.80%29.aspx) , vous pouvez travailler directement avec des instances de la classe d' **élément** . Dans ce cas, vous devez implémenter une logique qui détermine le type d’élément dans le magasin représenté par l’instance de la classe d' **élément** . Pour utiliser cet élément, vous devez effectuer une liaison à l’élément à l’aide d’une instance de la classe qui représente l’élément. 
  
### <a name="items-in-folders"></a>Éléments dans des dossiers

Certains dossiers ont des restrictions quant aux types d’éléments qu’ils peuvent contenir. Il s’agit de restrictions que la base de données de boîtes aux lettres Exchange applique aux dossiers, et non aux limitations d’affichage client. 
  
**Tableau 4. Restrictions des éléments pour les dossiers**

|**Classe de dossier de l’API managée EWS**|**Type de dossier EWS**|**Restriction**|
|:-----|:-----|:-----|
|[Classe de dossier de base](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer de nouveaux objets [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) de l’API managée EWS et des objets [PostItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) , ou des types de [message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) EWS ou des types de **PostItem** , dans les dossiers génériques. Vous pouvez déplacer d’autres types d’éléments dans des dossiers génériques, mais il se peut que le client ne les affiche pas.  <br/> |
|[CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](https://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer des objets de [rendez-](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) vous de l’API managée EWS et des types [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) EWS dans le dossier de calendrier. Vous pouvez déplacer d’autres types d’éléments dans le dossier calendrier, mais il se peut que le client ne les affiche pas.  <br/> |
|[ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](https://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer de nouveaux objets de [contact](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) et d’API managée EWS, [ou des types](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) de [contacts](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) EWS ou des types [DistributionList](https://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) dans le dossier contacts. Vous pouvez déplacer d’autres types d’éléments dans le dossier contacts, mais il se peut que le client ne les affiche pas.  <br/> |
|[SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |Aucune restriction. Les éléments ne se trouvent pas réellement dans le dossier de recherche ; ils se trouvent ailleurs dans la boîte aux lettres.  <br/> |
|[TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](https://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |Vous pouvez uniquement créer des objets de [tâche](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) de l’API managée EWS ou des types de [tâches](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) EWS dans le dossier tâches. Vous pouvez déplacer d’autres types d’éléments dans le dossier tâches, mais il se peut que le client ne les affiche pas.  <br/> |

<a name="bk_upgrading"> </a>

## <a name="upgrading-from-earlier-product-versions"></a>Mise à niveau à partir de versions antérieures du produit

Les dossiers sont en grande partie restés inchangés dans les versions antérieures et actuelles du produit. Notez toutefois que les versions antérieures d’Exchange utilisent des dossiers gérés pour effectuer la gestion des enregistrements de messagerie (MRM). Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange à partir d’Exchange 2013 utilisent des stratégies de rétention pour MRM. Vous pouvez [mettre à niveau les dossiers gérés pour utiliser des stratégies de rétention](https://technet.microsoft.com/library/dd298032%28v=exchg.150%29.aspx). 
  
Les éléments n’ont pas été modifiés dans les versions antérieures et actuelles du produit.

<a name="bk_inthissection"> </a>

## <a name="in-this-section"></a>Contenu de cette section

- [Utiliser des dossiers à l’aide d’EWS dans Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Utiliser des dossiers masqués à l’aide d’EWS dans Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)
    
- [Utilisations d’éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    
- [Supprimer des éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Exporter et importer des éléments à l’aide d’EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)   
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)   
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

