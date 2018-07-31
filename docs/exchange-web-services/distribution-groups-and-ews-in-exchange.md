---
title: Les groupes de distribution et EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fe08c2e3-92a0-43ec-bc61-69b14caee8fe
description: En savoir plus sur les différents types de groupes de distribution qui sont disponibles dans Exchange et comment vous pouvez les gérer dans votre API managées ou les applications EWS.
ms.openlocfilehash: 725b02c69f004a58c7216763d3c44f1e9d2df2ab
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353958"
---
# <a name="distribution-groups-and-ews-in-exchange"></a>Les groupes de distribution et EWS dans Exchange

En savoir plus sur les différents types de groupes de distribution qui sont disponibles dans Exchange et comment vous pouvez les gérer dans votre API managées ou les applications EWS.
  
Un groupe de distribution est une collection d’adresses de messagerie qui sont associés à une seul alias ou l’adresse électronique. Groupes de distribution (également appelés listes de distribution) autoriser un utilisateur à envoyer un message électronique à plusieurs personnes à l’aide d’une seule adresse destinataire. Étant donné que l’appartenance au groupe de distribution et par conséquent, les destinataires du message, peuvent être gérés en dehors des threads de messagerie individuelles, des groupes de distribution fournissent un excellent moyen pour activer la distribution du courrier à un groupe d’utilisateurs. Vous pouvez créer et gérer des groupes de distribution à l’aide de l’API managée EWS, EWS et Exchange Management Shell par programme. Avant de commencer la programmation, examinons les différents types de groupes de distribution qui sont disponibles et les options pour les gérer.
  
## <a name="types-of-distribution-groups"></a>Types de groupes de distribution

Exchange prend en charge trois types de groupes de distribution :
  
