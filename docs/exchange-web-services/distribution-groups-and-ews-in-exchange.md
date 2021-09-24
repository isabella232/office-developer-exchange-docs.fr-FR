---
title: Les groupes de distribution et EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: fe08c2e3-92a0-43ec-bc61-69b14caee8fe
description: Découvrez les différents types de groupes de distribution disponibles dans Exchange et comment les gérer dans votre API gérée EWS ou votre application EWS.
ms.openlocfilehash: 71dc1a1e4c71310943eb19f8a5d6b3f470ab7ccb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512302"
---
# <a name="distribution-groups-and-ews-in-exchange"></a>Les groupes de distribution et EWS dans Exchange

Découvrez les différents types de groupes de distribution disponibles dans Exchange et comment les gérer dans votre API gérée EWS ou votre application EWS.
  
Un groupe de distribution est une collection d’adresses de messagerie associées à une seule adresse de messagerie ou un seul alias. Les groupes de distribution (parfois appelés listes de distribution) permettent à un utilisateur d’envoyer des messages électroniques à plusieurs personnes à l’aide d’une seule adresse de destinataire. Étant donné que l’appartenance à un groupe de distribution et, par conséquent, les destinataires du message, peuvent être gérés en dehors des threads de messagerie individuels, les groupes de distribution offrent un excellent moyen d’activer la distribution du courrier à un groupe d’utilisateurs. Vous pouvez créer et gérer des groupes de distribution par programme à l’aide de l’API gérée EWS, d’EWS et de Exchange Management Shell. Avant de commencer la programmation, explorons les différents types de groupes de distribution disponibles et vos options de gestion.
  
## <a name="types-of-distribution-groups"></a>Types de groupes de distribution

Exchange prend en charge trois types de groupes de distribution :
  
