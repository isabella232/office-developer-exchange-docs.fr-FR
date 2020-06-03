---
title: Accéder aux dossiers publics avec EWS dans Exchange
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: Découvrez comment utiliser EWS et l’API managée EWS pour accéder aux dossiers publics et acheminer les demandes de dossiers publics dans Exchange.
localization_priority: Priority
ms.openlocfilehash: e921a77b250e11e974b0c47b1d28a8e020837d44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460210"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Accéder aux dossiers publics avec EWS dans Exchange

Découvrez comment utiliser EWS et l’API managée EWS pour accéder aux dossiers publics et acheminer les demandes de dossiers publics dans Exchange.
  
Les dossiers publics fournissent un référentiel partagé des éléments auxquels les utilisateurs de votre organisation peuvent accéder. Office 365, Exchange Online et les versions locales d’Exchange à partir d’Exchange 2013 introduisent une nouvelle architecture pour les dossiers publics. Les dossiers publics dans Exchange utilisent une conception de boîte aux lettres spécialisée (au lieu d’une base de données de dossiers publics) pour stocker la hiérarchie de dossiers publics et le contenu des dossiers publics. Les autorisations de dossiers publics sont gérées via le contrôle d’accès basé sur un rôle (RBAC).
  
Les technologies d’accès client, telles que les services Web Exchange (EWS) et l’API managée EWS, fournissent un accès par programme à la hiérarchie de dossiers publics et aux éléments de contenu d’une base de données de dossiers publics. Cet article fournit des informations sur la façon dont vous pouvez utiliser EWS et l’API managée EWS pour accéder aux dossiers publics et aux dossiers publics et aux données de dossiers publics. 
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>Opérations EWS et méthodes de l’API managée EWS pour l’accès aux dossiers publics
<a name="bk_functionality"> </a>

La plupart des opérations EWS de base prennent en charge l’accès aux dossiers publics. Vous pouvez utiliser les opérations de dossier et d’élément, ainsi que les méthodes de l’API managée EWS indiquées dans le tableau suivant, pour travailler avec des dossiers publics.
  
