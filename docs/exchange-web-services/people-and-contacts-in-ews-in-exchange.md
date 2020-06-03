---
title: Personnes et contacts dans EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 043c33be-a0d1-4bad-a840-85715eda4813
description: Découvrez les personnages, le magasin de contacts unifié et comment travailler avec les contacts à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: f0590a0d8a99b8320cc1b316829177e05e443de6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457671"
---
# <a name="people-and-contacts-in-ews-in-exchange"></a>Personnes et contacts dans EWS dans Exchange

Découvrez les personnages, le magasin de contacts unifié et comment travailler avec les contacts à l’aide de l’API managée EWS ou d’EWS dans Exchange. 
  
Les contacts sont des éléments d’Exchange qui stockent des informations sur une personne, un groupe ou une organisation. Les contacts peuvent inclure des noms et des adresses de messagerie, ainsi que d’autres informations, notamment des adresses de messagerie instantanée, des adresses physiques, des anniversaires, des informations familiales, ainsi qu’une photo ou une image qui représente le contact.
  
Les informations de contact sont stockées à l’un des deux emplacements suivants :
  
- Services de domaine Active Directory (AD DS), si le contact se trouve dans l’organisation.
    
- Le dossier contacts ou un autre dossier de la boîte aux lettres d’un utilisateur, si le contact se trouve à l’extérieur de l’organisation.
    
Plusieurs éléments de contact peuvent représenter une seule personne. Exchange utilise des personnages pour vous aider à rassembler ces différents éléments de contact. Un *personnage* est une agrégation d’informations de contact pour la même personne de différentes sources. En plus des informations de contact dans Exchange, les personnages peuvent également être regroupés à partir des informations contenues dans le cache de destinataires de la boîte aux lettres, d’un dossier masqué pour les contacts de messagerie instantanée appelés QuickContacts et de sources de données tierces. Le magasin de contacts unifié dans Exchange permet aux clients de messagerie instantanée d’utiliser cette agrégation ; la seule différence réside dans le fait que le magasin de contacts unifié ne regroupe pas d’informations à partir des services AD DS, comme illustré dans la figure 1. 
  
**Figure 1. Sources d’informations de contact pour les personnes et le magasin de contacts unifié**

![Image illustrant les sources qui sont regroupées en personas et les sources qui sont incluses dans le magasin de contacts unifié. Ce dernier n’agrège pas les informations de contact du service d’annuaire.](media/EX15_PersonaOverview.png)
  
**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour l’utilisation de contacts**