- [Groupes de distribution universels](distribution-groups-and-ews-in-exchange.md#bk_DistributionGroup) , objets de groupe de distribution universels Active Directory qui sont à extension messagerie. Groupes de distribution universels sont utilisés pour distribuer des messages à un groupe de destinataires. 
    
- [Groupes de sécurité](distribution-groups-and-ews-in-exchange.md#bk_SecurityGroup) — des objets Active Directory qui sont à extension messagerie ; également connu sous le nom des groupes de sécurité universels. Groupes de sécurité sont utilisés pour affecter des autorisations d’accès à des ressources dans les Services de domaine Active Directory (AD DS) ainsi que pour distribuer des messages. 
    
- [Groupes de contacts](distribution-groups-and-ews-in-exchange.md#bk_ContactGroup) , les groupes de distribution privée qui sont trouvent dans la boîte aux lettres d’un utilisateur. 
    
Le type de groupe de distribution que vous choisissez dépendra où vous souhaitez stocker le groupe de distribution qui vont l’utiliser, et qu’il sera utilisé pour.

<a name="bk_DistributionGroup"> </a>

### <a name="universal-distribution-groups"></a>Groupes de distribution universels

Vous pouvez utiliser des groupes de distribution universels à consolider des groupes de destinataires dans une seul alias ou l’adresse électronique. Étant donné que les groupes de distribution universels sont stockées dans AD DS, tout le monde peut les utiliser pour envoyer un message électronique, y compris les utilisateurs extérieurs à votre organisation. Vous pouvez utiliser les API managées EWS pour développer un groupe de distribution, mais pour créer et gérer des groupes de distribution, vous devrez utiliser des [applets de commande Exchange Management Shell](#bk_UsingEMS).
  
Vous pouvez également utiliser des groupes de distribution universels pour contenir une collection de salles ; par exemple, pour faciliter l’accès aux utilisateurs de rechercher une salle de conférence pour une réunion. Les utilisateurs peuvent ajouter à une liste de salles — un groupe de distribution universel qui contient les boîtes aux lettres de ressources de salle, à une demande de réunion pour rechercher une salle disponible sans avoir à ajouter chaque salle individuellement.
  
Vous pouvez créer un groupe de distribution universel statique qui restent inchangées jusqu'à ce que vous permet de mettre à jour l’appartenance, ou vous pouvez créer un groupe de distribution universel dynamique. Un groupe de distribution universel dynamique interroge les objets à extension messagerie d’Active Directory et génère l’appartenance au groupe en fonction des résultats. L’appartenance au groupe est recalculé à chaque fois qu’un message électronique est envoyé au groupe. 

<a name="bk_SecurityGroup"> </a>

### <a name="security-groups"></a>Groupes de sécurité

Groupes de sécurité et les groupes de distribution universels sont identiques dans la plupart des méthodes. Toutefois, contrairement aux groupes de distribution universels, vous pouvez utiliser des groupes de sécurité pour attribuer des autorisations à des ressources réseau dans AD DS. Vous ne pouvez pas utiliser les API managées EWS pour créer et gérer des groupes de sécurité ; au lieu de cela, vous utilisez les [applets de commande Exchange Management Shell](#bk_UsingEMS). Mais, comme les groupes de distribution universels, vous pouvez utiliser les API managées EWS pour développer les groupes de sécurité.

<a name="bk_ContactGroup"> </a>

### <a name="contact-groups"></a>Groupes de contacts

Si vous souhaitez donner à chaque accès d’administration des utilisateurs au serveur pour créer des groupes de distribution, mais que vous souhaitez leur permettre d’envoyer un message à de grandes quantités de personnes, vous pouvez pour procéder à l’aide de groupes de contacts. Un groupe de contacts ne dispose pas d’une adresse de messagerie associée, et il n’existe que dans la boîte aux lettres d’un utilisateur ; les autres utilisateurs ne sont pas y accéder. Vous pouvez [utiliser les API managées EWS pour créer des groupes de contacts](how-to-create-contact-groups-by-using-ews-in-exchange.md).
  
## <a name="managing-distribution-groups-by-using-the-ews-managed-api-or-ews"></a>Gestion des groupes de distribution à l’aide de l’API managée EWS ou EWS

Vous pouvez utiliser les API managées EWS pour développer un groupe de distribution universel ou un groupe de sécurité et pour contrôler la création et la gestion d’un groupe de contacts ; Toutefois, vous ne pouvez pas utiliser ces technologies pour créer ou modifier les membres de ces groupes. 
  
**Le tableau 1. Opérations EWS pour la gestion des groupes de distribution et les méthodes de l’API managée EWS**

|**Méthode d'API managée EWS**|**Opération EWS**|**Utiliser pour...**|
|:-----|:-----|:-----|
|Méthodes de la [classe ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx)  <br/> |[CreatItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |Créer un groupe de contacts dans la banque d’informations Exchange.<br/><br/>**Remarque**: vous ne pouvez pas créer un groupe de distribution universel ou un groupe de sécurité à l’aide des API managées ou EWS.           |
|[ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |Développez un groupe de distribution universel, un groupe de sécurité ou un groupe de contacts en récupérant une liste de ses membres.  <br/> |
|[FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Rechercher des groupes de contacts dans la boîte aux lettres.  <br/> |
|[GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) <br/> |[GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) <br/> |Récupérer une collection de toutes les salles d’une liste de salles spécifié dans une organisation. Une liste de salles est un groupe de distribution qui contient uniquement des boîtes aux lettres de ressources de salle.  <br/> |
|[ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |Rechercher et retourner des candidats possibles pour correspondre à un nom ambigu. Les candidats peuvent être des groupes de distribution.  <br/> |
   
Vous pouvez utiliser les informations renvoyées par la [expandgroup,](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) méthode ou l’opération [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) pour déterminer quels sont les types de membres dans le groupe. Les types de membres sont définies par l’énumération d’API managées [MailboxType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.mailboxtype%28v=exchg.80%29.aspx) et l’élément EWS [MailboxType](http://msdn.microsoft.com/library/696e5fdb-d8c5-40f0-9e79-885eae65dfa4%28Office.15%29.aspx) . 
  
**Le tableau 2. Types de membres de groupe de distribution**

|**Valeur d’énumération MailboxType**|**Valeur de l’élément MailboxType**|**Description**|
|:-----|:-----|:-----|
|Mailbox  <br/> |Mailbox  <br/> |Un objet Active Directory à extension messagerie.  <br/> |
|PublicGroup  <br/> |PublicDL  <br/> |Un groupe de distribution contenu dans le groupe que vous venez de développer. Pour obtenir une liste complète des membres, développez ce groupe.  <br/> |
|ContactGroup  <br/> |PrivateDL  <br/> |Un groupe de contacts qui se trouve dans la boîte aux lettres et n’est disponible pour les utilisateurs de cette boîte aux lettres.  <br/> |
|Contact  <br/> |Contact  <br/> |Un contact de base de données Exchange ou d’un contact de messagerie Active Directory.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="managing-distribution-groups-by-using-the-exchange-management-shell"></a>Gestion des groupes de distribution à l’aide d’Exchange Management Shell

Vous pouvez [utiliser les applets de commande Exchange Management Shell](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx) pour créer et gérer les groupes de distribution universels et les groupes de sécurité dans votre code. 
  
> [!NOTE]
> Vous ne pouvez pas utiliser les applets de commande Exchange Management Shell pour gérer les groupes de contacts. 
  
**Le tableau 3. Applets de commande Exchange Management Shell pour travailler avec des groupes de distribution**

|**Applet de commande**|**Utiliser pour...**|
|:-----|:-----|
|[Disable-DistributionGroup](http://technet.microsoft.com/en-us/library/aa997942%28v=exchg.150%29.aspx) <br/> |Supprimer des fonctionnalités de messagerie d’un groupe de distribution à extension messagerie.  <br/> |
|[Enable-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998916%28v=exchg.150%29.aspx) <br/> |Activer la messagerie d’un groupe universel existant.  <br/> |
|[Get-DistributionGroup](http://technet.microsoft.com/en-us/library/bb124755%28v=exchg.150%29.aspx) <br/> |Requête pour les groupes de distribution existants.  <br/> |
|[Nouveau groupe de distribution](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx) <br/> |Créer un groupe de distribution.  <br/> |
|[Remove-DistributionGroup](http://technet.microsoft.com/en-us/library/aa997627%28v=exchg.150%29.aspx) <br/> |Supprimer un groupe de distribution existant de domaine Active Directory.  <br/> |
|[Set-DistributionGroup](http://technet.microsoft.com/en-us/library/bb124955%28v=exchg.150%29.aspx) <br/> |Modifier les paramètres d’un groupe de distribution existant.  <br/> |
|[Ajouter-DistributionGroupMember](http://technet.microsoft.com/en-us/library/bb124340%28v=exchg.150%29.aspx) <br/> |Ajouter un destinataire à un groupe de distribution.  <br/> |
|[Get-DistributionGroupMember](http://technet.microsoft.com/en-us/library/aa996367%28v=exchg.150%29.aspx) <br/> |Trouvez des membres du groupe de distribution existant.  <br/> |
|[Remove-DistributionGroupMember](http://technet.microsoft.com/en-us/library/aa998016%28v=exchg.150%29.aspx) <br/> |Supprimer un destinataire existant d’un groupe de distribution.  <br/> |
|[Mise à jour-DistributionGroupMember](http://technet.microsoft.com/en-us/library/dd335049%28v=exchg.150%29.aspx) <br/> |Mettre à jour un membre d’un groupe de distribution spécifié.  <br/> |
|[Get-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb124762%28v=exchg.150%29.aspx) <br/> |Récupérer les paramètres dans un groupe de distribution dynamique existant.  <br/> |
|[Nouvelle-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb125127%28v=exchg.150%29.aspx) <br/> |Créer un groupe de distribution dynamique.  <br/> |
|[Remove-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb125038%28v=exchg.150%29.aspx) <br/> |Supprimer un groupe de distribution dynamique existant. Cette cmdlet supprime le groupe de distribution dynamique à partir d’AD DS.  <br/> |
|[Set-DynamicDistributionGroup](http://technet.microsoft.com/en-us/library/bb123796%28v=exchg.150%29.aspx) <br/> |Modifier les paramètres d’un groupe de distribution dynamique existant.  <br/> |

<a name="bk_UsingEMS"> </a>

## <a name="in-this-section"></a>In this section

- [Créer des groupes de contacts à l’aide de EWS dans Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)   
- [Développez les groupes de distribution à l’aide EWS dans Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)   
- [Cmdlets d’appel Exchange Management Shell à partir du Code managé](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx)
    

