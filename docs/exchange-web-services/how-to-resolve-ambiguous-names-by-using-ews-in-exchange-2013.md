---
title: Résoudre des noms ambigus en utilisant EWS dans Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Découvrez comment utiliser les API managées EWS pour résoudre les noms ambigus en obtenant les correspondances possibles à partir des Services de domaine Active Directory (AD DS) ou un dossier de contacts dans la boîte aux lettres de l’utilisateur.
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754931"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Résoudre des noms ambigus en utilisant EWS dans Exchange 2013

Découvrez comment utiliser les API managées EWS pour résoudre les noms ambigus en obtenant les correspondances possibles à partir des Services de domaine Active Directory (AD DS) ou un dossier de contacts dans la boîte aux lettres de l’utilisateur.
  
Une liste de noms et les adresses manuscrite est proposée à un utilisateur dans votre organisation pour les employés ayant participé à une session de formation. Pour envoyer un message électronique avec des informations supplémentaires à des personnes dans la liste, mais ils ne peuvent pas lire adresse de messagerie de tout le monde. Si vous souhaitez résoudre ce problème pour vos utilisateurs dans votre application, EWS peut aider. Vous pouvez utiliser la méthode d’API managées [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) ou l’opération EWS [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) pour renvoyer une liste de correspondances potentielles pour une sélection de texte, tel que partie d’un nom de famille. Les éléments retournés peuvent être boîtes aux lettres des utilisateurs publics, des groupes de distribution et les contacts. 
  
Notez que Exchange enregistre les adresses de messagerie avec des types de routage préfixés, tel que smtp ou sip, dans un tableau à valeurs multiples. La méthode **ResolveName** et l’opération **ResolveNames** effectuent une correspondance partielle dans chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « sip : User1 ». Si vous ne spécifiez pas un type de routage, la méthode ou l’opération sera smtp par défaut, faire correspondre à une propriété d’adresse smtp principale et recherche pas dans le tableau à valeurs multiples. Par exemple, si vous recherchez User1 et que vous n’incluez pas le préfixe sip, vous pas reçoit sip:User1@Contoso.com ainsi, même si c’est une boîte aux lettres valide. 
  
Vous pouvez uniquement spécifier un nom ambigu dans une demande unique. Si vous disposez d’une liste de noms ambigus à résoudre, vous devez parcourir la liste et appelez la méthode ou l’opération pour chaque entrée. Candidats à partir du dossier de Contacts d’un utilisateur a une valeur non nulle élément ID, qui peut ensuite être utilisée dans un appel de la méthode [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) ou d’une requête d’opération [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) pour récupérer des informations supplémentaires. Si le candidat est un groupe de distribution, vous pouvez utiliser la méthode d’API managées [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) ou l’opération EWS [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) pour obtenir la liste des membres. Si le paramètre _returnContactDetails_ ou l’attribut EWS **ReturnFullContactData** est définie sur true, les entrées d’Active Directory renvoyées par le biais d’une méthode **ResolveName** ou opération **ResolveNames** inclut des propriétés supplémentaires qui décrivent le contact. Le paramètre _returnContactDetails_ ou l’attribut **ReturnFullContactData** ne pas avoir une incidence sur les données renvoyées pour les contacts et des groupes de contacts. 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>Résoudre des noms ambigus à l’aide des API managées
<a name="bk_EWSMA"> </a>

Vous pouvez utiliser la méthode [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) pour rechercher les candidats qui correspondent au nom ambigu que vous passez. Vous pouvez utiliser des surcharges de la méthode **ResolveName** pour rechercher les candidats de cinq façons différentes. 
  
**Le tableau 1. Méthodes ResolveName surchargées**

