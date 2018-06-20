---
title: Personnes et des contacts dans EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 043c33be-a0d1-4bad-a840-85715eda4813
description: Découvrez les personnages, le magasin de contacts unifié et comment travailler avec des contacts à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: fe11c6247cade8e78610d953088f6d593bdb560c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755060"
---
# <a name="people-and-contacts-in-ews-in-exchange"></a>Personnes et des contacts dans EWS dans Exchange

Découvrez les personnages, le magasin de contacts unifié et comment travailler avec des contacts à l’aide de l’API managée EWS ou EWS dans Exchange. 
  
Les contacts sont des éléments qui stockent des informations sur une personne, groupe ou organisation dans Exchange. Contacts peuvent inclure des noms et les adresses de messagerie et d’autres informations, y compris les adresses de messagerie instantanée, les adresses physiques, anniversaires, informations sur la famille et une photo ou image qui représente le contact.
  
Informations de contact sont stockées dans un des deux emplacements :
  
- Services de domaine Active Directory (AD DS), si le contact se trouve dans l’organisation.
    
- Le dossier de Contacts ou un autre dossier de boîte aux lettres d’un utilisateur, si le contact est en dehors de l’organisation.
    
Plusieurs éléments de contact peuvent représenter une seule personne. Exchange utilise les personnages pour aider à rassembler les différents éléments de contact. Un *personnage* est un regroupement des informations de contact de la même personne provenant de différentes sources. En outre pour les informations de contact dans Exchange, les personnages peuvent également être regroupés à partir des informations dans le cache de destinataires pour la boîte aux lettres, un dossier de contacts de messagerie instantanée appelée QuickContacts, masqué et à partir de sources de données tierces. Le magasin de contacts unifié dans Exchange permet aux clients de messagerie instantanée à utiliser cette agrégation ; la seule différence est que le magasin de contacts unifié n’agrège pas les informations de domaine Active Directory, comme indiqué dans la Figure 1. 
  
**La figure 1. Sources d’informations de contact pour les personnages et le magasin de contacts unifié**

![Image illustrant les sources qui sont regroupées en personas et les sources qui sont incluses dans le magasin de contacts unifié. Ce dernier n’agrège pas les informations de contact du service d’annuaire.](media/EX15_PersonaOverview.png)
  
**Le tableau 1. Méthodes d’API managées et opérations EWS pour travailler avec des contacts**

