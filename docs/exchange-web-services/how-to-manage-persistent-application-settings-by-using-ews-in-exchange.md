---
title: Gérer les paramètres de l’application permanente à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 90f561f2-e40e-4f5b-b321-f86dbf4a1b71
description: Découvrez comment créer, trouver, obtenir, mettre à jour et supprimer les paramètres de l’application permanente à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: ab5a9cc927bd0a6c4efacce622cc71db1a9b02a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754870"
---
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a><span data-ttu-id="2e552-103">Gérer les paramètres de l’application permanente à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2e552-103">Manage persistent application settings by using EWS in Exchange</span></span>

<span data-ttu-id="2e552-104">Découvrez comment créer, trouver, obtenir, mettre à jour et supprimer les paramètres de l’application permanente à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e552-104">Learn how to create, find, get, update, and delete persistent application settings by using the EWS Managed API or EWS in Exchange.</span></span> 
  
<span data-ttu-id="2e552-105">Objets de configuration utilisateur sont la meilleure option pour stocker les paramètres de configuration de votre application client Exchange, principalement parce qu’ils sont masqués à partir des résultats de recherche dans la plupart des applications clientes.</span><span class="sxs-lookup"><span data-stu-id="2e552-105">User configuration objects are the best option for storing configuration settings for your Exchange client application, primarily because they are hidden from search results in most client applications.</span></span> <span data-ttu-id="2e552-106">Applications clientes masquer généralement ces paramètres, car l’utilisateur final n’a pas besoin de les voir et afin que l’utilisateur ne par inadvertance accéder à ces informations.</span><span class="sxs-lookup"><span data-stu-id="2e552-106">Client applications typically hide these settings because the end user doesn't need to see them, and so that the user doesn't accidentally access this information.</span></span> <span data-ttu-id="2e552-107">Les exemples de code dans cet article montrent vous comment vous pouvez utiliser des objets de configuration utilisateur pour gérer les paramètres persistants, y compris comment créer, trouverez, obteniez, mettre à jour et supprimez des paramètres d’application persistant qui sont stockés dans les objets de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-107">The code examples in this article show you how you can use user configuration objects to manage persistent settings, including how to create, find, get, update, and delete persistent application settings that are stored in user configuration objects.</span></span>

<span data-ttu-id="2e552-108"><a name="createconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-108"></span></span>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="2e552-109">Créer un paramètre d’application à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-109">Create an application setting by using the EWS Managed API</span></span>