Pour plus d’informations sur les méthodes de l’API managée EWS, consultez la rubrique [EWS Managed API Namespaces](https://msdn.microsoft.com/library/jj220535%28v=exchg.80%29.aspx).
  
|**Opération EWS**|**Méthode d'API managée EWS**|
|:-----|:-----|
|[Opération CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder. Save ()** <br/> |
|[Opération UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder. Update ()** <br/> |
|[Opération DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder. Delete ()** <br/> |
|[Opération MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)<sup>1</sup> <br/> |**Folder. Move ()** <br/> |
|[CopyFolder opération](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx)<sup>2</sup> <br/> |**Folder. Copy ()** <br/> |
|[Opération GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder. bind ()** <br/> |
|[Opération EmptyFolder](https://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx)<sup>3</sup> <br/> |**Folder. Empty ()** <br/> |
|[Opération FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService. FindFolders ()** <br/> **Folder. FindFolders ()** <br/> |
|[Opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item. Save ()** <br/> |
|[Opération MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item. Move ()** <br/> |
|[Opération CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item. Copy ()** <br/> |
|[Opération UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item. Update ()** <br/> |
|[Opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item. Delete ()** <br/> |
|[Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)<sup>4</sup> <br/> |**ExchangeService. FindItems ()** <br/> **Folder. FindItems ()** <br/> |
|[Opération GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item. bind ()** <br/> |
|[Opération ConvertId](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)<sup>5</sup> <br/> |**ExchangeService. ConvertId ()** <br/> **ExchangeService. ConvertIds ()** <br/> |
   
<sup>1</sup> le transfert de dossiers entre un dossier public et un dossier privé n’est pas disponible dans les versions d’Exchange commençant par Exchange 2013. 
  
<sup>2</sup> cette opération est uniquement applicable aux dossiers publics dans exchange Server 2007 et exchange Server 2010. 
  
<sup>3</sup> cette opération est uniquement applicable aux dossiers publics dans Exchange 2010. 
  
<sup>4</sup> la recherche avec indexation de texte intégral dans un seul dossier public par le biais de l’option de recherche QueryString est prise en charge dans les versions d’Exchange commençant par Exchange 2013. 
  
<sup>5</sup> l’opération ConvertId ne convertit pas correctement les identificateurs de dossier public de l’identificateur EWS vers l’identificateur de magasin. Vous pouvez mettre à jour manuellement l’identificateur renvoyé sous forme de [solution de contournement](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId).
  
Les opérations suivantes ne sont pas prises en charge ou sont partiellement prises en charge, pour les dossiers publics dans les versions d’Exchange commençant par Exchange 2013 :
  
- **CopyFolder** (non pris en charge). Vous pouvez utiliser **CreateFolder** avec l’opération **CopyItems** pour implémenter la fonctionnalité de l’opération **CopyFolder** . 
    
- **EmptyFolder** (non pris en charge). Vous pouvez utiliser **FindItem** avec l’opération **DeleteItem** pour implémenter la fonctionnalité de fonctionnement de **EmptyFolder** . 
    
- **MoveFolder** (partiellement pris en charge). Vous ne pouvez pas déplacer des dossiers entre des dossiers privés et publics. Vous pouvez déplacer des dossiers entre des dossiers privés et publics dans Exchange 2007 et Exchange 2010. Vous pouvez déplacer des dossiers dans un dossier public dans toutes les versions d’Exchange. 
    
EWS et l’API managée EWS ne prennent pas en charge les fonctionnalités suivantes pour les dossiers publics :
  
- À l’aide de **opérationsyncfolderhierarchy**. Utilisez les opérations **FindFolder**, **GetFolder** et **SyncFolderItems** pour synchroniser les éléments et les dossiers d’une boîte aux lettres de dossiers publics. 
    
- Recherches en profondeur dans une hiérarchie de dossiers publics. Utiliser les appels de l’opération **FindFolder** récursive pour parcourir la hiérarchie de dossiers publics. 
    
- Utilisation de l’opération **CreateFolderPath** pour créer une hiérarchie de dossiers pour les dossiers publics. Vous devrez utiliser l’opération **CreateFolder** pour chaque niveau de dossier dans une hiérarchie de dossiers distincte lorsque vous ciblez une boîte aux lettres de dossiers publics. 
    
- Utilisation de l’opération **CreateItem** pour enregistrer des copies des messages électroniques envoyés. À la place, utilisez l’opération **MoveItem** pour déplacer une copie du message dans un dossier public. 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>Scénarios d’utilisation d’EWS et de l’API managée EWS pour utiliser des dossiers publics
<a name="bk_scenarios"> </a>

Les dossiers publics permettent de nombreux scénarios importants pour les utilisateurs de boîtes aux lettres Exchange. Vous pouvez aider les utilisateurs à l’aide d’EWS et de l’API managée EWS pour implémenter des solutions personnalisées permettant d’accéder à des dossiers publics et de les utiliser, ainsi que leur contenu. 
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>Accès par programme aux messages électroniques qui ont été envoyés à des listes de distribution

Les utilisateurs de boîtes aux lettres Exchange peuvent utiliser des dossiers publics pour stocker des messages électroniques qui sont envoyés à des listes de distribution. Il s’agit d’un moyen pratique d’enregistrer l’historique des listes de distribution. Vous pouvez utiliser l' [opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) dans EWS ou les méthodes **ExchangeService. FindItems ()** et **Folder. FINDITEMS ()** dans l’API managée EWS pour accéder aux messages électroniques de liste de distribution stockée. 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>Partager des messages électroniques importants et d’autres éléments de boîte aux lettres

Les utilisateurs de boîtes aux lettres peuvent utiliser des dossiers publics en tant que référentiel partagé pour les éléments de boîte aux lettres. Différents utilisateurs d’une organisation peuvent partager des messages électroniques importants ou des contacts à l’aide de dossiers publics. EWS peut fournir l’accès à ces éléments de boîte aux lettres partagés. Vous pouvez utiliser l' [opération MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) dans EWS ou la méthode **Item. Move ()** dans l’API managée EWS pour déplacer des messages électroniques, des contacts et d’autres éléments de boîte aux lettres à l’intérieur ou à l’extérieur d’un dossier public. 
  
### <a name="public-discussions-with-post-items"></a>Discussions publiques avec des éléments de publication

Les dossiers publics constituent un conteneur pratique pour les éléments post. Les éléments post fournissent un moyen d’utiliser des conversations thématiques sans avoir à envoyer de messages électroniques entre les utilisateurs. Les utilisateurs peuvent utiliser des dossiers publics et publier des éléments pour héberger et gérer des conversations thématiques entre différents utilisateurs de boîtes aux lettres au sein d’une organisation. De cette façon, les utilisateurs de boîtes aux lettres peuvent accéder à l’historique partagé d’une conversation qui utilise des éléments post même s’ils ne faisaient pas partie de la conversation. Vous pouvez utiliser l' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) dans EWS ou la méthode **Item. Save ()** dans l’API managée EWS pour créer et répondre aux éléments de publication stockés dans un dossier public. 
  
## <a name="routing-public-folder-requests"></a>Routage des demandes de dossier public
<a name="bk_routing"> </a>

Le contenu des dossiers publics peut être stocké sur plusieurs serveurs de boîtes aux lettres. La hiérarchie de dossiers publics peut être stockée dans une boîte aux lettres, tandis que le contenu du dossier public est stocké sur une autre. Chacun de ces serveurs peut être différent du serveur de boîtes aux lettres de l’utilisateur qui demande les informations. Dans ce cas, il est important d’inclure les en-têtes X-AnchorMailbox et X-PublicFolderMailbox supplémentaires dans vos demandes de dossiers publics pour recevoir des informations précises sur les dossiers publics.
  
La valeur pour X-AnchorMailbox et X-PublicFolderMailbox peut varier selon que vous effectuez une demande liée à la hiérarchie de dossiers ou au contenu du dossier. Le tableau suivant identifie la procédure à suivre pour chaque méthode d’API managée EWS ou opération EWS.
  
**Méthodes de l’API managée EWS et opérations EWS pour le routage des demandes de dossier public**

|**Lors de l’appel de ces méthodes**|**Lors de l’appel de ces opérations**|**Utilisez cette procédure**|
|:-----|:-----|:-----|
|[Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder. Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |Routage des demandes de hiérarchie de dossiers publics  <br/> |
|[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item. Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item. Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Routage des demandes de contenu de dossier public  <br/> |
   
## <a name="version-differences"></a>Différences entre les versions
<a name="VersionDifferences"> </a>

Dans Exchange 2007 et Exchange 2010, l’opération **ConvertId** fonctionne comme prévu lors de la conversion d’identificateurs de dossiers publics à partir de l’identificateur EWS vers l’identificateur de magasin. 
  
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Limites des dossiers publics](https://technet.microsoft.com/library/dn594582%28v=exchg.150%29.aspx)
    
- [FAQ : dossiers publics](https://technet.microsoft.com/library/jj552408.aspx)
    
- [Procédures de dossiers publics](https://technet.microsoft.com/library/jj657481.aspx)
    

