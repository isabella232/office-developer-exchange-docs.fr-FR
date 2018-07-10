---
title: Travailler avec des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: e70ac499da57faa60b4bcb6082648b23d1a7e791
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754966"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a><span data-ttu-id="60b65-103">Travailler avec des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="60b65-103">Work with Exchange mailbox items by using EWS in Exchange</span></span>

<span data-ttu-id="60b65-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="60b65-104">Learn how to create, get, update, and delete items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="60b65-105">Vous pouvez utiliser les API managées EWS pour travailler avec des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="60b65-105">You can use the EWS Managed API or EWS to work with items in a mailbox.</span></span> <span data-ttu-id="60b65-106">Vous pouvez utiliser les éléments génériques : objets d’API managées, [élément](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) ou types EWS [élément](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) — pour effectuer certaines opérations (obtention d’un élément ou suppression d’un élément à l’aide identificateur de l’élément) ; Toutefois, la plupart du temps, que vous devrez utiliser [fortement typées élément](folders-and-items-in-ews-in-exchange.md#bk_item) pour effectuer une opération get ou mettre à jour opération car vous aurez besoin d’accéder aux propriétés qui sont spécifiques à l’élément fortement typé.</span><span class="sxs-lookup"><span data-stu-id="60b65-106">You can use generic items — EWS Managed API [Item](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) objects or EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) types — to perform some operations (getting an item or deleting an item by using the item's identifier); however, most of the time you'll have to use a [strongly typed item](folders-and-items-in-ews-in-exchange.md#bk_item) to perform a get or update operation because you'll need access to the properties that are specific to the strongly typed item.</span></span> 

<span data-ttu-id="60b65-107">Par exemple, vous ne pouvez pas utiliser un élément générique pour récupérer un élément qui contient un début et date de fin, vous avez besoin d’un objet d’API managées [rendez-vous](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou un type EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) à le faire.</span><span class="sxs-lookup"><span data-stu-id="60b65-107">For example, you can't use a generic item to retrieve an item that contains a start and end date - you need an EWS Managed API [Appointment](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object or an EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) type to do that.</span></span> <span data-ttu-id="60b65-108">Et si vous utilisez l’API managée EWS, vous devrez toujours créer des éléments fortement typées, car la classe de **l’élément** générique ne dispose pas d’un constructeur.</span><span class="sxs-lookup"><span data-stu-id="60b65-108">And if you're using the EWS Managed API, you always have to create strongly typed items, because the generic **Item** class does not have a constructor.</span></span> <span data-ttu-id="60b65-109">Si vous travaillez avec un élément qui n’est pas fortement typé, vous pouvez toujours utiliser la classe de **l’élément de** base pour travailler avec l’élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-109">If you're working with an item that is not strongly typed, you can always use the base **Item** class to work with the item.</span></span> 
  
<span data-ttu-id="60b65-110">**Le tableau 1. Méthodes d’API managées et opérations EWS pour l’utilisation d’éléments**</span><span class="sxs-lookup"><span data-stu-id="60b65-110">**Table 1. EWS Managed API methods and EWS operations for working with items**</span></span>

