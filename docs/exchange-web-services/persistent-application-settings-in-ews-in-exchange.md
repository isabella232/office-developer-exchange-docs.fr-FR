---
title: Paramètres de l'application persistant dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 394d4e70-8517-4073-809a-5b61780ff923
description: Découvrez les différentes options que votre API managée EWS ou votre application EWS peut utiliser pour créer des paramètres d’application personnalisés persistants dans Exchange.
ms.openlocfilehash: b1faa057e5a0c1a96498efcc23738c83d25ae986
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457402"
---
# <a name="persistent-application-settings-in-ews-in-exchange"></a>Paramètres de l'application persistant dans EWS dans Exchange

Découvrez les différentes options que votre API managée EWS ou votre application EWS peut utiliser pour créer des paramètres d’application personnalisés persistants dans Exchange.
  

  
Le moyen le plus simple de maintenir la synchronisation des configurations clientes personnalisées pour une boîte aux lettres, ou des dossiers et des éléments d’une boîte aux lettres, est de stocker les paramètres d’application sur un serveur Exchange. Vous pouvez vous assurer que ces paramètres sont conservés pour une boîte aux lettres à l’aide de l’une des méthodes suivantes : 
  
- Objets de configuration utilisateur
    
- Propriétés étendues
    
- Éléments personnalisés
    
## <a name="what-are-my-options-for-creating-persistent-application-settings"></a>Quelles sont les options permettant de créer des paramètres d’application permanente ?
<a name="Options"> </a>

Les objets de configuration utilisateur constituent votre meilleure option de stockage des paramètres de configuration de vos applications clientes EWS. Vous pouvez également utiliser des propriétés d’extension ou des éléments personnalisés, ou une combinaison des trois. Choisissez votre option en fonction de l’étendue de vos paramètres et indiquez si vos paramètres doivent être disponibles pour d’autres applications.
  
**Tableau 1. Options recommandées pour la création de paramètres d’application persistante en fonction de l’étendue**

|**Définition de l’étendue**|**Utiliser...**|**Accessible par**|
|:-----|:-----|:-----|
|Option  <br/> |Une propriété étendue sur un élément existant.  <br/> |N’importe quelle application EWS. Seuls les clients EWS qui connaissent l’identificateur de propriété peuvent accéder à une propriété étendue.  <br/> |
|Folder  <br/> |Un objet de configuration utilisateur sur le dossier cible. Il s’agit d’un moyen efficace pour enregistrer les paramètres d’affichage d’un dossier.  <br/> |N’importe quelle application EWS.  <br/> |
|Boîte aux lettres  <br/> |Un objet de configuration utilisateur dans le dossier msgrootfolder par défaut.  <br/> |N’importe quelle application EWS.  <br/> |
   
### <a name="user-configuration-objects"></a>Objets de configuration utilisateur
<a name="UserConfig"> </a>

Les objets de configuration utilisateur sont des éléments spéciaux qui sont associés à des dossiers dans une boîte aux lettres. Les objets de configuration utilisateur, également appelés éléments associés aux dossiers, sont généralement la meilleure option pour conserver les paramètres d’application, en particulier si les informations de configuration sont associées à un dossier ou à une boîte aux lettres. Elles ne sont généralement pas exposées aux utilisateurs finaux. Étant donné qu’ils peuvent stocker en mode natif des flux de données et des dictionnaires de données, ils sont idéaux pour stocker des informations de configuration. La meilleure façon d’utiliser des objets de configuration utilisateur est de stocker un ensemble de configurations dans un document XML, puis d’enregistrer ces informations dans l’une des propriétés du flux de configuration de l’utilisateur.
  
Les objets de configuration utilisateur sont accessibles différemment des autres types d’éléments stockés dans une boîte aux lettres. Vous pouvez utiliser la méthode de l’API managée de [dossier. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=EXCHG.80%29.aspx) ou l’opération EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher tous les éléments, mais vous devez utiliser l’option de parcours de recherche **associée** pour rechercher des objets de configuration utilisateur. Le parcours de recherche **associé** indique que les résultats de la recherche doivent contenir uniquement des objets de configuration utilisateur. EWS inclut un ensemble d’opérations spécifiques aux objets de configuration utilisateur. 
  
**Tableau 1. Opérations EWS et méthodes de l’API managée EWS pour l’utilisation d’objets de configuration utilisateur**