- [Groupes de distribution universels](distribution-groups-and-ews-in-exchange.md#bk_DistributionGroup) : objets de groupe de distribution universel Active Directory à messagerie activée. Les groupes de distribution universels sont utilisés pour distribuer des messages à un groupe de destinataires. 
    
- [Groupes de](distribution-groups-and-ews-in-exchange.md#bk_SecurityGroup) sécurité : objets Active Directory à messagerie également appelés groupes de sécurité universels. Les groupes de sécurité sont utilisés pour attribuer des autorisations d’accès aux ressources des services de domaine Active Directory (AD DS) et pour distribuer des messages. 
    
- [Groupes de contacts](distribution-groups-and-ews-in-exchange.md#bk_ContactGroup) : groupes de distribution privés situés dans la boîte aux lettres d’un utilisateur. 
    
Le type de groupe de distribution que vous choisissez dépend de l’endroit où vous prévoyez de stocker le groupe de distribution, de la personne qui l’utilisera et de son utilisation.

<a name="bk_DistributionGroup"> </a>

### <a name="universal-distribution-groups"></a>Groupes de distribution universels

Vous pouvez utiliser des groupes de distribution universels pour consolider des groupes de destinataires dans un seul alias ou adresse de messagerie. Étant donné que les groupes de distribution universels sont stockés dans AD DS, tout le monde peut les utiliser pour envoyer des messages électroniques, y compris des utilisateurs extérieurs à votre organisation. Vous pouvez utiliser l’API gérée EWS ou EWS pour développer un groupe de distribution, mais pour créer et gérer des groupes de distribution, vous devez utiliser les [cmdlets Exchange Management Shell.](#bk_UsingEMS)
  
Vous pouvez également utiliser des groupes de distribution universels pour contenir une collection de salles . par exemple, pour faciliter la recherche d’une salle de conférence pour une réunion. Les utilisateurs peuvent ajouter une liste de salles (un groupe de distribution universel qui contient des boîtes aux lettres de ressources de salle) à une demande de réunion pour trouver une salle disponible sans avoir à ajouter chaque salle individuellement.
  
Vous pouvez créer un groupe de distribution universel statique qui reste le même jusqu’à ce que vous mettez à jour l’appartenance, ou vous pouvez créer un groupe de distribution universel dynamique. Un groupe de distribution universel dynamique interroge les objets à messagerie Active Directory et crée l’appartenance au groupe en fonction des résultats. L’appartenance au groupe est recalculée chaque fois qu’un message électronique est envoyé au groupe. 

<a name="bk_SecurityGroup"> </a>

### <a name="security-groups"></a>Groupes de sécurité

Les groupes de distribution universels et les groupes de sécurité sont identiques dans la plupart des cas. Toutefois, contrairement aux groupes de distribution universels, vous pouvez utiliser des groupes de sécurité pour attribuer des autorisations aux ressources réseau dans AD DS. Vous ne pouvez pas utiliser l’API gérée EWS ou EWS pour créer et gérer des groupes de sécurité . à la place, vous utilisez [les cmdlets Exchange Management Shell.](#bk_UsingEMS) Toutefois, tout comme les groupes de distribution universels, vous pouvez utiliser l’API gérée EWS ou EWS pour développer des groupes de sécurité.

<a name="bk_ContactGroup"> </a>

### <a name="contact-groups"></a>Groupes de contacts

Si vous ne souhaitez pas accorder à chaque utilisateur un accès administratif au serveur pour créer des groupes de distribution, mais que vous souhaitez lui permettre d’envoyer un seul message à un grand nombre de personnes, vous pouvez le faire à l’aide de groupes de contacts. Une adresse de messagerie n’est pas associée à un groupe de contacts et elle n’existe que dans la boîte aux lettres d’un utilisateur . les autres utilisateurs n’y auront pas accès. Vous pouvez [utiliser l’API gérée EWS ou EWS pour créer des groupes de contacts.](how-to-create-contact-groups-by-using-ews-in-exchange.md)
  
## <a name="managing-distribution-groups-by-using-the-ews-managed-api-or-ews"></a>Gestion des groupes de distribution à l’aide de l’API gérée EWS ou d’EWS

Vous pouvez utiliser l’API gérée EWS ou EWS pour développer un groupe de distribution universel ou un groupe de sécurité et contrôler la création et la gestion d’un groupe de contacts . toutefois, vous ne pouvez pas utiliser ces technologies pour créer ou modifier les membres de ces groupes. 
  
**Tableau 1. Méthodes d’API gérées EWS et opérations EWS pour la gestion des groupes de distribution**

|**Méthode d'API managée EWS**|**Opération EWS**|**À utiliser pour...**|
|:-----|:-----|:-----|
|[Méthodes de classe ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)  <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Créez un groupe de contacts dans le magasin Exchange’informations.<br/><br/>**REMARQUE**: vous ne pouvez pas créer un groupe de distribution universel ou un groupe de sécurité à l’aide de l’API gérée EWS ou d’EWS.           |
|[ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |Développez un groupe de distribution universel, un groupe de sécurité ou un groupe de contacts en récupérant une liste de ses membres.  <br/> |
|[FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Recherchez des groupes de contacts dans la boîte aux lettres.  <br/> |
|[GetRooms](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) <br/> |[GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) <br/> |Récupérez une collection de toutes les salles d’une liste de salles spécifiée dans une organisation. Une liste de salles est un groupe de distribution qui contient uniquement des boîtes aux lettres de ressources de salle.  <br/> |
|[ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |Recherchez et renvoyer des candidats possibles pour correspondre à un nom ambigu. Les candidats peuvent être des groupes de distribution.  <br/> |
   
Vous pouvez utiliser les informations renvoyées par la méthode [ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou l’opération [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) pour déterminer les types de membres du groupe. Les types de membres sont définis par l’éumération [MailboxType](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.mailboxtype%28v=exchg.80%29.aspx) EWS Managed API et l’élément [MailboxType](https://msdn.microsoft.com/library/696e5fdb-d8c5-40f0-9e79-885eae65dfa4%28Office.15%29.aspx) EWS. 
  
**Tableau 2. Types de membres de groupe de distribution**

|**Valeur d’éumération MailboxType**|**Valeur de l’élément MailboxType**|**Description**|
|:-----|:-----|:-----|
|Boîte aux lettres  <br/> |Boîte aux lettres  <br/> |Objet Active Directory à messagerie.  <br/> |
|PublicGroup  <br/> |PublicDL  <br/> |Groupe de distribution contenu dans le groupe que vous avez développé. Pour obtenir la liste complète des membres, développez également ce groupe.  <br/> |
|ContactGroup  <br/> |PrivateDL  <br/> |Groupe de contacts situé dans la boîte aux lettres et disponible uniquement pour les utilisateurs de cette boîte aux lettres.  <br/> |
|Contact  <br/> |Contact  <br/> |Contact Exchange base de données ou contact de messagerie Active Directory.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="managing-distribution-groups-by-using-the-exchange-management-shell"></a>Gestion des groupes de distribution à l’aide de Exchange Management Shell

Vous pouvez [utiliser les cmdlets Exchange Management Shell](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx) pour créer et gérer des groupes de distribution universels et des groupes de sécurité dans votre code. 
  
> [!NOTE]
> Vous ne pouvez pas utiliser Exchange cmdlets Management Shell pour gérer les groupes de contacts. 
  
**Tableau 3. Exchange Cmdlets Management Shell pour travailler avec des groupes de distribution**

|**Cmdlet**|**À utiliser pour...**|
|:-----|:-----|
|[Disable-DistributionGroup](https://technet.microsoft.com/library/aa997942%28v=exchg.150%29.aspx) <br/> |Supprimez les fonctionnalités de messagerie d’un groupe de distribution à messagerie.  <br/> |
|[Enable-DistributionGroup](https://technet.microsoft.com/library/aa998916%28v=exchg.150%29.aspx) <br/> |Activer la messagerie d’un groupe universel existant.  <br/> |
|[Get-DistributionGroup](https://technet.microsoft.com/library/bb124755%28v=exchg.150%29.aspx) <br/> |Requête pour les groupes de distribution existants.  <br/> |
|[New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx) <br/> |Créez un groupe de distribution.  <br/> |
|[Remove-DistributionGroup](https://technet.microsoft.com/library/aa997627%28v=exchg.150%29.aspx) <br/> |Supprimez un groupe de distribution existant d’AD DS.  <br/> |
|[Set-DistributionGroup](https://technet.microsoft.com/library/bb124955%28v=exchg.150%29.aspx) <br/> |Modifier les paramètres d’un groupe de distribution existant.  <br/> |
|[Add-DistributionGroupMember](https://technet.microsoft.com/library/bb124340%28v=exchg.150%29.aspx) <br/> |Ajoutez un destinataire à un groupe de distribution.  <br/> |
|[Get-DistributionGroupMember](https://technet.microsoft.com/library/aa996367%28v=exchg.150%29.aspx) <br/> |Recherchez les membres existants du groupe de distribution.  <br/> |
|[Remove-DistributionGroupMember](https://technet.microsoft.com/library/aa998016%28v=exchg.150%29.aspx) <br/> |Supprimez un destinataire existant d’un groupe de distribution.  <br/> |
|[Update-DistributionGroupMember](https://technet.microsoft.com/library/dd335049%28v=exchg.150%29.aspx) <br/> |Mettre à jour un membre d’un groupe de distribution spécifié.  <br/> |
|[Get-DynamicDistributionGroup](https://technet.microsoft.com/library/bb124762%28v=exchg.150%29.aspx) <br/> |Récupérez les paramètres d’un groupe de distribution dynamique existant.  <br/> |
|[New-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125127%28v=exchg.150%29.aspx) <br/> |Créez un groupe de distribution dynamique.  <br/> |
|[Remove-DynamicDistributionGroup](https://technet.microsoft.com/library/bb125038%28v=exchg.150%29.aspx) <br/> |Supprimez un groupe de distribution dynamique existant. Cette cmdlet supprime le groupe de distribution dynamique des AD DS.  <br/> |
|[Set-DynamicDistributionGroup](https://technet.microsoft.com/library/bb123796%28v=exchg.150%29.aspx) <br/> |Modifier les paramètres d’un groupe de distribution dynamique existant.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="in-this-section"></a>Contenu de cette section

- [Créer des groupes de contacts à l’aide d’EWS dans Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)   
- [Développer des groupes de distribution à l’aide d’EWS Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)   
- [Appel des cmdlets Exchange Management Shell à partir du code géré](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx)
    