|**Si vous souhaitez...**|**Utiliser cette méthode d’API managée EWS**|**Utiliser cette opération EWS**|
|:-----|:-----|:-----|
|Créer un contact  <br/> |Instancier un nouvel objet [contact](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) et utiliser [contact. Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) <br/> |
|Copier un contact  <br/> |[Contact. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Déplacer un contact  <br/> |[Contact. Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Mettre à jour un contact existant  <br/> |[Contact. bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) et [contact. Update](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.update%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/298fdd71-a83d-4407-9728-4f0a8e2d857c%28Office.15%29.aspx) <br/> |
|Supprimer un contact  <br/> |[Contact. bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) et [contact. Delete](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.delete%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
|Rechercher un contact  <br/> |[ExchangeService. FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
|Rechercher des contacts  <br/> |N/A  <br/> |[FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |
|Développer un groupe de distribution  <br/> |[ExchangeService. Expandgroup,](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) <br/> |[ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) <br/> |
|Résoudre un nom ambigu  <br/> |[ExchangeService. ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |
|Obtenir un personnage  <br/> |N/A  <br/> |[GetPersona](https://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |
|Utiliser des photos de contacts  <br/> |[Contact. SetContactPicture](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx), [contact. GetContactPictureAttachment](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.getcontactpictureattachment%28v=exchg.80%29.aspx)ou [contact. RemoveContactPicture](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.setcontactpicture%28v=exchg.80%29.aspx) <br/> |[GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) ou [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/> |
   
## <a name="personas"></a>Personnages
<a name="PEOPLESEARCH"> </a>

Jusqu’à récemment, les contacts étaient généralement stockés dans un seul emplacement, généralement sur un client de messagerie. Aujourd’hui, il est de plus en plus courant de stocker les contacts dans différents emplacements, comme sur un téléphone, sur un site de réseau social, dans un dossier de contacts dans une boîte aux lettres Exchange ou dans le service d’annuaire d’une organisation. Avec la prolifération des informations de contact, il est possible que plusieurs contacts qui représentent la même personne contiennent des informations différentes ; par exemple, un contact peut inclure un numéro de téléphone professionnel et un autre numéro de téléphone personnel, ou un contact stocké dans un dossier de contacts peut avoir un nom différent du contact de la même personne stockée sur votre téléphone.
  
Dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir d’Exchange 2013, les contacts de sources différentes qui représentent la même personne sont associés à un autre, de la même manière que les messages électroniques sont regroupés en conversations, par le biais d’un ID de lien commun. Lorsque des informations de contact agrégées sont renvoyées par un serveur Exchange, elles incluent un ensemble d’attributs pour chaque contact, comme un dossier source, un nom d’affichage, un ID et un ID source. La somme des propriétés et attributs renvoyés est appelé un personnage, et l’ensemble de propriétés renvoyées est appelé [forme du personnage](https://msdn.microsoft.com/library/61d87cd5-3270-40d1-bab7-d0d5bf938607%28Office.15%29.aspx).
  
Étant donné que les informations qui composent un personnage ne sont pas stockées dans un seul et même emplacement, et que ces informations peuvent être modifiées à tout moment, un personnage est créé uniquement lorsque vous effectuez une requête auprès d’un serveur Exchange. Vous utilisez l’opération EWS [FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) pour effectuer une demande de recherche de Persona. Votre requête peut inclure un ordre de tri et peut être filtrée en fonction d’une chaîne de requête pour vous aider à trouver le personnage correct en commandant et en filtrant les résultats. Par exemple, vous pouvez récupérer le nom complet et un ensemble de toutes les adresses de messagerie associées à un contact spécifique à partir du dossier de contacts, d’un compte LinkedIn, d’un compte LinkedIn et du service d’annuaire d’une entreprise, ou vous pouvez récupérer un ensemble de personnes ayant des adresses de messagerie instantanée. La liaison de contacts dans Personas est automatique sur la base d’un algorithme qui reconnaît une relation entre les contacts stockés sur différents appareils. 
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
**Tableau 2. Opérations EWS pour utiliser des personnes**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Renvoie tous les personnages disponibles à partir d’un dossier de contacts spécifié ou récupère les contacts qui correspondent à une chaîne de requête spécifiée.  <br/> |
|[GetPersona](https://msdn.microsoft.com/library/e2146df0-53d0-4caf-9758-b600bbc14b6a%28Office.15%29.aspx) <br/> |Renvoie un jeu de propriétés associé à un personnage spécifique, comme toutes les adresses de messagerie instantanée ou les noms d’affichage pour un ID de personnage spécifié.  <br/> |
   
Vous pouvez utiliser les opérations **GetPersona** et **FindPeople** pour récupérer efficacement les informations de contact à partir de plusieurs sources. Étant donné que tous les éléments liés à un personnage sont associés à un ID de lien, vous pouvez utiliser ces opérations dans une large gamme d’applications qui utilisent des données de contact. Voici quelques exemples : 
  
- Application de téléphone mobile qui utilise l’opération **GetPersona** lorsqu’un utilisateur appelle un contact, puis propose des numéros de téléphone supplémentaires à appeler s’il n’y a aucune réponse. 
    
- Application qui utilise l’opération **FindPeople** pour analyser les messages de la boîte de réception des adresses de messagerie afin de déterminer si elles se trouvent dans un personnage existant. Les adresses qui ne sont pas déjà associées à un personnage peuvent être utilisées pour créer des prospects commerciaux ou répertorier toutes les communications récentes avec la personne représentée par ce personnage. 
    
- [Une application de messagerie pour Outlook](mail-apps-for-outlook-and-ews-in-exchange.md) qui offre différentes salutations selon que la correspondance est formelle ou informelle. Les salutations formelles sont fournies par les noms d’affichage du service d’annuaire et les salutations informelles proviennent du nom d’affichage qui provient des contacts de réseau social. 
    
## <a name="unified-contact-store"></a>Magasin de contacts unifié
<a name="PEOPLESEARCH"> </a>

Les personnages ne sont pas simplement limités à un client de messagerie. Si vous développez un client de messagerie instantanée, vous pouvez vous demander un ou plusieurs des éléments suivants :
  
- Comment puis-je configurer les applications clientes Lync avec un ensemble par défaut d’éléments de contact de messagerie instantanée ?
    
- Comment puis-je gérer les listes de contacts et de groupes de messagerie instantanée ?
    
- Comment puis-je gérer l’accès client Lync personnalisé aux contacts de messagerie instantanée et aux groupes de messagerie instantanée ?
    
Le magasin de contacts unifié fonctionne en arrière-plan dans Exchange pour regrouper les données de contact à partir d’Exchange et d’autres sources dans une seule entité ou un seul personnage. Bien que les opérations EWS que vous utilisez pour accéder au magasin de contacts unifié soient propres aux contacts de messagerie instantanée, vous pouvez utiliser le magasin de contacts unifié dans Exchange pour travailler avec des personnes dans tous les types d’applications. N’oubliez pas que le magasin de contacts unifié ne peut pas accéder aux données de contact AD DS.
  
Les contacts de messagerie instantanée sont stockés dans un dossier masqué nommé QuickContacts. Vous pouvez utiliser les opérations **AddNewImContactToGroup** et **AddImContactToGroup** pour ajouter des contacts à des groupes qui sont stockés dans ce dossier masqué. Étant donné que vous pouvez utiliser le magasin de contacts unifié pour regrouper les contacts de messagerie instantanée, vous pouvez accéder aux groupes de contacts et les mettre à jour plus facilement. 
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
**Tableau 3. Opérations EWS pour accéder au magasin de contacts unifié**

|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[AddNewImContactToGroup](https://msdn.microsoft.com/library/0cb5525f-faa3-48f1-9551-df55ffc26f46%28Office.15%29.aspx) <br/> |Ajoute un nouveau contact de messagerie instantanée à un groupe de messagerie instantanée, avec un maximum de 1000 contacts.  <br/> |
|[AddImContactToGroup](https://msdn.microsoft.com/library/376acc42-2684-4596-aca1-82a4a10865c9%28Office.15%29.aspx) <br/> |Ajoute un contact de messagerie instantanée existant à un groupe de messagerie instantanée, avec un maximum de 1000 contacts.  <br/> |
|[AddImGroup](https://msdn.microsoft.com/library/6df6e504-b7c8-4773-b10f-ffa5defac229%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de messagerie instantanée, avec un maximum de 64 groupes.  <br/> |
|[AddDistributionGroupToImList](https://msdn.microsoft.com/library/5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a%28Office.15%29.aspx) <br/> |Ajoute un nouveau groupe de distribution à un groupe de messagerie instantanée, avec un maximum de 64 groupes.  <br/> |
|[GetImItemList](https://msdn.microsoft.com/library/e31d14e1-0c1f-4b69-98b7-157d59c13698%28Office.15%29.aspx) <br/> |Récupère une liste de groupes de messagerie instantanée et de personnes de contact de messagerie instantanée.  <br/> |
|[GetImItems](https://msdn.microsoft.com/library/51186691-46d2-4d5c-b8bc-4ee2bb20fbe7%28Office.15%29.aspx) <br/> |Récupère des informations sur des groupes de messagerie instantanée et des personnages de contact de messagerie instantanée spécifiques.  <br/> |
|[RemoveContactFromImList](https://msdn.microsoft.com/library/28ec96c3-45af-48ff-9f17-718a527dc0ad%28Office.15%29.aspx) <br/> |Supprime un contact d’un groupe de messagerie instantanée.  <br/> |
|[RemoveImContactFromGroup](https://msdn.microsoft.com/library/a190bbec-c71b-4e6a-880b-55854c724d8c%28Office.15%29.aspx) <br/> |Supprime un contact de messagerie instantanée d’un groupe de messagerie instantanée.  <br/> |
|[RemoveDistributionGroupFromImList](https://msdn.microsoft.com/library/252bddf2-98b6-4824-b548-2fba2bda5384%28Office.15%29.aspx) <br/> |Supprime un groupe de distribution d’un groupe de messagerie instantanée.  <br/> |
|[RemoveImGroup](https://msdn.microsoft.com/library/5e788016-68e0-4a3f-9243-03f6b6c6b389%28Office.15%29.aspx) <br/> |Supprime un groupe de messagerie instantanée.  <br/> |
|[SetImGroup](https://msdn.microsoft.com/library/2d48aa07-8152-4c3d-a519-061253e80174%28Office.15%29.aspx) <br/> |Modifie le nom d’affichage d’un groupe de messagerie instantanée.  <br/> |
   
## <a name="in-this-section"></a>Dans cette section
<a name="PEOPLESEARCH"> </a>

- [Traiter les contacts par lots à l’aide d’EWS dans Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    
- [Résoudre des noms ambigus à l’aide d’EWS dans Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    
- [Obtenir des photos de l’utilisateur à l’aide d’EWS dans Exchange](how-to-get-user-photos-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi
<a name="PEOPLESEARCH"> </a>

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