|**M?thode**|**Son fonctionnement**|
|:-----|:-----|
|[ResolveName(String)](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |Recherche de contacts dans le dossier Contacts de l’utilisateur et la liste d’adresses globale (LAG), dans cet ordre. La variable de chaîne est le nom ambigu que vous essayez de résoudre.  <br/> |
|[ResolveName (chaîne, ResolveNameSearchLocation, Boolean)](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |Recherche de contacts dans le dossier Contacts par défaut et/ou la liste d’adresses globale (LAG). La valeur de chaîne est le nom ambigu, l’emplacement de recherche spécifie le dossier Contacts et/ou la liste d’adresses globale, et la valeur booléenne indique s’il faut renvoyer les informations de contact.  <br/> |
|[ResolveName (chaîne, ResolveNameSearchLocation, Boolean, PropertySet)](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |Recherche de contacts dans le dossier Contacts par défaut et/ou la liste d’adresses globale (GAL). Cette méthode vous permet de vous permet de définir les propriétés qui sont retournées.  <br/> |
|[ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |Recherche de contacts dans des dossiers de contacts spécifiées et/ou la liste d’adresses globale (LAG). Vous pouvez utiliser cette méthode pour passer une collection de dossiers à rechercher. Cela vous permet de rechercher dans les dossiers de contacts autre que le dossier Contacts par défaut.  <br/> |
|[ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |Recherche de contacts dans la liste d’adresses globale (LAG) et/ou dans des dossiers de contacts. Cette méthode vous permet de vous permet de définir les propriétés qui sont retournées.  <br/> |
   
Commençons par un exemple simple. L’exemple suivant montre comment résoudre la chaîne de texte « dan » et de sortie de l’adresse e-mail et le nom de chaque candidat trouvé. Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange. 
  
```cs
// Resolve the ambiguous name "dan".
   NameResolutionCollection resolvedNames = service.ResolveName("dan");
   // Output the list of candidates.
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

La réponse renvoie un maximum de 100 candidats, bien qu’il peut y avoir plus de 100 candidats potentiels. Pour déterminer si uniquement les 100 premières candidats d’un plus grand nombre de candidats ont été retournés, vérifiez la valeur de [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) dans l’objet [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) . Si la valeur est true, il n’existe pas plus possible de candidats ; Si la valeur est false, la méthode renvoyée uniquement les 100 premières d’un plus grand nombre de candidats potentiels. 
  
Si vous travaillez dans une organisation de grande taille, il est probable qu’un nom tel que « dan » renverra le nombre maximal de 100 candidats. Pour réduire le nombre de candidats renvoyée, limitez dans lequel vous recherchez. L’exemple suivant utilise l’énumération [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) pour spécifier où chercher pour résoudre le nom ambigu. 
  
```cs
// Resolve the ambiguous name "dan".
// Only use the Contacts folder.
   NameResolutionCollection resolvedNames = service.ResolveName("dan", ResolveNameSearchLocation.ContactsOnly, false);
   // Output the list of candidates.   
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

Si vous stockez vos contacts dans un dossier autre que le dossier Contacts connu, utilisez une des méthodes surchargées pour indiquer où rechercher les candidats. L’exemple suivant crée une liste de dossiers pour la méthode **ResolveName** en fonction de l’ID de dossier. L' **ID FolderId** a été raccourcie pour des raisons de lisibilité. 
  
```cs
// Create a list to store folders to search.
List<FolderId> folders = new List<FolderId>();
// Add a folder to the list based on the FolderId.
folders.Add(new FolderId("AABR8mboAAA="));
// Resolve the ambiguous name "dan".
// Only use the folders specified.
NameResolutionCollection resolvedNames = service.ResolveName("dan", folders, ResolveNameSearchLocation.ContactsOnly, false);
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

Si vous appliquez des filtres et aucune candidats ne sont renvoyées, la [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) contient zéro entrées. Vous pouvez le vérifier en examinant la propriété [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) de la collection. 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>Résoudre des noms ambigus à l’aide de EWS
<a name="bk_EWSMA"> </a>

Vous pouvez utiliser l’opération EWS [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) pour identifier les candidats possibles pour un nom ambigu. L’élément [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) contient le nom ambigu à résoudre. L’exemple suivant montre comment résoudre le nom Sadie. C’est également la demande XML par l’API managée EWS lorsque vous [Utilisez la méthode ResolveName](#bk_EWSMA), sauf qu’elle utilise un nom différent pour les exemples de sortie valide.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

La réponse renvoie un maximum de 100 candidats, bien qu’il peut y avoir plus de 100 candidats potentiels pour déterminer si uniquement les 100 premières candidats d’un plus grand nombre de candidats ont été retournés, vérifiez la valeur de [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribut de l’élément [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) . Si la valeur est true, il n’existe pas plus possible de candidats ; Si la valeur est false, l’opération renvoyée uniquement les 100 premières d’un plus grand nombre de candidats potentiels. 
  
L’exemple suivant montre la réponse XML lorsqu’un candidat est trouvé. N’oubliez pas la [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) peut contenir jusqu'à 100 candidats, chacun d’eux représenté par l’élément de la [solution](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) et ses éléments enfants. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>Sadie@Contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:Sadie@Contoso.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

Vous allez pas toujours pour rechercher des candidats pour votre nom ambigu. L’exemple suivant montre la réponse XML, comme une erreur, lorsque aucun candidats ne sont détectés.
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>

```

## <a name="see-also"></a>Voir aussi


- [Personnes et contacts dans EWS dans Exchange](people-and-contacts-in-ews-in-exchange.md)
    
- [Développez les groupes de distribution à l’aide EWS dans Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

