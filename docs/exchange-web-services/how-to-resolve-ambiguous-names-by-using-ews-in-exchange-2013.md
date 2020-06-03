---
title: Résoudre des noms ambigus à l’aide d’EWS dans Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Découvrez comment utiliser l’API managée EWS ou EWS pour résoudre des noms ambigus en obtenant les correspondances possibles des services de domaine Active Directory (AD DS) ou d’un dossier de contacts dans la boîte aux lettres de votre utilisateur.
ms.openlocfilehash: 5e30e268f54e6ca257e188592e49d168e64332ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527746"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Résoudre des noms ambigus à l’aide d’EWS dans Exchange 2013

Découvrez comment utiliser l’API managée EWS ou EWS pour résoudre des noms ambigus en obtenant les correspondances possibles des services de domaine Active Directory (AD DS) ou d’un dossier de contacts dans la boîte aux lettres de votre utilisateur.
  
Un utilisateur de votre organisation reçoit une liste manuscrite de noms et d’adresses pour les employés qui ont participé à une session de formation. Ils veulent envoyer un courrier électronique contenant des informations supplémentaires à des personnes figurant dans la liste, mais ils ne peuvent pas lire l’adresse de messagerie de tous les utilisateurs. Si vous souhaitez résoudre ce problème pour vos utilisateurs dans votre application, EWS peut vous aider. Vous pouvez utiliser la méthode de l’API managée EWS [ExchangeService. ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) ou l’opération EWS [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) pour renvoyer une liste de correspondances potentielles pour une sélection de texte, telle qu’une partie d’un nom de famille. Les éléments renvoyés peuvent être des boîtes aux lettres utilisateur publiques, des groupes de distribution et des contacts. 
  
Notez qu’Exchange enregistre les adresses de messagerie avec des types de routage préfixés, tels que SMTP ou SIP, dans un tableau à valeurs multiples. La méthode **ResolveName** et l’opération **ResolveNames** effectuent une correspondance partielle par rapport à chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « SIP : utilisateur1 ». Si vous ne spécifiez pas de type de routage, la méthode ou l’opération prend par défaut la valeur SMTP, la associe à une propriété d’adresse SMTP principale, et non à la recherche dans le tableau à valeurs multiples. Par exemple, si vous recherchez Utilisateur1 et que vous n’incluez pas le préfixe SIP, vous ne recevrez pas sip :User1@Contoso.com comme résultat, même s’il s’agit d’une boîte aux lettres valide. 
  