<span data-ttu-id="2e552-110">Vous pouvez utiliser la méthode d’API managées [UserConfiguration.Save](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) pour créer un paramètre de configuration personnalisé.</span><span class="sxs-lookup"><span data-stu-id="2e552-110">You can use the [UserConfiguration.Save](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS Managed API method to create a custom configuration setting.</span></span> <span data-ttu-id="2e552-111">Un objet de configuration utilisateur peut contenir le code XML, binaire, un dictionnaire de données ou une combinaison de ces trois types de données.</span><span class="sxs-lookup"><span data-stu-id="2e552-111">A user configuration object can contain XML, binary, a data dictionary, or a combination of those three data types.</span></span> <span data-ttu-id="2e552-112">L’exemple suivant montre comment enregistrer un objet de configuration utilisateur nommé ContosoDraftSettings qui contient des données binaires dans le dossier Brouillons à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="2e552-112">The following example shows how to save a user configuration object named ContosoDraftSettings that contains binary data to your Drafts folder by using the EWS Managed API.</span></span> <span data-ttu-id="2e552-113">Cela peut être utile si vous souhaitez stocker les informations de configuration sur le mode d’affichage des éléments de brouillon dans votre application cliente.</span><span class="sxs-lookup"><span data-stu-id="2e552-113">This might be useful if you want to store configuration information about how draft items are displayed in your client application.</span></span> 
  
```cs
private static void CreateUserConfiguration(ExchangeService service, byte[] binaryData)
{
    // Create the user configuration object.
    UserConfiguration configDrafts = new UserConfiguration(service);
    // Add user configuration data to the BinaryData property.
    configDrafts.BinaryData = binaryData;
    // Name and save the user configuration object on the Drafts folder.
    // This results in a call to EWS.
    configDrafts.Save("ContosoDraftSettings", WellKnownFolderName.Drafts);
}
```

## <a name="create-an-application-setting-by-using-ews"></a><span data-ttu-id="2e552-114">Créer un paramètre d’application à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-114">Create an application setting by using EWS</span></span>
<span data-ttu-id="2e552-115"><a name="bk_createEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-115"></span></span>

<span data-ttu-id="2e552-116">Vous pouvez utiliser l’opération EWS [CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) pour créer un paramètre de configuration personnalisé.</span><span class="sxs-lookup"><span data-stu-id="2e552-116">You can use the [CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS operation to create a custom configuration setting.</span></span> <span data-ttu-id="2e552-117">L’exemple suivant montre la requête XML pour la création d’un objet de configuration utilisateur nommé ContosoDraftSettings.</span><span class="sxs-lookup"><span data-stu-id="2e552-117">The following example shows the request XML for creating a user configuration object named ContosoDraftSettings.</span></span> <span data-ttu-id="2e552-118">La demande essaie d’enregistrer un flux binaire à un objet de configuration utilisateur dans le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="2e552-118">The request attempts to save a binary stream to a user configuration object on the Drafts folder.</span></span> <span data-ttu-id="2e552-119">Il s’agit du même fichier XML qui est généré par l’exemple d’API managées.</span><span class="sxs-lookup"><span data-stu-id="2e552-119">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:CreateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="ContosoDraftSettings">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:BinaryData>iVBORw0KGH5UhKquRSzaeAAAAAElFTkSuQmCC</t:BinaryData>
      </m:UserConfiguration>
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2e552-120">La [réponse XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) est simple et indique si la demande de création a réussi ou si une erreur s’est produite.</span><span class="sxs-lookup"><span data-stu-id="2e552-120">The [response XML](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) is simple and indicates whether the create request was successful or whether an error occurred.</span></span> 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="2e552-121">Rechercher un paramètre d’application à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-121">Find an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="2e552-122"><a name="findconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-122"></span></span>

<span data-ttu-id="2e552-123">Vous pouvez utiliser la méthode d’API managées [Folder.FindItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) avec l’option traversée du contenu associé pour rechercher des objets de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-123">You can use the [Folder.FindItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS Managed API method with the associated traversal option to find user configuration objects.</span></span> <span data-ttu-id="2e552-124">L’exemple de code suivant montre comment rechercher des objets de configuration d’utilisateur stockés dans le dossier Brouillons à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="2e552-124">The following code example shows you how to find user configuration objects stored on the Drafts folder by using the EWS Managed API.</span></span> 
  
```cs
private static void FindAssociated(ExchangeService service)
{
    // This is the ItemClass prefix of user configuration objects that are created by using EWS.
    const string userConfigPrefix = "IPM.Configuration.";
            
    // This is the name of a configuration setting created by using EWS.
    string userConfigName = "TestConfig";
    // Return the first five items. 
    ItemView view = new ItemView(5);
    // Request only the properties that you need. Because all the results will be user configuration 
    // objects, you won't need to request the ItemSchema.IsAssociated property, which identifies 
    // user configuration objects.
    PropertySet props = new PropertySet(BasePropertySet.IdOnly, 
                                        ItemSchema.ItemClass);
    view.PropertySet = props;
            
    // Set the traversal to find user configuration objects. 
    view.Traversal = ItemTraversal.Associated;
    // Send the request to search the Drafts folder for all the user configuration objects 
    // in the folder. You do not have to use a search restriction because you will not return
    // a large number of search results. For this scenario, it is better to sort the results
    // on the client. This method results in a call to EWS.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Drafts, view);
    // Output a list of the item classes for the associated items. 
    foreach (Item item in findResults)
    {
        if (item.ItemClass == userConfigPrefix + userConfigName)
        {
            Console.WriteLine("You found the configuration: " + userConfigPrefix + userConfigName);
        }
    }
}
```

## <a name="find-an-application-setting-by-using-ews"></a><span data-ttu-id="2e552-125">Rechercher un paramètre d’application à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-125">Find an application setting by using EWS</span></span>
<span data-ttu-id="2e552-126"><a name="bk_findEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-126"></span></span>

<span data-ttu-id="2e552-127">Vous pouvez utiliser l’opération EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher des objets de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-127">You can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation to find user configuration objects.</span></span> 
  
<span data-ttu-id="2e552-128">L’exemple suivant montre la requête XML pour la recherche d’objets de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-128">The following example shows the request XML for finding user configuration objects.</span></span> <span data-ttu-id="2e552-129">Il s’agit du même fichier XML qui est généré par l’exemple d’API managées.</span><span class="sxs-lookup"><span data-stu-id="2e552-129">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Associated">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemClass" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="5" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="drafts" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2e552-130">L’exemple suivant montre le XML de la réponse réussie pour la recherche d’objets de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-130">The following example shows the successful response XML for finding user configuration objects.</span></span> <span data-ttu-id="2e552-131">Il s’agit du même fichier XML est traité par l’exemple d’API managées.</span><span class="sxs-lookup"><span data-stu-id="2e552-131">This is the same XML that is processed by the EWS Managed API example.</span></span> <span data-ttu-id="2e552-132">Notez ce qui suit dans cette réponse XML :</span><span class="sxs-lookup"><span data-stu-id="2e552-132">Note the following in this response XML:</span></span> 
  
- <span data-ttu-id="2e552-133">Nous avons réduit les touches identificateur et de modification pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2e552-133">We shortened the identifier and change keys for readability.</span></span>
    
- <span data-ttu-id="2e552-134">Les objets de configuration utilisateur sont renvoyées sous forme de messages.</span><span class="sxs-lookup"><span data-stu-id="2e552-134">The two user configuration objects are returned as messages.</span></span> <span data-ttu-id="2e552-135">Il s’agit, car l’opération **FindItem** retourne tous les éléments qui ne sont pas définies dans le schéma EWS comme éléments de message.</span><span class="sxs-lookup"><span data-stu-id="2e552-135">This is because the **FindItem** operation returns all items that are not defined in the EWS schema as message items.</span></span> 
    
- <span data-ttu-id="2e552-136">Les propriétés [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) pour les objets de configuration utilisateur sont différentes.</span><span class="sxs-lookup"><span data-stu-id="2e552-136">The [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) properties for the two user configuration objects are different.</span></span> <span data-ttu-id="2e552-137">Le premier objet de configuration utilisateur a été créé à l’aide de EWS.</span><span class="sxs-lookup"><span data-stu-id="2e552-137">The first user configuration object was created by using EWS.</span></span> <span data-ttu-id="2e552-138">Le deuxième objet a été créé par une autre API.</span><span class="sxs-lookup"><span data-stu-id="2e552-138">The second object was created by another API.</span></span> 
    
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" 
                        TotalItemsInView="2" 
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
                <t:ItemClass>IPM.Configuration.TestConfig</t:ItemClass>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAkADEzOzFAAA=" ChangeKey="CQAAABQAAABAByOw==" />
                <t:ItemClass>IPM.Microsoft.FolderDesign.NamedView</t:ItemClass>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="2e552-139">Obtenir et mettre à jour les paramètres de l’application à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-139">Get and update application settings by using the EWS Managed API</span></span>
<span data-ttu-id="2e552-140"><a name="getconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-140"></span></span>

<span data-ttu-id="2e552-141">Une fois que vous avez trouvé un objet de configuration utilisateur, vous pouvez utiliser la méthode d’API managées [UserConfiguration.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) pour obtenir l’objet de configuration à partir de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2e552-141">After you find a user configuration object, you can use the [UserConfiguration.Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS Managed API method to get the configuration object from the mailbox.</span></span> <span data-ttu-id="2e552-142">Une fois que vous obtenez l’objet de configuration, vous pouvez utiliser la méthode [UserConfiguration.Update](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="2e552-142">After you get the configuration object, you can use the [UserConfiguration.Update](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) method to update it.</span></span> <span data-ttu-id="2e552-143">L’exemple suivant montre comment obtenir et mettre à jour un objet de configuration utilisateur à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="2e552-143">The following example shows how to get and update a user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void GetAndUpdateUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object named "TestConfig" in the user's mailbox. 
    // Results in a call to EWS. You can also use the Load method to get the latest
    // server version of the user configuration object.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                         "TestConfig",
                                                         WellKnownFolderName.Drafts,
                                                         UserConfigurationProperties.All);
            
    // Display the returned configuration object property values.
    if (usrConfig.XmlData != null)
    {
        Console.WriteLine("XmlData: " + Encoding.UTF8.GetString(usrConfig.XmlData));
    }
    if (usrConfig.BinaryData != null)
    {
        Console.WriteLine("BinaryData: " + Encoding.UTF8.GetString(usrConfig.BinaryData));
    }
    if (usrConfig.Dictionary.Count > 0)
    {
        Console.WriteLine("Contains {0} dictionary entries", usrConfig.Dictionary.Count);
    }
    // Add dictionary property values to the local copy of the object.
    usrConfig.Dictionary.Add("Key5", 1);
    // Updates the server version of the user configuration object 
    // if it has changed on the client. Results in a call to EWS.
    if (usrConfig.IsDirty)
    {
        usrConfig.Update();
    }
}
```

## <a name="get-and-update-application-settings-by-using-ews"></a><span data-ttu-id="2e552-144">Obtenir et mettre à jour les paramètres de l’application à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-144">Get and update application settings by using EWS</span></span>
<span data-ttu-id="2e552-145"><a name="bk_getEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-145"></span></span>

<span data-ttu-id="2e552-146">Vous pouvez utiliser l’opération EWS [GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) pour récupérer l’objet de configuration à partir de la boîte aux lettres et [UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) pour mettre à jour l’objet.</span><span class="sxs-lookup"><span data-stu-id="2e552-146">You can use the [GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS operation to retrieve the configuration object from the mailbox, and the [UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) to update the object.</span></span> <span data-ttu-id="2e552-147">L’exemple suivant montre la requête XML pour obtenir un objet de configuration utilisateur nommé TestConfig.</span><span class="sxs-lookup"><span data-stu-id="2e552-147">The following example shows the request XML for getting a user configuration object named TestConfig.</span></span> <span data-ttu-id="2e552-148">La demande indique que toutes les configurations doivent être renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="2e552-148">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="2e552-149">Il s’agit du même fichier XML qui est généré par l’exemple d’API managées.</span><span class="sxs-lookup"><span data-stu-id="2e552-149">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>All</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2e552-150">L’exemple suivant montre la réponse positive XML pour obtenir des objets de configuration d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-150">The following example shows the successful response XML for getting a user configuration objects.</span></span> <span data-ttu-id="2e552-151">La réponse contient un dictionnaire de données.</span><span class="sxs-lookup"><span data-stu-id="2e552-151">The response contains a data dictionary.</span></span> <span data-ttu-id="2e552-152">Il s’agit du même fichier XML est traité par l’exemple d’API managées.</span><span class="sxs-lookup"><span data-stu-id="2e552-152">This is the same XML that is processed by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts" />
            </t:UserConfigurationName>
            <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>Key1</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>Integer32</t:Type>
                  <t:Value>1</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="2e552-153">L’exemple suivant montre la requête XML de mise à jour d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-153">The following example shows the request XML for updating a user configuration object.</span></span> <span data-ttu-id="2e552-154">La demande indique que toutes les configurations doivent être renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="2e552-154">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="2e552-155">Il s’agit du même fichier XML qui est généré par l’exemple d’API managées qui appelle la méthode **UserConfiguration.Update** .</span><span class="sxs-lookup"><span data-stu-id="2e552-155">This is the same XML that is generated by the EWS Managed API example that calls the **UserConfiguration.Update** method.</span></span> <span data-ttu-id="2e552-156">Vous pouvez voir que la mise à jour XML contienne les entrées du dictionnaire existant et celui qui a été ajouté avant la mise à jour supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="2e552-156">You can see that the update XML contains the existing dictionary entries and the additional one that was added before the update.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:UpdateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key1</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>555-555-1111</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key5</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>
    </m:UpdateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2e552-157">La [réponse XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) est simple et indique si la mise à jour a réussi ou si une erreur s’est produite.</span><span class="sxs-lookup"><span data-stu-id="2e552-157">The [response XML](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) is simple and indicates whether the update was successful or whether an error occurred.</span></span> 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="2e552-158">Supprimer un paramètre d’application à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-158">Delete an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="2e552-159"><a name="deleteconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-159"></span></span>

<span data-ttu-id="2e552-160">Vous pouvez utiliser la méthode d’API managées [UserConfiguration.Delete](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) pour supprimer les objets de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-160">You can use the [UserConfiguration.Delete](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API method to delete user configuration objects.</span></span> <span data-ttu-id="2e552-161">L’exemple de code suivant montre comment supprimer l’objet de configuration utilisateur ContosoDraftSettings à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="2e552-161">The following code example shows you how to delete the ContosoDraftSettings user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void DeleteUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object. Results in a call to EWS.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                        "ContosoDraftSettings",
                                                        WellKnownFolderName.Drafts,
                                                        UserConfigurationProperties.Id);
    // Deletes the user configuration object.
    // Results in a call to EWS.
    usrConfig.Delete();
}
```

