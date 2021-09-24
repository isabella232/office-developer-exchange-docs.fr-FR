---
title: Acheminer les demandes de contenu de dossier public
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Toutes les demandes d’informations de dossier public qui impliquent le contenu du dossier public doivent être acheminées vers la boîte aux lettres de dossiers publics qui contient le contenu du dossier cible. Pour router les demandes vers cette boîte aux lettres, vous devez définir les en-têtes X-AnchorMailbox et X-PublicFolderMailbox sur des valeurs spécifiques.
ms.openlocfilehash: d5a066a63d9bc3b48c41473545343125538d856b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521101"
---
# <a name="route-public-folder-content-requests"></a>Acheminer les demandes de contenu de dossier public

Toutes les demandes d’informations de dossier public qui impliquent le contenu du dossier public doivent être acheminées vers la boîte aux lettres de dossiers publics qui contient le contenu du dossier cible. Pour router les demandes vers cette boîte aux lettres, vous devez définir les **en-têtes X-AnchorMailbox** et **X-PublicFolderMailbox** sur des valeurs spécifiques. 
  
Le tableau suivant fournit une vue d’ensemble du processus :
  
**Vue d’ensemble des dossiers publics**

|En-tête|De quoi ai-je besoin ?|Comment puis-je l’obtenir ?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |1. [Valeurs X-AnchorMailbox et X-PublicFolderInformation ](how-to-route-public-folder-hierarchy-requests.md) pour la boîte aux lettres de hiérarchie de dossiers publics.<br/><br/>2. GUID de la boîte aux lettres de dossiers publics qui contient le contenu de la boîte aux lettres, qui est envoyé au service de découverte automatique.<br/><br/>  **AutoDiscoverSMTPAddress dans** la réponse de découverte automatique devient la valeur de l’en-tête **X-AnchorMailbox.**  <br/> ![TODO](media/Ex15_PF_PFContent.png)| 1. Utilisez l’exemple de code de cet article, qui implémente [l’API gérée EWS](#bk_determineguidewsma). Vous [pouvez également utiliser EWS](#bk_determineguidews) et convertir vos résultats pour obtenir un GUID.<br/><br/>2. [Effectuer une demande de découverte automatique](#bk_makeautodrequest) à l’aide du GUID et du nom de domaine.<br/><br/>3. Utilisez la valeur de l’élément **AutoDiscoverSMTPAddress** renvoyé dans la réponse de découverte automatique pour remplir la valeur des [en-têtes.](#bk_setheadervalues)  <br/> |
|**X-PublicFolderMailbox** <br/> |Votre travail est terminé, la valeur X-PublicFolderMailbox est identique à la valeur X-AnchorMailbox !  <br/> |Vous l’avez déjà !  <br/> |
   
Une fois que vous avez déterminé les valeurs d’en-tête, incluez-les lorsque vous faites des demandes de contenu [de dossier public.](#bk_setheadervalues)
  
Les étapes de cet article sont spécifiques aux demandes de contenu de dossier public. Pour déterminer si votre demande est une hiérarchie de dossiers publics ou une demande de contenu, voir [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).

<a name="bk_determineguidewsma"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a>Déterminer le GUID de la boîte aux lettres de dossiers publics à l’aide de l’API gérée EWS


Pour déterminer le GUID de la boîte aux lettres de contenu de dossier public, utilisez l’exemple de code suivant, qui permet de : 
  
- Utilise les **en-têtes X-AnchorMailbox** et **X-PublicFolderInformation** que vous avez récupérés en routant les demandes de hiérarchie [de dossiers publics.](how-to-route-public-folder-hierarchy-requests.md)
    
- Appelle la méthode [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) de l’API gérée EWS et inclut une demande pour **la propriété PR_REPLICA_LIST** (0x66980102) 
    
La **PR_REPLICA_LIST** identifie le GUID de boîte aux lettres de la boîte aux lettres de dossiers publics qui contient le contenu du dossier. La **PR_REPLICA_LIST** est un tableau d’bytes, mais est castée en tant que GUID pour ce scénario. Le GUID et le nom de domaine sont concatés pour former l’adresse sur laquelle appeler la découverte automatique. 
  
Cet exemple suppose qu’il s’agit de l’objet ExchangeService pour l’utilisateur de boîte aux lettres et que ce sont les valeurs des `service` [](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) `PFHAnchorHeader` `PFHMailboxHeader` **en-têtes X-AnchorMailbox** et **X-PublicFolderMailbox,** et que le domaine est le nom de domaine utilisé par le client. 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

Si vous avez reçu l’erreur « La demande a échoué. La connexion sous-jacente a été fermée : Nous n’avons pas pu établir de relation d’approbation pour le canal sécurisé SSL/TLS », vous devez ajouter un appel à une méthode de rappel de [validation.](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) Un espace réservé et un commentaire pour cette méthode sont inclus dans l’exemple de code.
  
Si le GUID de boîte aux lettres est le même pour tous les dossiers [](#bk_makeautodrequest) publics sous la racine du dossier public, l’exemple indique l’adresse à utiliser lors de l’appel de la découverte automatique dans la sortie de la console et comme valeur de retour. Si le GUID de boîte aux lettres n’est pas le [](#bk_makeautodrequest) même pour tous les dossiers publics sous la racine du dossier public, vous devez effectuer une demande de découverte automatique sur l’adresse associée au dossier dans votre demande de contenu. 

<a name="bk_determineguidews"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a>Déterminer le GUID de la boîte aux lettres de dossiers publics à l’aide d’EWS

L’exemple de code suivant montre comment récupérer la valeur de la propriété **PR_REPLICA_LIST** (0x66980102) à l’aide de l’opération [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) EWS. Pour l’élément [ExtendedFieldURI,](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) l’attribut **PropertyTag** est définie sur la valeur décimale (26264) de la propriété **PR_REPLICA_LIST** et l’attribut **PropertyType** sur **Binary**.
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous utilisez la méthode **FindFolders** pour déterminer le GUID de la boîte aux lettres de dossiers publics à l’aide de l’API gérée [EWS.](#bk_determineguidewsma)
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **FindFolder** par un message [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) qui inclut la valeur de la **PR_REPLICA_LIST** étendue. Notez que la valeur de la propriété apparaît dans la réponse EWS en tant que format de chaîne d’un tableau d’byte codé en base 64. Certaines valeurs d’en-tête dans la réponse sont raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

Pour utiliser la valeur de **l’PR_REPLICA_LIST** renvoyée dans le code XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==, pour déterminer le GUID de la boîte aux lettres, la valeur doit être convertie en GUID dans un format similaire à celui de la conversion de la valeur dans l’exemple de code api gérée [EWS.](#bk_determineguidewsma) Le GUID est ensuite concaté avec le nom de domaine pour créer une adresse SMTP, qui est incluse dans la demande de [découverte automatique.](#bk_makeautodrequest)
  
## <a name="make-an-autodiscover-request"></a>Effectuer une demande de découverte automatique
<a name="bk_makeautodrequest"> </a>

Utilisez l’adresse renvoyée par la  `GetMailboxGuidAddress` méthode pour appeler la découverte automatique. Nous vous recommandons d’utiliser la Exchange [2013](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) : obtenir des paramètres utilisateur avec l’exemple de code de découverte automatique pour appeler le service de découverte automatique, car elle simplifie le processus de découverte automatique pour vous. Cet exemple de code utilise les arguments de ligne de commande répertoriés dans le tableau suivant pour appeler le service de découverte automatique POX afin de récupérer la valeur [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) associée au GUID de boîte aux lettres. 

  
|**Argument**|**Description**|
|:-----|:-----|
|emailAddress  <br/> |Adresse renvoyée par la méthode `GetMailboxGuidAddress` dans Déterminer le GUID de la boîte aux lettres de [dossiers publics.](#bk_determineguidewsma)  <br/> |
|-skipSOAP  <br/> |Indique que les demandes de découverte automatique POX sont requises.  <br/> |
|-auth authEmailAddress  <br/> |Adresse de messagerie de l’utilisateur de la boîte aux lettres, utilisée pour l’authentification. Vous serez invité à entrer le mot de passe de l’utilisateur de la boîte aux lettres lorsque vous exécuterez l’exemple.  <br/> |
   
Par exemple, les arguments de ligne de commande doivent ressembler à ceci :
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Où `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` se trouve l’adresse renvoyée par la **méthode GetMailboxGuidAddress** et `sonyaf@contoso.com` qui est l’utilisateur de la boîte aux lettres. 
  
Lorsque vous exécutez **la Exchange 2013** : obtenir les paramètres utilisateur avec l’exemple de découverte automatique, la dernière réponse de découverte automatique doit être réussie et inclure tous les paramètres utilisateur associés au GUID de boîte aux lettres. Enregistrez **le paramètre utilisateur AutoDiscoverSMTPAddress** localement, car vous l’utiliserez à l’étape suivante. 
  
Si vous ne souhaitez pas utiliser **Exchange 2013** : obtenir les paramètres utilisateur avec l’exemple de découverte automatique, vous pouvez obtenir le paramètre utilisateur **AutoDiscoverSMTPAddress** en générant une liste de points de terminaison de découverte [automatique,](how-to-generate-a-list-of-autodiscover-endpoints.md)puis en envoyant la demande de découverte automatique POX suivante à chaque URL jusqu’à ce que vous receviez une réponse réussie.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Pour plus d’informations sur le processus de découverte automatique, voir Découverte automatique pour [Exchange](autodiscover-for-exchange.md) [,](how-to-generate-a-list-of-autodiscover-endpoints.md)Générer une liste de points de terminaison de découverte automatique et obtenir les [paramètres](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)utilisateur à partir de Exchange à l’aide de la découverte automatique .
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Définir les valeurs des en-têtes X-AnchorMailbox et X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

En utilisant la valeur de **l’adresse AutoDiscoverSMTPAddress** acquise dans Créer une demande de découverte [automatique,](#bk_makeautodrequest)définissez les valeurs des **en-têtes X-AnchorMailbox** et **X-PublicFolderMailbox** dans votre demande de contenu de dossier public. 
  
Par exemple, pour une adresse AutoDiscoverSMTPAddress de NewPublicFolder@contoso.com, incluez les en-têtes suivants lors des appels aux méthodes ou opérations suivantes.
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

**Appels de dossier public nécessitant les en-têtes X-AncorMailbox et X-PublicFolder**

|**Méthodes d'API managée EWS**|**Opérations EWS**|
|:-----|:-----|
|[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
Pour ajouter ces en-têtes à l’aide de l’API gérée EWS, utilisez la [méthode HttpHeaders.Add.](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

Le code suivant montre une demande [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) avec l’en-tête **X-AnchorMailbox** et **X-PublicFolderMailbox** définie sur les valeurs récupérées dans les exemples de cet article. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Accéder aux dossiers publics avec EWS dans Exchange](public-folder-access-with-ews-in-exchange.md)    
- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)    
- [Générer une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  