|**Si vous souhaitez...**|**Utilisez cette méthode de l’API managée EWS**|**Utilisez cette opération EWS**|
|:-----|:-----|:-----|
|Créer un nouveau contact  <br/> |Instanciez un nouvel objet [Contact](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) et utilisez [Contact.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) <br/> |
|Copier un contact  <br/> |[Contact.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Déplacer un contact  <br/> |[Contact.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Mettre à jour un contact existant  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) et [Contact.Update](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.update%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/298fdd71-a83d-4407-9728-4f0a8e2d857c%28Office.15%29.aspx) <br/> |
|Supprimer un contact  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) et [Contact.Delete](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.delete%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
|Rechercher un contact  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
|Rechercher des personnes  <br/> |S/O  <br/> |[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |
|Développez un groupe de distribution  <br/> |[ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |
|Résoudre un nom ambigu  <br/> |[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |
|Obtenir un personnage  <br/> |S/O  <br/> |[GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |
|Utilisation de photos des contacts  <br/> |[Contact.SetContactPicture](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx), [Contact.GetContactPictureAttachment](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.getcontactpictureattachment%28v=exchg.80%29.aspx)ou [Contact.RemoveContactPicture](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx) <br/> |[GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) ou [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/> |
   
## <a name="personas"></a>Personnage
<a name="PEOPLESEARCH"> </a>

Jusqu'à récemment, contacts ont été généralement stockées dans un seul emplacement : en règle générale, sur un client de messagerie. Aujourd'hui, il devient plus courant de stocker des contacts à de nombreux emplacements différents, comme un téléphone, sur un site de réseau social, dans un dossier Contacts dans une boîte aux lettres Exchange, ou dans le service d’annuaire d’une organisation. Avec la prolifération des informations de contact, il est possible que plusieurs contacts qui représentent la même personne contiennent des informations différentes ; par exemple, un contact peut inclure un numéro de téléphone professionnel et un autre un numéro de téléphone personnel ou un contact stocké dans un dossier de Contacts peut avoir un nom différent de celui du contact pour la personne qui est stocké sur votre téléphone.
  
Dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange commençant par Exchange 2013, les contacts à partir de différentes sources qui représentent la même personne associées à l’autre, similaire à la façon dont les messages électroniques sont regroupées dans les conversations, au moyen d’un ID de lien courantes. Lorsque les informations de contact agrégées sont renvoyées par un serveur Exchange, il inclut un ensemble d’attributs pour chaque contact, comme un dossier source, un nom complet, un ID et un ID de la source. La somme des propriétés et attributs retournés est appelée un personnage et le jeu de propriétés renvoyé est appelé à la [forme du personnage](http://msdn.microsoft.com/library/61d87cd5-3270-40d1-bab7-d0d5bf938607%28Office.15%29.aspx).
  
Étant donné que les informations qui constitue un personnage ne sont pas stockées dans un seul emplacement et étant donné que ces informations peuvent être modifiées à tout moment, un personnage est créé uniquement lorsque vous effectuez une demande à un serveur Exchange. Vous utilisez l’opération EWS [FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) pour effectuer une demande de recherche personnage. Votre demande peut inclure un ordre de tri et peut être filtrée en fonction d’une chaîne de requête pour vous aider à trouver le personnage correct par tri et filtrage des résultats. Par exemple, vous pouvez récupérer le nom complet et un ensemble de toutes les adresses de messagerie qui sont associés à un contact spécifique à partir du dossier Contacts, un compte Hotmail, un compte LinkedIn et service d’annuaire de l’entreprise, ou vous pouvez extraire un ensemble de toutes les personnes qui posséder des adresses de messagerie instantanée. Liaison de contacts dans personnages est automatique selon un algorithme qui reconnaît une relation entre les contacts stockés sur différents périphériques. 
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
**Le tableau 2. Opérations EWS pour l’utilisation de personnages**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Renvoie tous les personnages disponibles à partir d’un dossier contacts spécifié ou récupère les contacts qui correspondent à une chaîne de requête spécifiée.  <br/> |
|[GetPersona](http://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Renvoie un ensemble de propriétés associées à un personnage spécifique, telles que le message instantané adresses ou les noms complets pour un ID de personnage spécifié.  <br/> |
   
Vous pouvez utiliser les opérations **GetPersona** et **FindPeople** pour récupérer des informations de contact à partir de plusieurs sources. Étant donné que tous les éléments associés à un personnage sont associés à un ID de lien, vous pouvez utiliser ces opérations dans une large gamme d’applications qui utilisent des données de contact. Voici quelques exemples : 
  
- Une application de téléphone mobile qui utilise l’opération **GetPersona** lorsqu’un utilisateur appelle un contact, puis propose les autres numéros de téléphone à appeler si aucun participant ne répond. 
    
- Une application qui utilise l’opération **FindPeople** pour analyser les messages de boîte de réception pour les adresses de messagerie déterminer si elles se trouvent dans personnage existant. Les adresses qui ne sont pas déjà associés à un personnage peuvent être utilisées pour créer les ventes potentielles ou liste toutes les communications récentes avec la personne représentée par ce personnage. 
    
- [Une application de messagerie pour Outlook](mail-apps-for-outlook-and-ews-in-exchange.md) offrant différents appels selon que la correspondance est formelle ou informelle. Formules de politesse formelles sont fournis par les noms d’affichage du service d’annuaire et le nom complet provenant de contacts des réseaux sociaux provenant de politesse informelle. 
    
## <a name="unified-contact-store"></a>Magasin de contacts unifié
<a name="PEOPLESEARCH"> </a>

Personnages ne sont pas uniquement limités à un client de messagerie. Si vous développez un client de messagerie instantanée, vous pouvez vous demander tout ou partie des éléments suivants :
  
- Comment puis-je mettre en service les applications de client Lync avec un ensemble par défaut des éléments de contact de messagerie instantanée ?
    
- Comment gérer les contacts de messagerie instantanée et des listes de groupe ?
    
- Comment gérer les accès au client Lync personnalisé pour les contacts de messagerie instantanée et les groupes de messagerie instantanée ?
    
Le magasin de contacts unifié fonctionne en arrière-plan dans Exchange contact agréger des données à partir d’Exchange et d’autres sources dans une seule entité ou personnage. Bien que les opérations EWS qui vous permet d’accéder au magasin de Contact unifié sont spécifiques à des contacts de messagerie instantanée, vous pouvez utiliser le magasin de contacts unifié dans Exchange pour travailler avec les personnages dans tous les types d’applications. N’oubliez pas que le magasin de contacts unifié ne peut pas accéder à des données de contacts AD DS.
  
Contacts de messagerie instantanée sont stockés dans un dossier caché appelé QuickContacts. Vous pouvez utiliser les opérations **AddNewImContactToGroup** et **AddImContactToGroup** pour ajouter des contacts à des groupes qui sont stockés dans ce dossier masqué. Et parce que vous pouvez utiliser le magasin de contacts unifié pour regrouper les contacts de messagerie instantanée, vous pouvez accéder et mettre à jour des groupes de contacts plus facilement. 
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
**Le tableau 3. Opérations EWS pour accéder au magasin de Contact unifié**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[AddNewImContactToGroup](http://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Ajoute un nouveau contact de messagerie instantanée à un groupe de messagerie instantanée, avec un maximum de 1000 contacts.  <br/> |
|[AddImContactToGroup](http://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Ajoute un contact de messagerie instantanée existant à un groupe de messagerie instantanée, avec un maximum de 1000 contacts.  <br/> |
|[AddImGroup](http://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de messagerie instantanée avec un maximum de 64 groupes.  <br/> |
|[AddDistributionGroupToImList](http://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de distribution à un groupe de messagerie instantanée, avec un maximum de 64 groupes.  <br/> |
|[GetImItemList](http://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Récupère une liste des groupes de messagerie instantanée et des personnes de contact de messagerie instantanée.  <br/> |
|[GetImItems](http://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Récupère des informations à propos des groupes spécifiques de messagerie instantanée et messagerie instantanée contact personnages.  <br/> |
|[RemoveContactFromImList](http://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Supprime un contact d’un groupe de messagerie instantanée.  <br/> |
|[RemoveImContactFromGroup](http://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Supprime un contact de messagerie instantanée à partir d’un groupe de messagerie instantanée.  <br/> |
|[RemoveDistributionGroupFromImList](http://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Supprime un groupe de distribution à partir d’un groupe de messagerie instantanée.  <br/> |
|[RemoveImGroup](http://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Supprime un groupe de messagerie instantanée.  <br/> |
|[SetImGroup](http://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Modifie le nom complet d’un groupe de messagerie instantanée.  <br/> |
   
## <a name="in-this-section"></a>Dans cette section
<a name="PEOPLESEARCH"> </a>

- [Contacts processus par lots à l’aide de EWS dans Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    
- [Résoudre des noms ambigus en utilisant EWS dans Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    
- [Obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange](how-to-get-user-photos-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi
<a name="PEOPLESEARCH"> </a>

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