## <a name="delete-an-application-setting-by-using-ews"></a><span data-ttu-id="2e552-162">Supprimer un paramètre d’application à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="2e552-162">Delete an application setting by using EWS</span></span>
<span data-ttu-id="2e552-163"><a name="bk_deleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2e552-163"></span></span>

<span data-ttu-id="2e552-164">Vous pouvez utiliser l’opération EWS [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) pour supprimer les objets de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2e552-164">You can use the [DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS operation to delete user configuration objects.</span></span> 
  
<span data-ttu-id="2e552-165">L’exemple suivant montre la requête XML pour supprimer un objet de configuration utilisateur nommé ContosoDraftSettings qui a été appliqué dans le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="2e552-165">The following example shows the request XML for deleting a user configuration object named ContosoDraftSettings that was applied to the Drafts folder.</span></span> <span data-ttu-id="2e552-166">Il s’agit du même fichier XML qui est généré par l’exemple d’API managées.</span><span class="sxs-lookup"><span data-stu-id="2e552-166">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:DeleteUserConfiguration>
      <m:UserConfigurationName Name="ContosoDraftSettings">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
    </m:DeleteUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2e552-167">La [réponse XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) est simple et indique si la demande de suppression a réussi ou si une erreur s’est produite.</span><span class="sxs-lookup"><span data-stu-id="2e552-167">The [response XML](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) is simple and indicates whether the delete request was a success or whether an error occurred.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2e552-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2e552-168">See also</span></span>

- [<span data-ttu-id="2e552-169">Paramètres de l'application persistant dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2e552-169">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
- [<span data-ttu-id="2e552-170">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="2e552-170">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="2e552-171">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="2e552-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

