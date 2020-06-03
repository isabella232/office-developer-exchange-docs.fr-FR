---
title: Nouveautés d’EWS et d’autres services Web dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: aff6328f-cff1-42a6-9a4d-ea4d2d0461cf
description: Découvrez les nouveautés de EWS et des services Web dans Exchange, ainsi que l’API managée EWS.
localization_priority: Priority
ms.openlocfilehash: 5e74ad9d4cf5083983c28e477fd50d48e2d7fbb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529839"
---
# <a name="whats-new-in-ews-and-other-web-services-in-exchange"></a>Nouveautés d’EWS et d’autres services Web dans Exchange

Découvrez les nouveautés de EWS et des services Web dans Exchange, ainsi que l’API managée EWS.
  
Les services Web dans Exchange ont été mis à jour pour inclure de nouvelles fonctionnalités. 
  
**Tableau 1. Nouvelles fonctionnalités de service Web dans Exchange Online, Exchange 2013 et l’API managée EWS**

|Fonctionnalité|Implémenté dans Exchange Online|Implémenté dans Exchange 2013|Implémenté dans l’API managée EWS|
|:-----|:-----:|:-----:|:-----:|
|[eDiscovery](#eDisc) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[Archivage](#arch) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[Personnages](#personas) <br/> |Oui  <br/> |Oui  <br/> |Non  <br/> |
|[Magasin de contacts unifié](#unified) <br/> |Oui  <br/> |Oui  <br/> |Non  <br/> |
|[Stratégies de rétention](#retentionpolicy) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[Photos de l'utilisateur](#userphoto) <br/> |Oui  <br/> |Oui  <br/> |Non  <br/> |
|[Applications de messagerie pour la gestion d’Outlook](#ewsmailapps) <br/> |Oui  <br/> |Oui  <br/> |Oui  <br/> |
|[Proposer une nouvelle heure de réunion](#propose) <br/> |Oui  <br/> |Non  <br/> |Non  <br/> |

<a name="eDisc"> </a>

## <a name="ediscovery-in-ews"></a>Découverte électronique dans EWS

eDiscovery est un service Web de requête fédéré qui permet aux applications externes, telles que SharePoint 2013, d’effectuer des requêtes de données Exchange. La découverte se compose de plusieurs phases, y compris l’identification et la conservation des données clés, le Culling et l’examen des données, ainsi que la production de données en justice. les requêtes eDiscovery facilitent le processus de découverte en fournissant un flux de travail de découverte unique entre Exchange et SharePoint.
  
**Tableau 2. Opérations EWS et méthodes de l’API managée EWS pour utiliser la découverte électronique**

|**Nom de l’opération**|**Méthode d'API managée EWS**|**Description**|
|:-----|:-----|:-----|
|[Opération GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |[ExchangeService. GetDiscoverySearchConfiguration ()](https://msdn.microsoft.com/library/jj670206%28v=exchg.80%29.aspx) <br/> |Obtient les informations de configuration pour les conservations inaltérables, les recherches de découverte enregistrées et les boîtes aux lettres qui sont activées pour la recherche de découverte.  <br/> |
|[Opération GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |[ExchangeService. GetHoldOnMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Obtient l’état d’une conservation basée sur une requête, qui est définie à l’aide de l’opération **SetHoldOnMailboxes** .  <br/> |
|[Opération GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |[ExchangeService. GetNonIndexableItemDetails ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemdetails%28v=exchg.80%29.aspx) <br/> |Obtient des détails sur les éléments qui ne peuvent pas être indexés. Cela inclut, sans s’y limiter, l’identificateur de l’élément, un code d’erreur, une description de l’erreur, lorsqu’une tentative d’indexation de l’élément est effectuée, ainsi que des informations supplémentaires sur l’élément.  <br/> |
|[Opération GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |[ExchangeService. GetNonIndexableItemStatistics ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getnonindexableitemstatistics%28v=exchg.80%29.aspx) <br/> |Obtient le nombre d’éléments qui ne peuvent pas être indexés dans une boîte aux lettres.  <br/> |
|[Opération GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |[ExchangeService. GetSearchableMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getsearchablemailboxes%28v=exchg.80%29.aspx) <br/> |Obtient la liste des boîtes aux lettres pour lesquelles le client est autorisé à effectuer des recherches ou à exécuter la fonctionnalité eDiscovery.  <br/> |
|[Opération SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService. SearchMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> |Recherche des éléments dans des boîtes aux lettres spécifiques qui correspondent à des mots clés de requête.  <br/> |
|[Opération SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |[ExchangeService. SetHoldOnMailboxes ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) <br/> |Définit une conservation basée sur une requête sur des éléments.  <br/> |

<a name="arch"> </a>

## <a name="archiving-in-ews"></a>Archivage dans EWS

Les boîtes aux lettres d’archivage sont des boîtes aux lettres secondaires associées à un utilisateur. Les boîtes aux lettres d’archivage sont généralement utilisées pour gérer les limites de stockage des courriers électroniques. Par exemple, les éléments de courrier plus anciens peuvent régulièrement être déplacés de la boîte de réception vers la boîte aux lettres d’archivage. 
  
Exchange introduit deux nouvelles opérations EWS que vous pouvez utiliser pour archiver un ensemble d’éléments de courrier à partir d’une boîte aux lettres principale. L’archivage des éléments de boîte de réception de cette manière conserve la hiérarchie des dossiers des éléments. En outre, les boîtes aux lettres d’archivage peuvent désormais être stockées localement sur un client, ou à distance, d’une manière qui est principalement opaque pour un utilisateur, en utilisant un chemin d’accès de dossier pour pointer vers le contenu de l’archive.
  
**Tableau 3. Opérations EWS et méthodes de l’API managée EWS pour utiliser l’archivage**

|**Nom de l’opération**|**Méthode d'API managée EWS**|**Description**|
|:-----|:-----|:-----|
|[Opération ArchiveItem](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |[ExchangeService. ArchiveItems ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.archiveitems%28v=exchg.80%29.aspx) <br/> |Déplace un élément de la boîte aux lettres principale vers la boîte aux lettres d’archivage.  <br/> |
|[Opération CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Non implémenté.  <br/> |Crée une hiérarchie de dossiers dans une boîte aux lettres principale ou d’archivage.  <br/> |

<a name="personas"> </a>

## <a name="personas-in-ews"></a>Personnages dans EWS

Un *personnage* est une collection de données associée à un individu. Les données peuvent provenir d’une ou de plusieurs sources et sont associées au personnage au moyen d’un ID de lien commun. Les personnages dans EWS vous permettent de lier, Rechercher, parcourir et extraire des informations sur une personne à partir de plusieurs sources et de les organiser en une seule entité logique. Les personnages diffèrent des contacts dans le fait qu’un contact est une collection de données d’une source unique associée à un individu ; par exemple, un contact Outlook personnel ou une entrée dans une liste d’adresses globale (LAG). 
  
L’API managée EWS n’implémente pas cette fonctionnalité.
  
> [!NOTE]
> Le magasin de contacts unifié expose également la fonctionnalité Persona par le biais des opérations qui prennent en charge cette fonctionnalité. 
  
**Tableau 4. Opérations EWS pour utiliser des personnes**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[Opération FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Renvoie tous les objets Persona d’un dossier de contacts spécifié ou récupère tous les contacts qui correspondent à une chaîne de requête spécifiée.  <br/> |
|[Opération GetPersona](https://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Récupère un personnage.  <br/> |

<a name="unified"> </a>

## <a name="unified-contact-store-in-ews"></a>Magasin de contacts unifié dans EWS

Le magasin de contacts unifié est une fonctionnalité qui offre une expérience de contact cohérente entre les produits Office et agit comme un point d’intégration pour les applications tierces afin d’utiliser le même magasin de contacts. Elle permet aux utilisateurs et aux applications de stocker, de gérer et d’accéder aux informations de contact et de les mettre à disposition de manière globale entre Lync, Exchange 2013, Outlook, Outlook Web App et toute autre application qui implémente l’accès au magasin de contacts unifié. Exchange est le magasin de contacts pour l’expérience du magasin de contacts unifié. 
  
L’API managée EWS n’implémente pas cette fonctionnalité.
  
**Tableau 5. Opérations EWS pour utiliser le magasin de contacts unifié**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[Opération AddNewImContactToGroup](https://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Ajoute un nouveau contact de messagerie instantanée à un groupe. Le magasin de contacts unifié peut contenir un maximum de 1000 contacts.  <br/> |
|[Opération AddImContactToGroup](https://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Ajoute un contact de messagerie instantanée existant à un groupe. Le magasin de contacts unifié peut contenir un maximum de 1000 contacts.  <br/> |
|[Opération AddImGroup](https://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de messagerie instantanée. Le magasin de contacts unifié peut contenir un maximum de 64 groupes.  <br/> |
|[Opération AddNewTelUriContactToGroup](https://msdn.microsoft.com/library/c9688ce8-2465-45bb-8bd2-94b32ed4885c%28Office.15%29.aspx) <br/> |Ajoute un nouveau contact à un groupe en fonction du numéro de téléphone d’un contact.  <br/> |
|[Opération AddDistributionGroupToImList](https://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de listes de distribution. Le magasin de contacts unifié peut contenir un maximum de 64 groupes.  <br/> |
|[Opération GetImItemList](https://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Récupère une liste de groupes de messagerie instantanée et de personnes de contact de messagerie instantanée.  <br/> |
|[Opération GetImItems](https://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Récupère des informations sur les groupes de messagerie instantanée et les personnages de contact de messagerie instantanée spécifiés.  <br/> |
|[Opération RemoveContactFromImList](https://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Supprime le contact spécifié de tous les groupes de messagerie instantanée.  <br/> |
|[Opération RemoveImContactFromGroup](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Supprime un contact de messagerie instantanée d’un groupe.  <br/> |
|[Opération RemoveDistributionGroupFromImList](https://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Supprime le groupe de listes de distribution de messagerie instantanée spécifié.  <br/> |
|[Opération RemoveImGroup](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Supprime le groupe de messagerie instantanée spécifié.  <br/> |
|[Opération SetImGroup](https://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Modifie le nom d’affichage d’un groupe.  <br/> |

<a name="retentionpolicy"> </a>
  
## <a name="retention-policies-in-ews"></a>Stratégies de rétention dans EWS

Les stratégies de rétention sont des stratégies utilisées dans Exchange pour regrouper une ou plusieurs balises de rétention, pour appliquer des paramètres de rétention à des dossiers ou des éléments individuels tels que des messages électroniques et des messages vocaux, et pour appliquer des paramètres de rétention à une boîte aux lettres.
  
Exchange comprend trois types de balises de rétention :
  
- Balises de stratégie par défaut qui s’appliquent aux éléments de boîte aux lettres qui n’ont pas d’autre type de balise de rétention.
    
- Les balises de stratégie de dossiers système qui sont appliquées aux dossiers par défaut, tels que la boîte de réception.
    
- Les balises personnelles qu’un utilisateur peut appliquer aux dossiers qu’il crée ou à des éléments individuels.
    
Une seule stratégie de rétention peut être affectée à une boîte aux lettres, mais elle peut avoir une ou plusieurs balises de rétention de différents types liés à celle-ci. Les balises de rétention peuvent être liées ou dissociées d’une stratégie de rétention à tout moment. EWS dans Exchange expose une nouvelle opération, [GetUserRetentionPolicyTags](https://msdn.microsoft.com/library/57c6ff23-5c2c-42ee-824b-5a1b6dafab8c%28Office.15%29.aspx), et l’API managée EWS implémente une nouvelle méthode, [ExchangeService. GetUserRetentionPolicyTags ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuserretentionpolicytags%28v=exchg.80%29.aspx), qui fournit une liste de toutes les balises liées à une stratégie de rétention. Vous pouvez définir et récupérer les balises de stratégie de rétention pour les éléments et les dossiers à l’aide des opérations **CreateItem**, **CreateFolder**, **UpdateItem**, **UpdateFolder**, **GetItem**et **GetFolder** . 

<a name="userphoto"> </a>

## <a name="requesting-user-photos"></a>Demande de photos de l’utilisateur

Vous pouvez demander des photos de l’utilisateur à partir du serveur Exchange à l’aide de l’une des deux implémentations de l' [opération GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx): [Rest](how-to-get-user-photos-by-using-ews-in-exchange.md) ou SOAP. Le point de terminaison REST utilise une requête **Get** HTTPS standard pour obtenir la photo de l’utilisateur. Le service renverra une photo de l’utilisateur stockée dans Exchange ou une photo des services de domaine Active Directory (AD DS). 
  
L’API managée EWS n’implémente pas cette fonctionnalité. Toutefois, vous pouvez utiliser l’API managée EWS pour renvoyer des photos de l’utilisateur qui sont stockées dans une boîte aux lettres en obtenant la photo qui est attachée à un contact.

<a name="blocksender"> </a>

## <a name="block-senders-and-mark-email-as-junk-in-ews"></a>Bloquer les expéditeurs et marquer le courrier comme courrier indésirable dans EWS

Vous pouvez désormais bloquer les expéditeurs et marquer le courrier comme courrier indésirable à l’aide de la nouvelle [opération MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) dans EWS ou de la méthode [ExchangeService. MarkAsJunk ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) dans l’API managée EWS. 

<a name="ewsmailapps"> </a>

## <a name="mail-apps-for-outlook"></a>Applications de messagerie pour Outlook

EWS prend désormais en charge la gestion des applications de messagerie pour Outlook. 
  
**Tableau 6. Opérations EWS et méthodes de l’API managée EWS pour utiliser des applications de messagerie pour Outlook**

|**Nom de l’opération**|**Méthode d'API managée EWS**|**Description**|
|:-----|:-----|:-----|
|[Opération DisableApp](https://msdn.microsoft.com/library/211731a3-2470-49af-bda3-1ddfc15a8e46%28Office.15%29.aspx) <br/> |[ExchangeService. DisableApp ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disableapp%28v=exchg.80%29.aspx) <br/> |Désactive une application installée.  <br/> |
|[Opération GetAppManifests](https://msdn.microsoft.com/library/21a4987c-c24d-4a6e-ace4-e81edcda6303%28Office.15%29.aspx) <br/> |[ExchangeService. GetAppManifests ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getappmanifests%28v=exchg.80%29.aspx) <br/> |Obtient les manifestes d’application pour une boîte aux lettres.  <br/> |
|[Opération GetAppMarketplaceUrl](https://msdn.microsoft.com/library/2c016fc3-0e13-4624-9a5b-d3e84577a860%28Office.15%29.aspx) <br/> |[ExchangeService. GetAppMarketplaceUrl ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getappmarketplaceurl%28v=exchg.80%29.aspx) <br/> |Obtient l’URL de l’application Marketplace.  <br/> |
|[Opération GetClientAccessToken](https://msdn.microsoft.com/library/086876cc-e22c-4e89-89f9-19e78af51217%28Office.15%29.aspx) <br/> |[ExchangeService. GetClientAccessToken ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getclientaccesstoken%28v=exchg.80%29.aspx) <br/> |Obtient les jetons d’accès au client.  <br/> |
|[Opération InstallApp](https://msdn.microsoft.com/library/596eae95-3e78-489a-8bb2-d2dd4a026405%28Office.15%29.aspx) <br/> |[ExchangeService. InstallApp ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.installapp%28v=exchg.80%29.aspx) <br/> |Installe une application pour une boîte aux lettres.  <br/> |
|[Opération UninstallApp](https://msdn.microsoft.com/library/7707aa6a-381d-43f7-a454-54f6343ed127%28Office.15%29.aspx) <br/> |[ExchangeService. UninstallApp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.uninstallapp%28v=exchg.80%29.aspx) <br/> |Désinstalle une application d’une boîte aux lettres.  <br/> |

<a name="propose"> </a>

## <a name="propose-new-meeting-time"></a>Proposer une nouvelle heure de réunion

La fonctionnalité proposer une nouvelle heure a été introduite dans la version 15.00.0800.007 d’Exchange. Cela permet aux participants à la réunion de [proposer de nouveaux horaires de réunion](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) à l’organisateur de la réunion. 
  
L’API managée EWS n’implémente pas cette fonctionnalité.
  
## <a name="see-also"></a>Voir aussi

- [Explorer l'API managée EWS, EWS et les services web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Applications de messagerie pour Outlook et EWS dans Exchange](mail-apps-for-outlook-and-ews-in-exchange.md)
- [L'archivage dans EWS dans Exchange](archiving-in-ews-in-exchange.md)
- [découverte électronique dans EWS dans Exchange](ediscovery-in-ews-in-exchange.md)
- [Personnes et contacts dans EWS dans Exchange](people-and-contacts-in-ews-in-exchange.md)
    