Vous ne pouvez spécifier qu’un seul nom ambigu dans une seule demande. Si vous avez une liste de noms ambigus à résoudre, vous devrez parcourir la liste et appeler la méthode ou l’opération pour chaque entrée. Les candidats du dossier de contacts d’un utilisateur auront une valeur d’ID d’élément non null, qui peut ensuite être utilisée dans un appel de méthode [contact. bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) ou une demande d’opération [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) pour extraire des informations supplémentaires. Si le candidat est un groupe de distribution, vous pouvez utiliser la méthode de l’API managée EWS [expandgroup, (itemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) ou l’opération EWS [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) pour obtenir la liste des membres. Si le paramètre _returnContactDetails_ ou l’attribut EWS **ReturnFullContactData** est défini sur true, les entrées Active Directory renvoyées via une méthode **ResolveName** ou **ResolveNames** incluent des propriétés supplémentaires qui décrivent le contact. Le paramètre _returnContactDetails_ ou l’attribut **ReturnFullContactData** n’affecte pas les données renvoyées pour les contacts et les groupes de contacts. 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>Résoudre les noms ambigus à l’aide de l’API managée EWS
<a name="bk_EWSMA"> </a>

Vous pouvez utiliser la méthode [ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) pour rechercher les candidats qui correspondent au nom ambigu que vous transmettez. Vous pouvez utiliser des surcharges de la méthode **ResolveName** pour rechercher des candidats de cinq manières différentes. 
  
**Tableau 1. Méthodes ResolveName surchargées**

|**Méthode**|**Fonctionnement**|
|:-----|:-----|
|[ResolveName (chaîne)](https://msdn.microsoft.com/library/dd635548%28v=exchg.80%29.aspx) <br/> |Recherche les contacts dans le dossier contacts de l’utilisateur et dans la liste d’adresses globale (LAG), dans cet ordre. La variable de chaîne est le nom ambigu que vous tentez de résoudre.  <br/> |
|[ResolveName (String, ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd634595%28v=exchg.80%29.aspx) <br/> |Recherche des contacts dans le dossier de contacts par défaut et/ou dans la liste d’adresses globale (LAG). La valeur de chaîne est le nom ambigu, l’emplacement de recherche spécifie le dossier contacts et/ou la liste d’adresses globale, et la valeur booléenne indique s’il faut renvoyer les informations de contact complètes.  <br/> |
|[ResolveName (String, ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532803%28v=exchg.80%29.aspx) <br/> |Recherche des contacts dans le dossier de contacts par défaut et/ou dans la liste d’adresses globale (LAG). Cette méthode vous permet de définir les propriétés qui sont renvoyées.  <br/> |
|[ResolveName (String, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd636014%28v=exchg.80%29.aspx) <br/> |Recherche des contacts dans les dossiers de contacts spécifiés et/ou dans la liste d’adresses globale (LAG). Vous pouvez utiliser cette méthode pour transmettre une collection de dossiers à rechercher. Cela vous permet de regarder dans des dossiers de contacts autres que le dossier de contacts par défaut.  <br/> |
|[ResolveName (String, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532581%28v=exchg.80%29.aspx) <br/> |Recherche des contacts dans la liste d’adresses globale (LAG) et/ou dans des dossiers de contacts spécifiques. Cette méthode vous permet de définir les propriétés qui sont renvoyées.  <br/> |
   
Commençons par un exemple simple. L’exemple suivant montre comment résoudre la chaîne de texte « Dan » et générer le nom et l’adresse de messagerie de chaque candidat trouvé. Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange. 
  
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

La réponse renvoie un maximum de 100 candidats, bien qu’il puisse y avoir plus de 100 candidats potentiels. Pour déterminer si seuls les 100 premiers candidats d’un plus grand nombre de candidats ont été renvoyés, vérifiez la valeur de [IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) dans l’objet [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) Si la valeur est true, il n’y a pas de candidats possibles ; Si la valeur est false, la méthode renvoie uniquement le premier 100 d’un plus grand nombre de candidats potentiels. 
  
Si vous travaillez dans une grande organisation, il est probable qu’un nom tel que « Dan » renvoie le nombre maximal de candidats de 100. Pour réduire le nombre de candidats renvoyés, limitez l’emplacement de la recherche. L’exemple suivant utilise l’énumération [ResolveNameSearchLocation](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) pour indiquer où Rechercher pour résoudre le nom ambigu. 
  
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

Si vous stockez vos contacts dans un dossier autre que le dossier contacts bien connu, utilisez l’une des méthodes surchargées pour spécifier où rechercher les candidats. L’exemple suivant crée une liste de dossiers pour la méthode **ResolveName** en fonction de l’ID de dossier. Le **FolderId** a été raccourci pour des raisons de lisibilité. 
  
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

Si vous appliquez des filtres et qu’aucun candidat n’est renvoyé, le [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) ne contient aucune entrée. Vous pouvez vérifier cela en examinant la propriété [Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) de la collection. 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>Résoudre des noms ambigus à l’aide d’EWS
<a name="bk_EWSMA"> </a>

Vous pouvez utiliser l’opération EWS [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) pour identifier les candidats possibles pour un nom ambigu. L’élément [UnresolvedEntry](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) contient le nom ambigu à résoudre. L’exemple suivant montre comment résoudre le nom Sadie. Il s’agit également de la requête XML que l’API managée EWS utilise lorsque vous [Utilisez la méthode ResolveName](#bk_EWSMA), à la différence qu’elle utilise un autre nom pour les exemples de sortie valides.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

La réponse renvoie un maximum de 100 candidats, bien qu’il puisse y avoir plus de 100 candidats potentiels pour déterminer si seuls les 100 premiers candidats d’un plus grand nombre de candidats ont été renvoyés, vérifiez la valeur de l’attribut [IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) de l’élément [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) . Si la valeur est true, il n’y a pas de candidats possibles ; Si la valeur est false, l’opération renvoie uniquement le premier 100 d’un plus grand nombre de candidats potentiels. 
  
L’exemple suivant montre la réponse XML lorsqu’un candidat est trouvé. N’oubliez pas que le [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) peut contenir jusqu’à 100 candidats, chacun étant représenté par l’élément de [résolution](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) et ses éléments enfants. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Vous n’allez pas toujours trouver des candidats pour votre nom ambigu. L’exemple suivant montre la réponse XML, comme une erreur, lorsqu’aucun candidat n’est trouvé.
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
- [Développer des groupes de distribution à l’aide d’EWS dans Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