|**Afin de...**|**Utiliser cette opération EWS**|**Utiliser cette méthode d’API managée EWS**|
|:-----|:-----|:-----|
|Créer un objet de configuration utilisateur  <br/> |[Opération CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) <br/> |[UserConfiguration. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) <br/> |
|Obtenir un objet de configuration utilisateur  <br/> |[Opération GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |[UserConfiguration. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> [UserConfiguration. Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.load%28v=exchg.80%29.aspx) <br/> |
|Mettre à jour un objet de configuration utilisateur  <br/> |[Opération UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) <br/> |[UserConfiguration. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> |
|Supprimer un objet de configuration utilisateur  <br/> |[Opération DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |
   
> [!NOTE]
> Les objets de configuration utilisateur créés à l’aide d’EWS ont un préfixe [ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) qui commence par «IPM. Configuration. ". Le **ItemClass** d’un objet de configuration utilisateur est le préfixe de l’objet Configuration utilisateur et le nom de votre objet de configuration utilisateur. Vous pouvez utiliser la propriété de l’API managée EWS [Item. ItemClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) ou l’élément EWS **ItemClass** pour rechercher les objets de configuration utilisateur que vous avez définis. 
  
### <a name="extended-properties"></a>Propriétés étendues
<a name="ExtendedProperties"> </a>

Utilisez les [propriétés étendues](properties-and-extended-properties-in-ews-in-exchange.md) si vous souhaitez stocker des informations de configuration sur des éléments. EWS, contrairement à MAPI, ne retourne pas de conteneur de propriétés pour les éléments. Cela signifie qu’un client EWS doit connaître l’identificateur de propriété étendue afin de trouver et d’accéder à la propriété étendue. Si vous avez besoin de stocker des informations de configuration sur des éléments autres que des objets de configuration utilisateur, l’utilisation de propriétés étendues pour créer des propriétés personnalisées peut être la solution pour vous. Les propriétés étendues vous permettent d’accéder à des informations et de les stocker sur les propriétés qui ne font pas partie du jeu de propriétés standard d’un élément. 
  
> [!IMPORTANT]
> Le schéma de base de données Exchange comporte un nombre fini de propriétés. Le nombre maximal d’identificateurs de propriétés pour une base de données Exchange est de 32 767. Si vous utilisez des propriétés étendues pour stocker de nombreux paramètres, nous vous conseillons d’utiliser une seule propriété étendue pour stocker ces paramètres afin de ne pas dépasser ce maximum. 
  
Vous pouvez utiliser l' [élément. mettre à jour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=EXCHG.80%29.aspx) la méthode de l’API managée EWS ou l’opération EWS [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) pour définir les propriétés étendues des objets de configuration de l’utilisateur. 
  
### <a name="custom-items"></a>Éléments personnalisés
<a name="CustomItems"> </a>

Des éléments personnalisés peuvent également être utilisés pour stocker des informations. Les propriétés d’élément existantes peuvent être réaffectées pour contenir des informations de configuration. Vous pouvez utiliser les propriétés étendues pour définir vos propres propriétés pour votre application. L’utilisation d’éléments personnalisés pour stocker la configuration offre les avantages suivants : 
  
- Elles fonctionnent pour toutes les versions d’Exchange qui prennent en charge EWS.
    
- Si vous n’utilisez pas de propriétés étendues sur l’élément, le budget des propriétés Exchange n’est pas facturé.
    
## <a name="where-should-i-store-my-application-settings"></a>Où dois-je stocker mes paramètres d’application ?
<a name="ApplicationSettingsLocation"> </a>

Les dossiers de boîte aux lettres et les éléments qu’ils contiennent se trouvent dans le dossier de messages racine. Ce dossier est identifié par la valeur [WellKnownFolderName. msgfolderroot](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) dans l’API managée EWS. En termes MAPI, il s’agit de l’équivalent de la sous-arborescence IPM d’une boîte aux lettres. Les objets de configuration utilisateur sont souvent utilisés pour créer des paramètres d’interface utilisateur, afin qu’une application puisse afficher les paramètres d’affichage en fonction du dossier auquel un utilisateur accède. Les paramètres d’affichage basés sur un dossier sont généralement définis sur un objet de configuration utilisateur associé au dossier. Toutefois, vous pouvez parfois faire en sorte que vos paramètres soient globaux pour votre application. Dans ce cas, vous pouvez stocker vos paramètres dans le dossier de messages racine. 
  
La plupart des utilisateurs ne prennent pas en charge et n’accèdent généralement pas au dossier racine de la boîte aux lettres. Ce dossier est identifié par la valeur [WellKnownFolderName. root](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) dans l’API managée EWS. En termes MAPI, il s’agit de l’équivalent de la sous-arborescence non IPM d’une boîte aux lettres. Les informations auxquelles les utilisateurs finaux n’accèdent pas directement sont stockées dans le dossier racine de la boîte aux lettres. Il se peut que vous vouliez stocker le paramètre de votre application dans ce dossier car les applications clientes n’y accèdent généralement pas. 
  
## <a name="version-differences"></a>Différences entre les versions
<a name="VersionDifferences"> </a>

Les objets de configuration utilisateur sont disponibles dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange à partir d’Exchange 2010.
  
## <a name="see-also"></a>Voir aussi


- [Gérer les paramètres d’application permanente à l’aide d’EWS dans Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    
- [Les propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Utiliser des dossiers à l’aide d’EWS dans Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Utilisations d’éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

