---
title: Nouveautés dans EWS et d’autres services web Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: aff6328f-cff1-42a6-9a4d-ea4d2d0461cf
description: Découvrez les nouveautés dans EWS et des services web Exchange et l’API managée EWS.
ms.openlocfilehash: 9e848babc96707152be767f42b561a587fc6cff0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755081"
---
# <a name="whats-new-in-ews-and-other-web-services-in-exchange"></a>Nouveautés dans EWS et d’autres services web Exchange

Découvrez les nouveautés dans EWS et des services web Exchange et l’API managée EWS.
  
Services Web dans Exchange ont été mis à jour pour inclure les nouvelles fonctionnalités. 
  
**Le tableau 1. Service web de nouvelles fonctionnalités dans Exchange Online, Exchange 2013 et l’API managée EWS**

|Fonctionnalité|Implémentée dans Exchange Online|Implémenté dans Exchange 2013|Implémenté dans l’API managée EWS|
|:-----|:-----:|:-----:|:-----:|
|[découverte électronique](#eDisc) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[L’archivage](#arch) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[Personnages](#personas) <br/> |Oui  <br/> |Oui  <br/> |Non  <br/> |
|[Magasin de contacts unifié](#unified) <br/> |Oui  <br/> |Oui  <br/> |Non  <br/> |
|[Stratégies de rétention](#retentionpolicy) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[Photos de l’utilisateur](#userphoto) <br/> |Oui  <br/> |Oui  <br/> |Non  <br/> |
|[Applications de messagerie pour la gestion d’Outlook](#ewsmailapps) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[Proposer la nouvelle heure de réunion](#propose) <br/> |Oui  <br/> |Non  <br/> |Non  <br/> |

<a name="eDisc"> </a>

## <a name="ediscovery-in-ews"></a>découverte électronique dans EWS

découverte électronique est un service web requête fédérée qui permet aux applications externes, tels que SharePoint 2013, d’effectuer des requêtes de données Exchange. Découverte comprend plusieurs étapes, y compris identification préserver les données critiques, élimination vers le bas et examen des données et créer des données dans un tribunal. requêtes eDiscovery facilitent le processus de découverte en fournissant un flux de travail unique découverte entre Exchange et SharePoint.
  
**Le tableau 2. Opérations EWS et méthodes d’API managées pour travailler avec eDiscovery**

|**Nom de l’opération**|**Méthode d'API managée EWS**|**Description**|
|:-----|:-----|:-----|
|[Opération GetDiscoverySearchConfiguration](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |[ExchangeService.GetDiscoverySearchConfiguration()](http://msdn.microsoft.com/en-us/library/jj670206%28v=exchg.80%29.aspx) <br/> |Obtient les informations de configuration pour les archives permanentes, enregistrement des recherches de découverte et les boîtes aux lettres qui sont activées pour la recherche de découverte.  <br/> |
|[Opération GetHoldOnMailboxes](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |[ExchangeService.GetHoldOnMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Obtient l’état d’une suspension basée sur une requête, qui est définie à l’aide de l’opération **SetHoldOnMailboxes** .  <br/> |
|[Opération GetNonIndexableItemDetails](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |[ExchangeService.GetNonIndexableItemDetails()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemdetails%28v=exchg.80%29.aspx) <br/> |Obtient des informations sur les éléments qui ne peuvent pas être indexés. Cela inclut, mais n’est pas limité à l’identificateur d’élément, un code d’erreur, une description de l’erreur lors de la tentative d’index de l’élément et des informations supplémentaires sur l’élément.  <br/> |
|[Opération GetNonIndexableItemStatistics](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |[ExchangeService.GetNonIndexableItemStatistics()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemstatistics%28v=exchg.80%29.aspx) <br/> |Obtient le nombre d’éléments qui ne peuvent pas être indexés dans une boîte aux lettres.  <br/> |
|[Opération GetSearchableMailboxes](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |[ExchangeService.GetSearchableMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getsearchablemailboxes%28v=exchg.80%29.aspx) <br/> |Obtient une liste des boîtes aux lettres que le client a l’autorisation de rechercher ou d’effectuer une découverte électronique sur.  <br/> |
|[Opération SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService.SearchMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> |Recherche des éléments dans des boîtes aux lettres spécifiques qui correspondent à des mots clés de requête.  <br/> |
|[Opération SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |[ExchangeService.SetHoldOnMailboxes()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Ensembles de basée sur une requête en attente sur les éléments.  <br/> |

<a name="arch"> </a>

## <a name="archiving-in-ews"></a>L’archivage dans EWS

Boîtes aux lettres d’archivage sont des boîtes aux lettres secondaires qui sont associés à un utilisateur. Boîtes aux lettres d’archivage sont généralement utilisés pour gérer les limites de stockage de courrier électronique. Par exemple, les éléments de messagerie électronique antérieurs régulièrement peuvent être déplacés que de la boîte de réception à la boîte aux lettres d’archive. 
  
Exchange présente deux nouvelles opérations EWS que vous pouvez utiliser pour archiver un ensemble d’éléments de messagerie à partir d’une boîte aux lettres principale. L’archivage des éléments de boîte de réception de cette manière conserve la hiérarchie de dossiers des éléments. En outre, les boîtes aux lettres d’archive maintenant peuvent être stockées localement sur un client, soit à distance, d’une manière qui est principalement opaque à un utilisateur, à l’aide d’un chemin d’accès du dossier pour pointer vers le contenu de l’archive.
  
**Le tableau 3. Opérations EWS et méthodes d’API managées pour l’utilisation de l’archivage**

|**Nom de l’opération**|**Méthode d'API managée EWS**|**Description**|
|:-----|:-----|:-----|
|[Opération ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |[ExchangeService.ArchiveItems()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.archiveitems%28v=exchg.80%29.aspx) <br/> |Déplace un élément à partir de la boîte aux lettres principale pour la boîte aux lettres d’archive.  <br/> |
|[Opération CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Non implémenté.  <br/> |Crée une hiérarchie de dossiers dans un serveur principal ou d’une boîte aux lettres d’archive.  <br/> |

<a name="personas"> </a>

## <a name="personas-in-ews"></a>Personnages EWS

Un *personnage* est une collection de données qui sont associées à une personne. Les données peuvent provenir d’une ou plusieurs sources et sont associées avec le personnage au moyen d’un ID de lien courantes. Personnages EWS permettent de lier, recherche, rechercher et récupérer des informations sur une personne à partir de plusieurs sources et organiser ces informations en une seule entité logique. Personnages diffèrent des contacts en ce sens qu’un contact est une collection de données à partir d’une source unique qui est associée à une personne ; par exemple, un contact personnel Outlook ou une entrée dans une liste d’adresses globale (LAG). 
  
L’API managée EWS n’implémente pas cette fonctionnalité.
  
> [!NOTE]
> Le magasin de contacts unifié expose également les fonctionnalités de personnage par les opérations qui prennent en charge cette fonctionnalité. 
  
**Le tableau 4. Opérations EWS pour l’utilisation de personnages**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[Opération FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Renvoie tous les objets personnage à partir d’un dossier de contacts spécifié ou récupère tous les contacts qui correspondent à une chaîne de requête spécifiée.  <br/> |
|[Opération GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Récupère un personnage.  <br/> |

<a name="unified"> </a>

## <a name="unified-contact-store-in-ews"></a>Magasin de contacts unifié dans EWS

Le magasin de contacts unifié est une fonctionnalité qui fournit une expérience cohérente contact entre les produits Office et agit comme un point d’intégration aux applications de tiers afin d’utiliser le même magasin de contacts. Il permet aux utilisateurs et applications stocker, gérer et accéder aux informations de contact et les rendre disponibles globalement dans Lync, Exchange 2013, Outlook, Outlook Web App et toute autre application qui implémente l’accès pour le magasin de contacts unifié. Exchange est le magasin de contacts pour l’expérience de magasin de contacts unifié. 
  
L’API managée EWS n’implémente pas cette fonctionnalité.
  
**Tableau 5. Opérations EWS pour travailler avec le magasin de contacts unifié**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[Opération AddNewImContactToGroup](http://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Ajoute un nouveau contact de messagerie instantanée à un groupe. Le magasin de contacts unifié peut contenir un maximum de 1000 contacts.  <br/> |
|[Opération AddImContactToGroup](http://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Ajoute un contact de messagerie instantanée existant à un groupe. Le magasin de contacts unifié peut contenir un maximum de 1000 contacts.  <br/> |
|[Opération AddImGroup](http://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de messagerie instantanée. Le magasin de contacts unifié peut contenir un maximum de 64 groupes.  <br/> |
|[Opération AddNewTelUriContactToGroup](http://msdn.microsoft.com/library/c9688ce8-2465-45bb-8bd2-94b32ed4885c%28Office.15%29.aspx) <br/> |Ajoute un nouveau contact à un groupe basé sur le numéro de téléphone d’un contact.  <br/> |
|[Opération AddDistributionGroupToImList](http://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de liste de distribution. Le magasin de contacts unifié peut contenir un maximum de 64 groupes.  <br/> |
|[Opération GetImItemList](http://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Récupère une liste des groupes de messagerie instantanée et des personnes de contact de messagerie instantanée.  <br/> |
|[Opération GetImItems](http://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Récupère des informations sur les groupes de messagerie instantanée spécifiés et les personnes de contact de messagerie instantanée.  <br/> |
|[Opération RemoveContactFromImList](http://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Supprime le contact spécifié à partir de tous les groupes de messagerie instantanée.  <br/> |
|[Opération RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Supprime un contact de messagerie instantanée d’un groupe.  <br/> |
|[Opération RemoveDistributionGroupFromImList](http://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Supprime le groupe de liste de distribution par messagerie instantanée spécifié.  <br/> |
|[Opération RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Supprime le groupe de messagerie instantanée spécifié.  <br/> |
|[Opération SetImGroup](http://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Modifie le nom complet d’un groupe.  <br/> |

<a name="retentionpolicy"> </a>
  
## <a name="retention-policies-in-ews"></a>Stratégies de rétention dans EWS

Stratégies de rétention sont les stratégies qui sont utilisées dans Exchange au groupe d’une ou plusieurs balises de rétention, pour appliquer les paramètres de rétention aux dossiers ou individuels ces éléments sous forme de messages de messagerie vocale et de messagerie et pour appliquer les paramètres de rétention à une boîte aux lettres.
  
Exchange inclut trois types de balises de rétention :
  
- Balises de stratégie par défaut qui s’appliquent aux éléments de boîte aux lettres ayant aucun autre type de balise de rétention appliquée.
    
- Balises de stratégie de dossier système qui sont appliqués aux dossiers par défaut tels que la boîte de réception.
    
- Balises personnelles qu’un utilisateur peut appliquer aux dossiers qu’ils créent ou à des éléments individuels.
    
Stratégie de rétention qu’un seul peut être affectée à une boîte aux lettres, mais la stratégie peut avoir une ou plusieurs balises de rétention des différents types de lié. Balises de rétention peuvent être liés à ou non à partir d’une stratégie de rétention à tout moment. Une nouvelle opération, [GetUserRetentionPolicyTags](http://msdn.microsoft.com/library/57c6ff23-5c2c-42ee-824b-5a1b6dafab8c%28Office.15%29.aspx), expose les services EWS d’Exchange et l’API managée EWS implémente une nouvelle méthode, [ExchangeService.GetUserRetentionPolicyTags()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getuserretentionpolicytags%28v=exchg.80%29.aspx), qui fournit une liste de toutes les balises qui sont liés à une stratégie de rétention. Vous pouvez définir et récupérer des balises de stratégie de rétention des éléments et des dossiers en utilisant la **CreateItem**, **CreateFolder**, **UpdateItem**, **UpdateFolder**, **GetItem**et opérations **GetFolder** . 

<a name="userphoto"> </a>

## <a name="requesting-user-photos"></a>Demande de photos de l’utilisateur

Vous pouvez demander des photos de l’utilisateur à partir du serveur Exchange à l’aide d’une de ces deux implémentations de l' [opération GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx): [REST](how-to-get-user-photos-by-using-ews-in-exchange.md) ou SOAP. Le point de terminaison REST utilise une requête HTTPS **GET** standard pour obtenir la photo de l’utilisateur. Le service retournera soit une photo de l’utilisateur stockées dans Exchange ou une photo des Services de domaine Active Directory (AD DS). 
  
L’API managée EWS n’implémente pas cette fonctionnalité. Vous pouvez, toutefois, utiliser l’API managée EWS pour renvoyer les photos de l’utilisateur qui sont stockés dans une boîte aux lettres en obtenant la photo est attachée à un contact.

<a name="blocksender"> </a>

## <a name="block-senders-and-mark-email-as-junk-in-ews"></a>Bloquer les expéditeurs et marquer le courrier électronique comme courrier indésirable dans EWS

Vous pouvez maintenant bloquer les expéditeurs et marquer le courrier électronique comme courrier indésirable à l’aide de la nouvelle [opération MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) EWS ou la méthode [ExchangeService.MarkAsJunk()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) dans l’API managée EWS. 

<a name="ewsmailapps"> </a>

## <a name="mail-apps-for-outlook"></a>Applications de messagerie pour Outlook

EWS prend désormais en charge pour la gestion des applications de messagerie pour Outlook. 
  
**Le tableau 6. Opérations EWS et méthodes d’API managées pour travailler avec les applications de messagerie pour Outlook**

|**Nom de l’opération**|**Méthode d'API managée EWS**|**Description**|
|:-----|:-----|:-----|
|[Opération DisableApp](http://msdn.microsoft.com/library/211731a3-2470-49af-bda3-1ddfc15a8e46%28Office.15%29.aspx) <br/> |[ExchangeService.DisableApp()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disableapp%28v=exchg.80%29.aspx) <br/> |Désactive une application installée.  <br/> |
|[Opération GetAppManifests](http://msdn.microsoft.com/library/21a4987c-c24d-4a6e-ace4-e81edcda6303%28Office.15%29.aspx) <br/> |[ExchangeService.GetAppManifests()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmanifests%28v=exchg.80%29.aspx) <br/> |Obtient les manifestes d’application pour une boîte aux lettres.  <br/> |
|[Opération GetAppMarketplaceUrl](http://msdn.microsoft.com/library/2c016fc3-0e13-4624-9a5b-d3e84577a860%28Office.15%29.aspx) <br/> |[ExchangeService.GetAppMarketplaceUrl()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getappmarketplaceurl%28v=exchg.80%29.aspx) <br/> |Obtient l’URL du site marketplace application.  <br/> |
|[Opération GetClientAccessToken](http://msdn.microsoft.com/library/086876cc-e22c-4e89-89f9-19e78af51217%28Office.15%29.aspx) <br/> |[ExchangeService.GetClientAccessToken()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getclientaccesstoken%28v=exchg.80%29.aspx) <br/> |Obtient des jetons d’accès client.  <br/> |
|[Opération InstallApp](http://msdn.microsoft.com/library/596eae95-3e78-489a-8bb2-d2dd4a026405%28Office.15%29.aspx) <br/> |[ExchangeService.InstallApp()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.installapp%28v=exchg.80%29.aspx) <br/> |Installe une application pour une boîte aux lettres.  <br/> |
|[Opération UninstallApp](http://msdn.microsoft.com/library/7707aa6a-381d-43f7-a454-54f6343ed127%28Office.15%29.aspx) <br/> |[ExchangeService.UninstallApp](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.uninstallapp%28v=exchg.80%29.aspx) <br/> |Désinstalle une application à partir d’une boîte aux lettres.  <br/> |

<a name="propose"> </a>

## <a name="propose-new-meeting-time"></a>Proposer la nouvelle heure de réunion

La fonctionnalité de temps de nouveau proposer a été introduite dans la version 15.00.0800.007 d’Exchange. Ainsi, les participants de [proposer de nouvelles dates de réunion](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) à l’organisateur de la réunion. 
  
L’API managée EWS n’implémente pas cette fonctionnalité.
  
## <a name="see-also"></a>Voir aussi

- [Explorer l'API managée EWS, EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Applications de messagerie pour Outlook et EWS dans Exchange](mail-apps-for-outlook-and-ews-in-exchange.md)
- [L'archivage dans EWS dans Exchange](archiving-in-ews-in-exchange.md)
- [découverte électronique dans EWS dans Exchange](ediscovery-in-ews-in-exchange.md)
- [Personnes et contacts dans EWS dans Exchange](people-and-contacts-in-ews-in-exchange.md)
    