|<span data-ttu-id="60b65-111">**Pour...**</span><span class="sxs-lookup"><span data-stu-id="60b65-111">**In order to…**</span></span>|<span data-ttu-id="60b65-112">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="60b65-112">**EWS Managed API method**</span></span>|<span data-ttu-id="60b65-113">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="60b65-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="60b65-114">Créer un élément générique</span><span class="sxs-lookup"><span data-stu-id="60b65-114">Create a generic item</span></span>  <br/> |<span data-ttu-id="60b65-p103">Aucune. Vous pouvez uniquement créer des types d’élément spécifiques à l’aide de l’API managée EWS. Vous ne pouvez pas créer d’éléments génériques.</span><span class="sxs-lookup"><span data-stu-id="60b65-p103">None. You can only create specific item types by using the EWS Managed API; you cannot create generic items.</span></span>  <br/> |[<span data-ttu-id="60b65-117">CreateItem</span><span class="sxs-lookup"><span data-stu-id="60b65-117">CreateItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="60b65-118">Obtenir un élément</span><span class="sxs-lookup"><span data-stu-id="60b65-118">Get an item</span></span>  <br/> |[<span data-ttu-id="60b65-119">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="60b65-119">Item.Bind</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="60b65-120">GetItem</span><span class="sxs-lookup"><span data-stu-id="60b65-120">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="60b65-121">Mettre à jour un élément</span><span class="sxs-lookup"><span data-stu-id="60b65-121">Update an item</span></span>  <br/> |[<span data-ttu-id="60b65-122">Item.Update</span><span class="sxs-lookup"><span data-stu-id="60b65-122">Item.Update</span></span>](http://msdn.microsoft.com/fr-fr/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="60b65-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="60b65-123">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="60b65-124">Supprimer un élément</span><span class="sxs-lookup"><span data-stu-id="60b65-124">Delete an item</span></span>  <br/> |[<span data-ttu-id="60b65-125">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="60b65-125">Item.Delete</span></span>](http://msdn.microsoft.com/fr-fr/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="60b65-126">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="60b65-126">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="60b65-127">Dans cet article, vous apprendrez quand vous pouvez utiliser la classe de base générique et lorsque vous devez utiliser un élément fortement typé pour effectuer votre tâche.</span><span class="sxs-lookup"><span data-stu-id="60b65-127">In this article, you'll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task.</span></span> <span data-ttu-id="60b65-128">Les exemples de code montrent comment utiliser la classe de base et que faire lorsque vous ne pouvez pas utiliser la classe de base ou qu’il ne selon vos besoins.</span><span class="sxs-lookup"><span data-stu-id="60b65-128">The code examples will show you how to use the base class, and what to do when you can't use the base class or it doesn't fit your needs.</span></span>
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="60b65-129">Création d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-129">Create an item by using the EWS Managed API</span></span>
<span data-ttu-id="60b65-130"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-130"></span></span>

<span data-ttu-id="60b65-131">L’API managée EWS ne dispose pas d’un constructeur publiquement disponible pour la classe [d’élément](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , vous devez utiliser le constructeur pour le type d’élément spécifique que vous souhaitez créer afin de créer un élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-131">The EWS Managed API does not have a publicly available constructor for the [Item](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) class, so you must use the constructor for the specific item type you want to create in order to create an item.</span></span> <span data-ttu-id="60b65-132">Par exemple, utilisez le [constructeur de classe EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) pour créer un nouveau message électronique et [contactez le constructeur de classe](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) pour créer un nouveau contact.</span><span class="sxs-lookup"><span data-stu-id="60b65-132">For example, use the [EmailMessage class constructor](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create a new email message, and the [Contact class constructor](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) to create a new contact.</span></span> <span data-ttu-id="60b65-133">De même, le serveur ne retourne jamais les objets **élément** génériques dans les réponses ; tous les éléments génériques sont renvoyés en tant qu’objets **EmailMessage** .</span><span class="sxs-lookup"><span data-stu-id="60b65-133">Likewise, the server never returns generic **Item** objects in responses; all generic items are returned as **EmailMessage** objects.</span></span> 
  
<span data-ttu-id="60b65-p106">Lorsque vous connaissez le type d’élément à créer, vous pouvez effectuer la tâche en quelques étapes seulement. Les étapes sont similaires pour tous les types d’éléments :</span><span class="sxs-lookup"><span data-stu-id="60b65-p106">When you know the type of item to create, you can complete the task in just a few steps. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="60b65-136">Initialiser une nouvelle instance d’une des classes [d’élément](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) avec l’objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) en tant que paramètre.</span><span class="sxs-lookup"><span data-stu-id="60b65-136">Initialize a new instance of one of the [Item](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) classes with the [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object as a parameter.</span></span> 
    
2. <span data-ttu-id="60b65-p107">Définissez des propriétés sur l’élément. Les schémas sont différents pour chaque type d’élément, c’est pourquoi plusieurs propriétés sont disponibles pour ces derniers.</span><span class="sxs-lookup"><span data-stu-id="60b65-p107">Set properties on the item. The schemas are different for each item type, so different properties are available for different items.</span></span>
    
3. <span data-ttu-id="60b65-139">Enregistrez l’élément, ou enregistrez et envoyez l’élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-139">Save the item, or save and send the item.</span></span>
    
<span data-ttu-id="60b65-140">Par exemple, vous créez un objet [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) , définir des propriétés [ToRecipients](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) , le [corps](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)et [l’objet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx)et l’envoyer puis en utilisant la méthode [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-140">For example, you can create an [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object, set the [Subject](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx), and [ToRecipients](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) properties, and then send it by using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

<span data-ttu-id="60b65-141">Pour savoir comment créer une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [créer des rendez-vous et réunions à l’aide EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-141">To learn how to create a meeting or appointment item by using the EWS Managed API, see [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="create-an-item-by-using-ews"></a><span data-ttu-id="60b65-142">Création d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-142">Create an item by using EWS</span></span>
<span data-ttu-id="60b65-143"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-143"></span></span>

<span data-ttu-id="60b65-p108">Vous pouvez créer un élément générique ou un élément fortement typé à l’aide d’EWS. Les étapes sont similaires pour tous les types d’éléments :</span><span class="sxs-lookup"><span data-stu-id="60b65-p108">You can create a generic item or a strongly typed item by using EWS. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="60b65-146">Utilisez l’opération [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) pour créer un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="60b65-146">Use the [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to create an item in the Exchange store.</span></span> 
    
2. <span data-ttu-id="60b65-147">Utilisez l’élément [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) pour contenir un ou plusieurs éléments à créer.</span><span class="sxs-lookup"><span data-stu-id="60b65-147">Use the [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) element to contain one or more items to create.</span></span> 
    
3. <span data-ttu-id="60b65-148">Définissez des propriétés sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-148">Set properties on the item.</span></span>
    
<span data-ttu-id="60b65-149">Par exemple, vous pouvez créer un message électronique et l’envoyer en utilisant le code dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="60b65-149">For example, you can create an email message and send it by using the code in the following example.</span></span> <span data-ttu-id="60b65-150">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode [SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-150">This is also the XML request that the EWS Managed API sends when you call the [SendAndSaveCopy](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="60b65-151">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès et l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de la nouvelle message créé.</span><span class="sxs-lookup"><span data-stu-id="60b65-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="60b65-152">Pour savoir comment créer une réunion ou un élément de rendez-vous à l’aide de EWS, voir [créer des rendez-vous et réunions à l’aide EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-152">To learn how to create a meeting or appointment item by using EWS, see [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="60b65-153">Obtention d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-153">Get an item by using the EWS Managed API</span></span>
<span data-ttu-id="60b65-154"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-154"></span></span>

<span data-ttu-id="60b65-155">Pour utiliser l’API managée EWS pour obtenir un élément si vous connaissez [Item.Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à récupérer, vous appelez simplement une des méthodes [liaison](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) sur l’élément, et l’élément est récupéré.</span><span class="sxs-lookup"><span data-stu-id="60b65-155">To use the EWS Managed API to get an item if you know the [Item.Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to retrieve, you simply call one of the [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) methods on the item, and the item is retrieved.</span></span> <span data-ttu-id="60b65-156">Meilleure pratique, nous vous recommandons de limiter les propriétés renvoyées uniquement à ceux qui sont requis.</span><span class="sxs-lookup"><span data-stu-id="60b65-156">As a best practice, we recommend that you limit the properties returned to only those that are required.</span></span> <span data-ttu-id="60b65-157">Cet exemple renvoie la propriété **Id** d’élément et la propriété **Subject** .</span><span class="sxs-lookup"><span data-stu-id="60b65-157">This example returns the item **Id** property and the **Subject** property.</span></span> 
  
<span data-ttu-id="60b65-158">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="60b65-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="60b65-159">variable local *itemId* est l' [Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="60b65-159">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

<span data-ttu-id="60b65-160">Si vous recherchez un élément qui répond aux critères spécifiques, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="60b65-160">If you're searching for an item that meets specific criteria, do the following:</span></span>
  
1. <span data-ttu-id="60b65-161">Établissez une liaison vers le dossier qui contient les éléments à obtenir.</span><span class="sxs-lookup"><span data-stu-id="60b65-161">Bind to the folder that contains the items to get.</span></span>
    
2. <span data-ttu-id="60b65-162">Instanciez un [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) ou un [PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour filtrer les éléments à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="60b65-162">Instantiate a [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) or a [PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to filter the items to return.</span></span> 
    
3. <span data-ttu-id="60b65-163">Instancier un objet [CalendarView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) ou de [l’annonceAfficher le](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) pour spécifier le nombre d’éléments à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="60b65-163">Instantiate an [ItemView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object to specify the number of items to return.</span></span> 
    
4. <span data-ttu-id="60b65-164">Appelez la méthode [ExchangeService.FindItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [ExchangeService.FindAppointments](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-164">Call the [ExchangeService.FindItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [ExchangeService.FindAppointments](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="60b65-165">Par exemple, si vous souhaitez récupérer des messages électroniques non lus dans la boîte de réception, utilisez le code dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="60b65-165">For example, if you want to retrieve unread email messages in the Inbox, use the code in the following example.</span></span> <span data-ttu-id="60b65-166">Cet exemple utilise un **SearchFilterCollection** pour limiter les résultats de la méthode **FindItems** aux messages non lus et limite **l’annonceAfficher le** pour limiter les résultats à un élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-166">This example uses a **SearchFilterCollection** to limit the results of the **FindItems** method to unread messages, and limits the **ItemView** to limit results to one item.</span></span> <span data-ttu-id="60b65-167">Ce code fonctionne uniquement sur les objets [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) car la valeur [EmailMessageSchema.IsRead](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) fait partie de la **SearchFilter**.</span><span class="sxs-lookup"><span data-stu-id="60b65-167">This particular code only works on [EmailMessage](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects because the [EmailMessageSchema.IsRead](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) value is part of the **SearchFilter**.</span></span> 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

<span data-ttu-id="60b65-168">Sinon, vous pouvez utiliser un [PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour limiter les résultats de la recherche, comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="60b65-168">Alternatively, you can use a [PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) to limit the results of the search as shown in the following code example.</span></span> <span data-ttu-id="60b65-169">Cet exemple utilise la méthode [FindAppointments](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) pour récupérer jusqu'à cinq rendez-vous qui se produisent dans les 30 jours.</span><span class="sxs-lookup"><span data-stu-id="60b65-169">This example uses the [FindAppointments](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve up to five appointments that occur in the next 30 days.</span></span> <span data-ttu-id="60b65-170">Ce code bien sûr fonctionne uniquement sur les éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="60b65-170">This code of course only works on calendar items.</span></span> 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

<span data-ttu-id="60b65-171">Notez que cette propriété renvoie les informations du serveur dans la réponse de la méthode **lier** est différente de celle que le serveur renvoie une réponse de méthode **FindItem** ou **FindAppointment** les informations.</span><span class="sxs-lookup"><span data-stu-id="60b65-171">Note that the information the server returns in the **Bind** method response is different than the information that the server returns for a **FindItem** or **FindAppointment** method response.</span></span> <span data-ttu-id="60b65-172">La méthode **Bind** peut renvoyer toutes les propriétés schématisées, tandis que les méthodes **FindItem** et **FindAppointment** ne renvoient pas toutes les propriétés schématisées.</span><span class="sxs-lookup"><span data-stu-id="60b65-172">The **Bind** method can return all the schematized properties, whereas the **FindItem** and **FindAppointment** methods do not return all the schematized properties.</span></span> <span data-ttu-id="60b65-173">Si vous avez besoin d’un accès complet à l’élément, vous devez donc d’utiliser la méthode de **liaison** .</span><span class="sxs-lookup"><span data-stu-id="60b65-173">So if you need full access to the item, you'll have to use the **Bind** method.</span></span> <span data-ttu-id="60b65-174">Si vous n’avez pas l’élément **Id** de l’élément vous souhaitez récupérer, utiliser les méthodes **FindItem** ou **FindAppointment** pour récupérer l’Id, puis utilisez la méthode **Bind** pour récupérer les propriétés dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="60b65-174">If you don't have the item **Id** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** methods to retrieve the Id, and then use the **Bind** method to retrieve the properties you need.</span></span> 
  
<span data-ttu-id="60b65-175">Pour savoir comment obtenir une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-175">To learn how to get a meeting or appointment item by using the EWS Managed API, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="get-an-item-by-using-ews"></a><span data-ttu-id="60b65-176">Obtention d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-176">Get an item by using EWS</span></span>
<span data-ttu-id="60b65-177"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-177"></span></span>

<span data-ttu-id="60b65-178">Si vous connaissez l' [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de l’élément à récupérer, vous pouvez obtenir l’élément à l’aide de l’opération [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-178">If you know the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the item to retrieve, you can get the item by using the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="60b65-179">L’exemple suivant montre la demande XML pour obtenir l' [objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) d’un élément avec un **ID d’élément**spécifique.</span><span class="sxs-lookup"><span data-stu-id="60b65-179">The following example shows the XML request to get the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of an item with a specific **ItemId**.</span></span> <span data-ttu-id="60b65-180">C’est également la demande XML qui envoie de l’API managée EWS lors de l’appel de la méthode [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) sur un **ID d’élément**.</span><span class="sxs-lookup"><span data-stu-id="60b65-180">This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method on an **ItemId**.</span></span> <span data-ttu-id="60b65-181">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="60b65-181">The values of some attributes and elements have been shortened for readability.</span></span>
  
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
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre la réponse XML que le serveur renvoie une fois qu’il traite l’opération **GetItem** . La réponse indique que l’élément a été récupéré correctement. <span data-ttu-id="60b65-184">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="60b65-184">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="60b65-185">Si vous ne connaissez pas l' **ID d’élément** de l’élément que vous souhaitez récupérer, vous pouvez utiliser l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher l’élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-185">If you do not know the **ItemId** of the item you want to retrieve, you can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find the item.</span></span> <span data-ttu-id="60b65-186">Pour pouvoir utiliser l’opération **FindItem** , vous devez d’abord identifier le dossier dans lequel vous effectuez une recherche.</span><span class="sxs-lookup"><span data-stu-id="60b65-186">In order to use the **FindItem** operation, you must first identify the folder that you're searching.</span></span> <span data-ttu-id="60b65-187">Vous pouvez identifier le dossier à l’aide de son **DistinguinguishedFolderName** ou à l’aide de l' [ID FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="60b65-187">You can identify the folder by using its **DistinguinguishedFolderName** or by using the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span></span> <span data-ttu-id="60b65-188">Vous pouvez utiliser les opérations [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) ou de [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) pour obtenir l' **ID FolderId** dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="60b65-188">You can use either the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) or [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operations to get the **FolderId** you need.</span></span> <span data-ttu-id="60b65-189">Ensuite, utilisez l’opération **FindItem** pour rechercher ce dossier pour les résultats qui correspondent au filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="60b65-189">Then use the **FindItem** operation to search that folder for results that match the search filter.</span></span> <span data-ttu-id="60b65-190">Contrairement à l’API managée EWS, EWS ne fournit pas une opération de recherche distincte pour les rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="60b65-190">Unlike the EWS Managed API, EWS does not provide a separate find operation for appointments.</span></span> <span data-ttu-id="60b65-191">L’opération **FindItem** récupère les éléments de tous les types.</span><span class="sxs-lookup"><span data-stu-id="60b65-191">The **FindItem** operation retrieves items of all types.</span></span> 
  
<span data-ttu-id="60b65-192">L’exemple suivant montre la requête d’opération XML **FindItem** qui est envoyée au serveur pour rechercher les rendez-vous dans le dossier de calendrier qui se produisent dans les 30 jours.</span><span class="sxs-lookup"><span data-stu-id="60b65-192">The following example shows the XML **FindItem** operation request that is sent to the server to find appointments in the Calendar folder that occur in the next 30 days.</span></span> <span data-ttu-id="60b65-193">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="60b65-193">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="60b65-194">Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) qui inclut la valeur de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que l’opération s’est terminée correctement.</span><span class="sxs-lookup"><span data-stu-id="60b65-194">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the operation completed successfully.</span></span> <span data-ttu-id="60b65-195">Si les éléments de calendrier répondent aux critères de filtrage, ils sont inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="60b65-195">If any calendar items meet the filtering criteria, they are included in the response.</span></span>
  
<span data-ttu-id="60b65-196">Notez que cette propriété renvoie les informations du serveur dans la réponse d’opération **GetItem** est différent de celui les informations sur que le serveur renvoie dans un **FindItem** ou une réponse d’opération **FindAppointment** .</span><span class="sxs-lookup"><span data-stu-id="60b65-196">Note that the information the server returns in the **GetItem** operation response is different than the information the server returns in a **FindItem** or **FindAppointment** operation response.</span></span> <span data-ttu-id="60b65-197">L’opération **GetItem** peut renvoyer toutes les propriétés schématisées, tandis que les opérations **FindItem** et **FindAppointment** ne renvoient pas toutes les propriétés schématisées.</span><span class="sxs-lookup"><span data-stu-id="60b65-197">The **GetItem** operation can return all the schematized properties, whereas the **FindItem** and **FindAppointment** operations do not return all the schematized properties.</span></span> <span data-ttu-id="60b65-198">Si vous avez besoin d’un accès complet à l’élément, vous devez donc utiliser l’opération **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="60b65-198">So if you need full access to the item, you'll have to use the **GetItem** operation.</span></span> <span data-ttu-id="60b65-199">Si vous n’avez pas l' **ID d’élément** de l’élément vous souhaitez récupérer, les opérations **FindItem** ou **FindAppointment** permet de récupérer l' **ID d’élément**et utiliser l’opération **GetItem** pour récupérer les éléments dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="60b65-199">If you don't have the **ItemId** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** operations to retrieve the **ItemId**, and then use the **GetItem** operation to retrieve the elements you need.</span></span> 
  
<span data-ttu-id="60b65-200">Pour savoir comment obtenir une réunion ou un élément de rendez-vous à l’aide de EWS, voir [obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-200">To learn how to get a meeting or appointment item by using EWS, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="60b65-201">Mise à jour d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-201">Update an item by using the EWS Managed API</span></span>
<span data-ttu-id="60b65-202"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-202"></span></span>

<span data-ttu-id="60b65-203">Les étapes pour mettre à jour un élément à l’aide de l’API managée EWS sont similaires pour tous les types d’éléments ; Toutefois, les propriétés d’élément sont différentes pour chaque type d’élément et la méthode de [mise à jour](http://msdn.microsoft.com/fr-fr/library/office/dd635915%28v=exchg.80%29.aspx) possède de nombreuses méthodes surchargées à sélectionner.</span><span class="sxs-lookup"><span data-stu-id="60b65-203">The steps to update an item by using the EWS Managed API are similar for all item types; however, the item properties are different for each item type, and the [Update](http://msdn.microsoft.com/fr-fr/library/office/dd635915%28v=exchg.80%29.aspx) method has many overloaded methods to choose from.</span></span> <span data-ttu-id="60b65-204">Pour mettre à jour un élément :</span><span class="sxs-lookup"><span data-stu-id="60b65-204">To update an item:</span></span> 
  
1. <span data-ttu-id="60b65-205">Utilisez la méthode [lier](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour obtenir la dernière version de l’élément, sauf si vous disposez déjà d’elle.</span><span class="sxs-lookup"><span data-stu-id="60b65-205">Use the [Bind](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get the latest version of the item, unless you already have it.</span></span> <span data-ttu-id="60b65-206">Pour mettre à jour les propriétés spécifiques à un élément fortement typé, vous devrez lier à ce type d’élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-206">To update properties specific to a strongly typed item, you'll have to bind to that item type.</span></span> <span data-ttu-id="60b65-207">Pour mettre à jour les propriétés disponibles sur le type d’élément générique, vous pouvez lier à l’objet [d’élément](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-207">To update properties available on the generic item type, you can bind to the [Item](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> 
    
2. <span data-ttu-id="60b65-208">Mettez à jour les propriétés sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-208">Update the properties on the item.</span></span>
    
3. <span data-ttu-id="60b65-209">Appelez la méthode de **mise à jour** .</span><span class="sxs-lookup"><span data-stu-id="60b65-209">Call the **Update** method.</span></span> 
    
<span data-ttu-id="60b65-210">Par exemple, vous pouvez mettre à jour l’objet d’un message électronique à l’aide du type d’élément générique, comme illustré dans le code de l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="60b65-210">For example, you can update the subject of an email by using the generic item type, as shown in the code in the following example.</span></span>
  
<span data-ttu-id="60b65-211">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="60b65-211">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="60b65-212">variable local *itemId* est l' [Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="60b65-212">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

<span data-ttu-id="60b65-213">Pour savoir comment mettre à jour une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-213">To learn how to update a meeting or appointment item by using the EWS Managed API, see [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-ews"></a><span data-ttu-id="60b65-214">Mise à jour d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-214">Update an item by using EWS</span></span>
<span data-ttu-id="60b65-215"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-215"></span></span>

<span data-ttu-id="60b65-216">Pour mettre à jour un élément à l’aide d’EWS, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="60b65-216">To update an item by using EWS, do the following:</span></span>
  
1. <span data-ttu-id="60b65-217">Utiliser l’opération de [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir la dernière version de l’élément, sauf si vous disposez déjà d’elle.</span><span class="sxs-lookup"><span data-stu-id="60b65-217">Use the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> 
    
2. <span data-ttu-id="60b65-218">L’opération [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) permet de spécifier les champs pour mettre à jour et attribuer de nouvelles valeurs à ces champs.</span><span class="sxs-lookup"><span data-stu-id="60b65-218">Use the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to specify fields to update and assign new values to those fields.</span></span> 
    
<span data-ttu-id="60b65-219">L’exemple suivant montre la requête d’opération XML **UpdateItem** qui est envoyée au serveur pour mettre à jour la valeur de [l’objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) du message électronique.</span><span class="sxs-lookup"><span data-stu-id="60b65-219">The following example shows the XML **UpdateItem** operation request that is sent to the server to update the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) value of the email message.</span></span> <span data-ttu-id="60b65-220">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="60b65-220">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="60b65-221">Le serveur répond à la demande **UpdateItem** avec un message [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que la mise à jour de l’élément a réussi.</span><span class="sxs-lookup"><span data-stu-id="60b65-221">The server responds to the **UpdateItem** request with a [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item update was successful.</span></span>
  
<span data-ttu-id="60b65-222">Pour savoir comment mettre à jour une réunion ou un élément de rendez-vous à l’aide de EWS, voir [mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-222">To learn how to update a meeting or appointment item by using EWS, see [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="60b65-223">Suppression d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-223">Delete an item by using the EWS Managed API</span></span>
<span data-ttu-id="60b65-224"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-224"></span></span>

<span data-ttu-id="60b65-225">Vous pouvez supprimer des éléments en les déplaçant vers le dossier éléments supprimés ou à la benne.</span><span class="sxs-lookup"><span data-stu-id="60b65-225">You can delete items by moving them to the Deleted Items folder or to the dumpster.</span></span> <span data-ttu-id="60b65-226">Si vous connaissez l' [ItemId](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à supprimer, vous devez seulement appeler la méthode [Delete](http://msdn.microsoft.com/fr-fr/library/office/dd635072%28v=exchg.80%29.aspx) sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="60b65-226">If you know the [ItemId](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to delete, just call the [Delete](http://msdn.microsoft.com/fr-fr/library/office/dd635072%28v=exchg.80%29.aspx) method on the item.</span></span> 
  
<span data-ttu-id="60b65-227">Si vous devez rechercher l’élément avant de le supprimer, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="60b65-227">If you need to find the item before deleting it, do the following:</span></span>
  
1. <span data-ttu-id="60b65-228">Appelez la méthode [FindItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [FindAppointments](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) pour trouver l’élément à supprimer.</span><span class="sxs-lookup"><span data-stu-id="60b65-228">Call the [FindItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [FindAppointments](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to find the item to delete.</span></span> 
    
1. <span data-ttu-id="60b65-229">Instancier un [PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) et limitez aux propriétés à retourner ou utiliser un [SearchFilterCollection](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) pour rechercher des éléments spécifiques.</span><span class="sxs-lookup"><span data-stu-id="60b65-229">Instantiate a [PropertySet](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) and limit it to the properties to return, or use a [SearchFilterCollection](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) to find specific items.</span></span> 
    
2. <span data-ttu-id="60b65-230">Instanciez un [annonceAfficher](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) l’ou [CalendarView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) pour spécifier le nombre d’éléments à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="60b65-230">Instantiate an [ItemView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) to specify the number of items to return.</span></span> 
    
2. <span data-ttu-id="60b65-231">Appelez la méthode [Delete](http://msdn.microsoft.com/fr-fr/library/office/dd635072%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-231">Call the [Delete](http://msdn.microsoft.com/fr-fr/library/office/dd635072%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="60b65-232">Par exemple, le code suivant indique comment déplacer un message électronique vers le dossier Éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="60b65-232">For example, the following code shows how to move an email message to the Deleted Items folder.</span></span>
  
<span data-ttu-id="60b65-233">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="60b65-233">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="60b65-234">variable local *itemId* est l' [Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="60b65-234">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

<span data-ttu-id="60b65-235">Pour plus d’informations sur la suppression d’éléments, voir [suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-235">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="60b65-236">Pour savoir comment supprimer une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-236">To learn how to delete a meeting or appointment item by using the EWS Managed API, see [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-ews"></a><span data-ttu-id="60b65-237">Suppression d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="60b65-237">Delete an item by using EWS</span></span>
<span data-ttu-id="60b65-238"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-238"></span></span>

<span data-ttu-id="60b65-239">Vous pouvez supprimer un élément à l’aide de l’opération [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-239">You can delete an item by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="60b65-p128">L’exemple suivant présente la demande XML qui est envoyée au serveur pour déplacer le message vers le dossier Éléments supprimés. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="60b65-p128">The following example shows the XML request that is sent to the server to move the email message to the Deleted Items folder. The values of some attributes and elements have been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="60b65-242">Le serveur répond à la demande **DeleteItem** avec un message [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que la suppression de l’élément a réussi.</span><span class="sxs-lookup"><span data-stu-id="60b65-242">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/fr-fr/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span>
  
<span data-ttu-id="60b65-243">Pour plus d’informations sur la suppression d’éléments, voir [suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-243">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="60b65-244">Pour savoir comment supprimer une réunion ou un élément de rendez-vous à l’aide de EWS, voir [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-244">To learn how to delete a meeting or appointment item by using EWS, see [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="move-or-copy-items-to-another-mailbox"></a><span data-ttu-id="60b65-245">Déplacement ou copie d’éléments vers une autre boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="60b65-245">Move or copy items to another mailbox</span></span>
<span data-ttu-id="60b65-246"><a name="bk_movecopybtnmailboxes"> </a></span><span class="sxs-lookup"><span data-stu-id="60b65-246"></span></span>

<span data-ttu-id="60b65-247">Vous pouvez déplacer ou copier des éléments entre les boîtes aux lettres en utilisant les opérations [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) et [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="60b65-247">You can move or copy items between mailboxes by using the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) and [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) operations.</span></span> <span data-ttu-id="60b65-248">Pour plus d’informations, voir [exportation et importation d’éléments à l’aide de EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="60b65-248">To learn more, see [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="60b65-249">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="60b65-249">See also</span></span>

- [<span data-ttu-id="60b65-250">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="60b65-250">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="60b65-251">Utilisation de dossiers à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="60b65-251">Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="60b65-252">Suppression d’éléments à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="60b65-252">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)
    

