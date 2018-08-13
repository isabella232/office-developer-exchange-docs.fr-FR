---
title: Utilisations d’éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: a40cd7ae682c1fb0a8d2f9cfcb10d99d4ab08052
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353965"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a><span data-ttu-id="371d4-103">Utilisations d’éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="371d4-103">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>

<span data-ttu-id="371d4-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="371d4-104">Learn how to create, get, update, and delete items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="371d4-105">Vous pouvez utiliser l’API managée EWS ou EWS pour utiliser des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="371d4-105">You can use the EWS Managed API or EWS to work with items in a mailbox.</span></span> <span data-ttu-id="371d4-106">Vous pouvez utiliser des éléments génériques: des[éléments](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) de l’API managée EWS ou des[éléments](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx)de types EWS pour effectuer certaines opérations (telles que l’obtention ou la suppression d’un élément à l’aide de l’identificateur de ce dernier). Toutefois, la plupart du temps, vous devez utiliser un [élément fortement identifié](folders-and-items-in-ews-in-exchange.md#bk_item) pour effectuer une opération d’obtention ou de mise à jour, car vous devrez accéder aux propriétés propres à l’élément fortement identifié.</span><span class="sxs-lookup"><span data-stu-id="371d4-106">You can use generic items — EWS Managed API [Item](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) objects or EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) types — to perform some operations (getting an item or deleting an item by using the item's identifier); however, most of the time you'll have to use a [strongly typed item](folders-and-items-in-ews-in-exchange.md#bk_item) to perform a get or update operation because you'll need access to the properties that are specific to the strongly typed item.</span></span> 

<span data-ttu-id="371d4-107">Par exemple, vous ne pouvez pas utiliser un élément générique pour récupérer un élément qui contient une date de début et de fin. Pour ce faire, vous avez besoin d’un objet [de Rendez-vous](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)ou d’un[CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) de type EWS.</span><span class="sxs-lookup"><span data-stu-id="371d4-107">For example, you can't use a generic item to retrieve an item that contains a start and end date - you need an EWS Managed API [Appointment](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object or an EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) type to do that.</span></span> <span data-ttu-id="371d4-108">Si vous utilisez l’API managée EWS, vous devez toujours créer des éléments fortement identifiés, car la **classe**générique ne possède pas de constructeur.</span><span class="sxs-lookup"><span data-stu-id="371d4-108">And if you're using the EWS Managed API, you always have to create strongly typed items, because the generic **Item** class does not have a constructor.</span></span> <span data-ttu-id="371d4-109">Si vous utilisez un élément qui n’est pas fortement identifié, vous pouvez vous servir de la **classe**de base afin d’utiliser cet élément.</span><span class="sxs-lookup"><span data-stu-id="371d4-109">If you're working with an item that is not strongly typed, you can always use the base **Item** class to work with the item.</span></span> 
  
<span data-ttu-id="371d4-110">**Tableau 1. Méthodes d’API managée EWS et opérations EWS pour l’utilisation d’éléments**</span><span class="sxs-lookup"><span data-stu-id="371d4-110">**Table 1.  EWS Managed API methods and EWS operations for working with items**</span></span>

|<span data-ttu-id="371d4-111">**Afin de...**</span><span class="sxs-lookup"><span data-stu-id="371d4-111">**In order to**</span></span>|<span data-ttu-id="371d4-112">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="371d4-112">**EWS Managed API method**</span></span>|<span data-ttu-id="371d4-113">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="371d4-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="371d4-114">Créer un élément générique</span><span class="sxs-lookup"><span data-stu-id="371d4-114">Create a generic item</span></span>  <br/> |<span data-ttu-id="371d4-p103">Aucun. Vous pouvez uniquement créer des types d’élément spécifiques à l’aide de l’API managée EWS. Vous ne pouvez pas créer d’éléments génériques.</span><span class="sxs-lookup"><span data-stu-id="371d4-p103">None. You can only create specific item types by using the EWS Managed API; you cannot create generic items.</span></span>  <br/> |[<span data-ttu-id="371d4-117">CreateItem</span><span class="sxs-lookup"><span data-stu-id="371d4-117">CreateItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="371d4-118">Obtenir un élément</span><span class="sxs-lookup"><span data-stu-id="371d4-118">Get an item</span></span>  <br/> |[<span data-ttu-id="371d4-119">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="371d4-119">Item.Bind</span></span>](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="371d4-120">GetItem</span><span class="sxs-lookup"><span data-stu-id="371d4-120">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="371d4-121">Mettre à jour un élément</span><span class="sxs-lookup"><span data-stu-id="371d4-121">Update an item</span></span>  <br/> |[<span data-ttu-id="371d4-122">Item.Update</span><span class="sxs-lookup"><span data-stu-id="371d4-122">Item.Update</span></span>](http://msdn.microsoft.com/fr-FR/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="371d4-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="371d4-123">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="371d4-124">Supprimer un élément</span><span class="sxs-lookup"><span data-stu-id="371d4-124">Delete an item</span></span>  <br/> |[<span data-ttu-id="371d4-125">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="371d4-125">Item.Delete</span></span>](http://msdn.microsoft.com/fr-FR/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="371d4-126">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="371d4-126">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="371d4-127">Dans cet article, vous découvrirez également à quel moment vous pouvez utiliser la classe de base générique et à quel moment vous devez utiliser un élément fortement identifié pour mener à bien votre tâche.</span><span class="sxs-lookup"><span data-stu-id="371d4-127">In this article, you’ll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task. The code examples will show you how to use the base class, and what to do when you can’t use the base class or it doesn’t fit your needs.</span></span> <span data-ttu-id="371d4-128">Les exemples de code vous indiqueront comment utiliser la classe de base, ainsi que la marche à suivre lorsque vous ne pouvez pas utiliser cette dernière ou lorsqu’elle ne répond pas à vos besoins.</span><span class="sxs-lookup"><span data-stu-id="371d4-128">In this article, you’ll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task. The code examples will show you how to use the base class, and what to do when you can’t use the base class or it doesn’t fit your needs.</span></span>
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="371d4-129">Création d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-129">Create an item by using the EWS Managed API</span></span>
<span data-ttu-id="371d4-130"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-130"></span></span>

<span data-ttu-id="371d4-131">L’API managée EWS ne possède pas de constructeur publiquement disponible pour la [classe](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)d’élément. Par conséquent, afin de créer un élément, vous devez utiliser le constructeur approprié au type d’élément spécifique que vous souhaitez créer.</span><span class="sxs-lookup"><span data-stu-id="371d4-131">The EWS Managed API does not have a publicly available constructor for the [Item](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) class, so you must use the constructor for the specific item type you want to create in order to create an item.</span></span> <span data-ttu-id="371d4-132">Par exemple, utilisez le[constructeur de classe EmailMessage](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) pour créer un nouveau message électronique et le [constructeur de classe Contact](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) pour créer un contact.</span><span class="sxs-lookup"><span data-stu-id="371d4-132">For example, use the [EmailMessage class constructor](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create a new email message, and the [Contact class constructor](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) to create a new contact.</span></span> <span data-ttu-id="371d4-133">De même, le serveur ne renvoie jamais** d’objets**génériques dans les réponses. Tous les éléments génériques sont renvoyés sous forme d’objets **EmailMessage**.</span><span class="sxs-lookup"><span data-stu-id="371d4-133">Likewise, the server never returns generic **Item** objects in responses; all generic items are returned as **EmailMessage** objects.</span></span> 
  
<span data-ttu-id="371d4-p106">Lorsque vous connaissez le type d’élément à créer, vous pouvez effectuer la tâche en quelques étapes seulement. Les étapes sont similaires pour tous les types d’éléments :</span><span class="sxs-lookup"><span data-stu-id="371d4-p106">When you know the type of item to create, you can complete the task in just a few steps. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="371d4-136">Initialiser une nouvelle instance de l’un des classes[d’élément](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)avec l’objet[ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)en tant que paramètre.</span><span class="sxs-lookup"><span data-stu-id="371d4-136">Initialize a new instance of one of the [Item](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) classes with the [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object as a parameter.</span></span> 
    
2. <span data-ttu-id="371d4-p107">Les schémas sont différents pour chaque type d’élément, c’est pourquoi plusieurs propriétés sont disponibles pour ces derniers.</span><span class="sxs-lookup"><span data-stu-id="371d4-p107">Set properties on the item. The schemas are different for each item type, so different properties are available for different items.</span></span>
    
3. <span data-ttu-id="371d4-139">Enregistrez l’élément, ou enregistrez et envoyez l’élément.</span><span class="sxs-lookup"><span data-stu-id="371d4-139">Save the item, or save and send the item.</span></span>
    
<span data-ttu-id="371d4-140">Par exemple, vous pouvez créer un objet[EmailMessage](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx), définissez l’[objet](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [corps](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx), et les propriétés[ToRecipients](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx), puis envoyez-le à l’aide de la méthode[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-140">For example, you can create an [EmailMessage](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object, set the [Subject](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx), and [ToRecipients](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) properties, and then send it by using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
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

<span data-ttu-id="371d4-141">Pour découvrir comment créer un élément de réunion ou de rendez-vous à l’aide de l’API managée EWS, voir[ Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-141">To learn how to create a meeting or appointment item by using the EWS Managed API, see How to: Create appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="create-an-item-by-using-ews"></a><span data-ttu-id="371d4-142">Création d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-142">Create an item by using EWS</span></span>
<span data-ttu-id="371d4-143"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-143"></span></span>

<span data-ttu-id="371d4-p108">Vous pouvez créer un élément générique ou un élément fortement identifié à l’aide d’EWS. Les étapes sont identiques pour tous les types d’éléments:</span><span class="sxs-lookup"><span data-stu-id="371d4-p108">You can create a generic item or a strongly typed item by using EWS. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="371d4-146">Utilisez l’opération [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) pour créer un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="371d4-146">Use the [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to create an item in the Exchange store.</span></span> 
    
2. <span data-ttu-id="371d4-147">Utilisez l’élément [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) qui contiendra un élément ou plus à créer.</span><span class="sxs-lookup"><span data-stu-id="371d4-147">Use the [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) element to contain one or more items to create.</span></span> 
    
3. <span data-ttu-id="371d4-148">Définissez des propriétés sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="371d4-148">Set properties on the item.</span></span>
    
<span data-ttu-id="371d4-149">Par exemple, vous pouvez créer un message électronique et l’envoyer à l’aide du code de l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="371d4-149">For example, you can create an email message and send it by using the code in the following example.</span></span> <span data-ttu-id="371d4-150">Il s’agit également de la demande XML que l’API Managée EWS envoie lorsque vous appelez la méthode[SendAndSaveCopy](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-150">This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [get all attachments from an email](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx).</span></span> 
  
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

<span data-ttu-id="371d4-151">Le serveur répond à la demande**CreateItem** par un message [GetItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), qui inclut [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) renvoyant la valeur **NoError**, indiquant que le message a bien été créé, et où apparaît l’élément [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) du nouveau message.</span><span class="sxs-lookup"><span data-stu-id="371d4-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="371d4-152">Pour découvrir comment créer un élément de réunion ou de rendez-vous à l’aide d’EWS, voir [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-152">To learn how to create a meeting or appointment item by using EWS, see How to: Create appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="371d4-153">Obtention d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-153">Get an item by using the EWS Managed API</span></span>
<span data-ttu-id="371d4-154"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-154"></span></span>

<span data-ttu-id="371d4-155">Pour utiliser l’API Managée EWS afin de récupérer un élément si vous connaissez l’[Item.Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à récupérer, vous appelez simplement une des méthodes[Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx)sur l’élément et l’élément est récupéré.</span><span class="sxs-lookup"><span data-stu-id="371d4-155">To use the EWS Managed API to get an item if you know the [Item.Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to retrieve, you simply call one of the [Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) methods on the item, and the item is retrieved.</span></span> <span data-ttu-id="371d4-156">Pour une expérience optimale, nous vous recommandons de limiter les propriétés renvoyées à celles qui sont requises.</span><span class="sxs-lookup"><span data-stu-id="371d4-156">As a best practice, we recommend that you limit the properties returned to only those that are required.</span></span> <span data-ttu-id="371d4-157">Cet exemple renvoie la propriété **Id**de l’élément et la propriété** de l’objet**.</span><span class="sxs-lookup"><span data-stu-id="371d4-157">This example returns the item **Id** property and the **Subject** property.</span></span> 
  
<span data-ttu-id="371d4-158">Cet exemple suppose que le **service** est un valide objet[ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="371d4-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that itemId is the ItemId of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="371d4-159">La variable locale*itemId* est la[Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="371d4-159">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

<span data-ttu-id="371d4-160">Si vous recherchez un élément qui répond à des critères spécifiques, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="371d4-160">If you’re searching for an item that meets specific criteria, do the following:</span></span>
  
1. <span data-ttu-id="371d4-161">Établissez une liaison vers le dossier qui contient les éléments à obtenir.</span><span class="sxs-lookup"><span data-stu-id="371d4-161">Bind to the folder that contains the items to get.</span></span>
    
2. <span data-ttu-id="371d4-162">Instanciez un[SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) ou un [PropertySet](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour filtrer les éléments à retenir.</span><span class="sxs-lookup"><span data-stu-id="371d4-162">Instantiate a [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) or a [PropertySet](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to filter the items to return.</span></span> 
    
3. <span data-ttu-id="371d4-163">Instanciez un objet[ItemView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) ou d’un[CalendarView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx)afin de spécifier le nombre d’éléments à retenir.</span><span class="sxs-lookup"><span data-stu-id="371d4-163">Instantiate an [ItemView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object to specify the number of items to return.</span></span> 
    
4. <span data-ttu-id="371d4-164">Appelez la méthode[ExchangeService.FindItems](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [ExchangeService.FindAppointments](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-164">Call the [ExchangeService.FindItems](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [ExchangeService.FindAppointments](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="371d4-165">Par exemple, si vous souhaitez récupérer des messages électroniques non lus dans la boîte de réception, vous pouvez utiliser le code de l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="371d4-165">For example, if you want to retrieve unread email messages in the Inbox, use the code in the following example.</span></span> <span data-ttu-id="371d4-166">Cet exemple utilise un élément **SearchFilterCollection**pour limiter les résultats de la méthode**FindItems aux messages** aux messages non lus et limite l’élément**ItemView** afin de réduire les résultats à un seul élément.</span><span class="sxs-lookup"><span data-stu-id="371d4-166">This example uses a **SearchFilterCollection** to limit the results of the **FindItems** method to unread messages, and limits the **ItemView** to limit results to one item.</span></span> <span data-ttu-id="371d4-167">Ce code particulier fonctionne uniquement sur les objets[EmailMessage](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx), car la valeur [EmailMessageSchema.IsRead](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) fait partie de la **SearchFilter**.</span><span class="sxs-lookup"><span data-stu-id="371d4-167">This particular code only works on [EmailMessage](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects because the [EmailMessageSchema.IsRead](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) value is part of the **SearchFilter**.</span></span> 
  
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

<span data-ttu-id="371d4-168">Parallèlement, vous pouvez également utiliser un[PropertySet](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour limiter les résultats de la recherche, comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="371d4-168">Alternatively, you can use a [PropertySet](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) to limit the results of the search as shown in the following code example.</span></span> <span data-ttu-id="371d4-169">Cet exemple utilise la méthode[FindAppointments](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx)afin de récupérer un maximum de cinq rendez-vous qui se produisent dans les 30 jours suivants.</span><span class="sxs-lookup"><span data-stu-id="371d4-169">This example uses the [FindAppointments](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve up to five appointments that occur in the next 30 days.</span></span> <span data-ttu-id="371d4-170">Bien sûr, ce code fonctionne uniquement pour les éléments du calendrier.</span><span class="sxs-lookup"><span data-stu-id="371d4-170">This code of course only works on calendar items.</span></span> 
  
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

<span data-ttu-id="371d4-171">Notez que les informations que le serveur renvoie dans la réponse de la méthode **Bind** sont différentes des informations que le serveur renvoie pour une réponse de la méthode**FindItem** ou**FindAppointment**.</span><span class="sxs-lookup"><span data-stu-id="371d4-171">Note that the information the server returns in the **Bind** method response is different than the information that the server returns for a **FindItem** or **FindAppointment** method response.</span></span> <span data-ttu-id="371d4-172">La méthode**Bind** peut renvoyer toutes les propriétés schématisées, alors que les méthodes**FindItem**et**FindAppointment**ne les renvoient pas.</span><span class="sxs-lookup"><span data-stu-id="371d4-172">The **Bind** method can return all the schematized properties, whereas the **FindItem** and **FindAppointment** methods do not return all the schematized properties.</span></span> <span data-ttu-id="371d4-173">Par conséquent, si vous avez besoin d’un accès complet à l’élément, vous devez utiliser la méthode**Bind**.</span><span class="sxs-lookup"><span data-stu-id="371d4-173">So if you need full access to the item, you'll have to use the **Bind** method.</span></span> <span data-ttu-id="371d4-174">Si vous ne disposez pas de l’élément **Id**de l’élément que vous souhaitez récupérer, utilisez les méthodes**FindItem** ou **FindAppointment**pour récupérer l’identité, puis utilisez la méthode **Bind **pour récupérer les propriétés dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="371d4-174">If you don't have the item **Id** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** methods to retrieve the Id, and then use the **Bind** method to retrieve the properties you need.</span></span> 
  
<span data-ttu-id="371d4-175">Pour découvrir comment obtenir un élément de réunion ou de rendez-vous à l’aide de l’API managée EWS, voir[Obtenir des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-175">To learn how to get a meeting or appointment item by using the EWS Managed API, see How to: Get appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="get-an-item-by-using-ews"></a><span data-ttu-id="371d4-176">Obtention d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-176">Get an item by using EWS</span></span>
<span data-ttu-id="371d4-177"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-177"></span></span>

<span data-ttu-id="371d4-178">Si vous connaissez l’[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de l’élément à récupérer, vous pouvez obtenir ce dernier à l’aide de l’opération [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-178">If you know the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the item to retrieve, you can get the item by using the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="371d4-179">L’exemple suivant présente la requête XML permettant d’obtenir l’[objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) d’un élément comportant un **ItemId** spécifique.</span><span class="sxs-lookup"><span data-stu-id="371d4-179">The following example shows the XML request to get the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of an item with a specific **ItemId**.</span></span> <span data-ttu-id="371d4-180">Il s’agit également de la requête XML que l’API Managée EWS envoie lorsque vous appelez la méthode[Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) sur un**ItemId**.</span><span class="sxs-lookup"><span data-stu-id="371d4-180">This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method on an **ItemId**.</span></span> <span data-ttu-id="371d4-181">Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="371d4-181">The values of some attributes and elements have been shortened for readability.</span></span>
  
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

<span data-ttu-id="371d4-p116">L’exemple suivant présente la réponse XML que le serveur renvoie après avoir effectué l’opération **GetItem**. La réponse indique que l’élément a été récupéré. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="371d4-p116">The following example shows the XML response that the server returns after it processes the **GetItem** operation. The response indicates the item was retrieved successfully. The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="371d4-185">Si vous ne connaissez pas l’élément **ItemId** de l’élément que vous souhaitez récupérer, vous pouvez utiliser l’opération[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) à cette fin.</span><span class="sxs-lookup"><span data-stu-id="371d4-185">If you do not know the **ItemId** of the item you want to retrieve, you can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find the item.</span></span> <span data-ttu-id="371d4-186">Pour pouvoir utiliser l’opération**FindItem**, vous devez d’abord identifier le dossier que vous recherchez.</span><span class="sxs-lookup"><span data-stu-id="371d4-186">In order to use the **FindItem** operation, you must first identify the folder that you're searching.</span></span> <span data-ttu-id="371d4-187">Vous pouvez identifier le dossier à l’aide de son **DistinguinguishedFolderName** ou à l’aide de l’élément [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-187">You can identify the folder by using its **DistinguinguishedFolderName** or by using the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span></span> <span data-ttu-id="371d4-188">Vous pouvez utiliser soit l’opération [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) soit l’opération[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) pour obtenir l’élément **FolderId** dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="371d4-188">You can use either the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) or [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operations to get the **FolderId** you need.</span></span> <span data-ttu-id="371d4-189">Ensuite, utilisez l’opération**FindItem** pour rechercher ce dossier et pour obtenir des résultats qui correspondent au filtre de recherche.</span><span class="sxs-lookup"><span data-stu-id="371d4-189">Then use the **FindItem** operation to search that folder for results that match the search filter.</span></span> <span data-ttu-id="371d4-190">Contrairement à l’API managée EWS, EWS n’offre pas d’opération de recherche distincte pour les rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="371d4-190">Unlike the EWS Managed API, EWS does not provide a separate find operation for appointments.</span></span> <span data-ttu-id="371d4-191">L’opération** FindItem**récupère des éléments de tous types.</span><span class="sxs-lookup"><span data-stu-id="371d4-191">The **FindItem** operation retrieves items of all types.</span></span> 
  
<span data-ttu-id="371d4-p118">L’exemple suivant présente la demande d’opération **FindItem** XML qui est envoyée au serveur pour rechercher des rendez-vous prévus dans les 30 jours, dans le dossier de calendrier. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="371d4-p118">The following example shows the XML **FindItem** operation request that is sent to the server to find appointments in the Calendar folder that occur in the next 30 days. The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="371d4-p119">Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) comprenant la valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de l’élément **NoError**, qui indique que l’opération a abouti. Si des éléments de calendrier répondent à des critères de filtre, ils sont inclus dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="371d4-p119">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the operation completed successfully. If any calendar items meet the filtering criteria, they are included in the response.</span></span>
  
<span data-ttu-id="371d4-196">Notez que les informations que le serveur renvoie dans la réponse de l’opération **GetItem** sont différentes des informations que le serveur renvoie dans une réponse de l’opération**FindItem** ou **FindAppointment**.</span><span class="sxs-lookup"><span data-stu-id="371d4-196">Note that the information the server returns in the **GetItem** operation response is different than the information the server returns in a **FindItem** or **FindAppointment** operation response.</span></span> <span data-ttu-id="371d4-197">L’opération**GetItem** peut renvoyer toutes les propriétés schématisées, alors que les opérations**FindItem**et**FindAppointment**ne les renvoient pas.</span><span class="sxs-lookup"><span data-stu-id="371d4-197">The **GetItem** operation can return all the schematized properties, whereas the **FindItem** and **FindAppointment** operations do not return all the schematized properties.</span></span> <span data-ttu-id="371d4-198">Par conséquent, si vous avez besoin d’un accès complet à l’élément, vous devez utiliser l’opération **GetItem**.</span><span class="sxs-lookup"><span data-stu-id="371d4-198">So if you need full access to the item, you'll have to use the **GetItem** operation.</span></span> <span data-ttu-id="371d4-199">Si vous ne disposez pas de l’**ItemId**de l’élément que vous souhaitez récupérer, utilisez les opérations**FindItem** ou **FindAppointment**pour récupérer l’**ItemId**, puis utilisez l’opération**GetItem**pour récupérer les éléments dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="371d4-199">If you don't have the **ItemId** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** operations to retrieve the **ItemId**, and then use the **GetItem** operation to retrieve the elements you need.</span></span> 
  
<span data-ttu-id="371d4-200">Pour découvrir comment obtenir un élément de réunion ou de rendez-vous à l’aide d’EWS, voir [Obtenir des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-200">To learn how to get a meeting or appointment item by using EWS, see How to: Get appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="371d4-201">Mise à jour d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-201">Update an item by using the EWS Managed API</span></span>
<span data-ttu-id="371d4-202"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-202"></span></span>

<span data-ttu-id="371d4-203">Les étapes pour mettre à jour un élément à l’aide de l’API managée EWS sont similaires pour tous les types d’éléments. Toutefois, les propriétés sont différentes pour chaque type d’élément et la méthode [de Mise à jour](http://msdn.microsoft.com/fr-FR/library/office/dd635915%28v=exchg.80%29.aspx)présente de nombreuses méthodes surchargées parmi lesquelles faire votre choix.</span><span class="sxs-lookup"><span data-stu-id="371d4-203">The steps to update an item by using the EWS Managed API are similar for all item types; however, the item properties are different for each item type, and the [Updatehttp://msdn.microsoft.com/en-us/library/office/dd635915(v=exchg.80).aspx](http://msdn.microsoft.com/fr-FR/library/office/dd635915%28v=exchg.80%29.aspx) method has many overloaded methods to choose from. To update an item:</span></span> <span data-ttu-id="371d4-204">Pour mettre à jour un élément, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="371d4-204">To update an item:</span></span> 
  
1. <span data-ttu-id="371d4-205">Utilisez la méthode[Bind](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour obtenir la dernière version de l’élément, sauf si vous la possédez déjà.</span><span class="sxs-lookup"><span data-stu-id="371d4-205">Use the [GetItem](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> <span data-ttu-id="371d4-206">Pour mettre à jour des propriétés propres à un élément fortement identifié, vous devez établir une liaison avec ce type d’élément.</span><span class="sxs-lookup"><span data-stu-id="371d4-206">To update properties specific to a strongly typed item, you'll have to bind to that item type.</span></span> <span data-ttu-id="371d4-207">Pour mettre à jour des propriétés disponibles sur le type d’élément générique, vous pouvez lier à l’objet de l’[élément](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-207">To update properties available on the generic item type, you can bind to the [Item](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> 
    
2. <span data-ttu-id="371d4-208">Mettez à jour les propriétés sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="371d4-208">Update the properties on the item.</span></span>
    
3. <span data-ttu-id="371d4-209">Appelez la méthode de**mise à jour**.</span><span class="sxs-lookup"><span data-stu-id="371d4-209">Call the **Update** method.</span></span> 
    
<span data-ttu-id="371d4-210">Par exemple, vous pouvez mettre à jour l’objet d’un message électronique à l’aide du type d’élément générique, comme illustré dans le code de l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="371d4-210">For example, you can update the subject of an email by using the generic item type, as shown in the code in the following example.</span></span>
  
<span data-ttu-id="371d4-211">Cet exemple suppose que le **service** est un valide objet[ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="371d4-211">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that itemId is the ItemId of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="371d4-212">La variable locale*itemId* est la[Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="371d4-212">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
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

<span data-ttu-id="371d4-213">Pour découvrir comment mettre à jour un élément de réunion ou de rendez-vous à l’aide de l’API managée EWS, voir [ Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-213">To learn how to update a meeting or appointment item by using the EWS Managed API, see How to: Update appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="update-an-item-by-using-ews"></a><span data-ttu-id="371d4-214">Mise à jour d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-214">Update an item by using EWS</span></span>
<span data-ttu-id="371d4-215"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-215"></span></span>

<span data-ttu-id="371d4-216">Pour mettre à jour un élément à l’aide d’EWS, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="371d4-216">To update an item by using EWS, do the following:</span></span>
  
1. <span data-ttu-id="371d4-217">Utilisez l’opération [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir la dernière version de l’élément, sauf si vous la possédez déjà.</span><span class="sxs-lookup"><span data-stu-id="371d4-217">Use the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> 
    
2. <span data-ttu-id="371d4-218">Utilisez l’opération [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) afin de spécifier des champs à mettre à jour et d’affecter de nouvelles valeurs à ces champs.</span><span class="sxs-lookup"><span data-stu-id="371d4-218">Use the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to specify fields to update and assign new values to those fields.</span></span> 
    
<span data-ttu-id="371d4-p124">L’exemple suivant présente la demande d’opération **UpdateItem** XML qui est envoyée au serveur pour mettre à jour l’[objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) du message électronique. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="371d4-p124">The following example shows the XML **UpdateItem** operation request that is sent to the server to update the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) value of the email message. The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="371d4-221">Le serveur répond à la requête **UpdateItem** par un message [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) comprenant la valeur [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, qui indique que l’élément a été mis à jour avec succès.</span><span class="sxs-lookup"><span data-stu-id="371d4-221">The server responds to the **UpdateItem** request with a [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes the a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item update was successful.</span></span>
  
<span data-ttu-id="371d4-222">Pour découvrir comment mettre à jour un élément de réunion ou de rendez-vous à l’aide d’EWS, voir[Mettre à jour des rendez-vous et des réunions à l’aide d’EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-222">To learn how to update a meeting or appointment item by using EWS, see How to: Update appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="371d4-223">Suppression d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-223">Delete an item by using the EWS Managed API</span></span>
<span data-ttu-id="371d4-224"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-224"></span></span>

<span data-ttu-id="371d4-225">Vous pouvez supprimer des éléments en les déplaçant vers le dossier Éléments supprimés ou en les envoyant dans la corbeille.</span><span class="sxs-lookup"><span data-stu-id="371d4-225">You can delete items by moving them to the Deleted Items folder or to the dumpster.</span></span> <span data-ttu-id="371d4-226">Si vous connaissez l’[ItemId](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à supprimer, appelez simplement la méthode[Supprimer](http://msdn.microsoft.com/fr-FR/library/office/dd635072%28v=exchg.80%29.aspx)sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="371d4-226">If you know the [ItemId](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to delete, just call the [Delete](http://msdn.microsoft.com/fr-FR/library/office/dd635072%28v=exchg.80%29.aspx) method on the item.</span></span> 
  
<span data-ttu-id="371d4-227">Si vous devez rechercher l’élément avant de le supprimer, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="371d4-227">If you need to find the item before deleting it, do the following:</span></span>
  
1. <span data-ttu-id="371d4-228">Appelez la méthode [FindItems](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [FindAppointments](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx)pour rechercher l’élément à supprimer.</span><span class="sxs-lookup"><span data-stu-id="371d4-228">Call the [FindItems](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [FindAppointments](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to find the item to delete.</span></span> 
    
1. <span data-ttu-id="371d4-229">Instanciez un[PropertySet](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx)et limitez-le aux propriétés à renvoyer, ou utilisez un[SearchFilterCollection](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx)pour rechercher des éléments spécifiques.</span><span class="sxs-lookup"><span data-stu-id="371d4-229">Instantiate a [PropertySet](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) and limit it to the properties to return, or use a [SearchFilterCollection](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) to find specific items.</span></span> 
    
2. <span data-ttu-id="371d4-230">Instanciez un objet[ItemView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) ou[CalendarView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx)afin de spécifier le nombre d’éléments à retenir. </span><span class="sxs-lookup"><span data-stu-id="371d4-230">Instantiate an [ItemView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) to specify the number of items to return.</span></span> 
    
2. <span data-ttu-id="371d4-231">Appelez la méthode[supprimer](http://msdn.microsoft.com/fr-FR/library/office/dd635072%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-231">Call the [Delete](http://msdn.microsoft.com/fr-FR/library/office/dd635072%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="371d4-232">Par exemple, le code suivant indique comment déplacer un message électronique vers le dossier Éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="371d4-232">For example, the following code shows how to move an email message to the Deleted Items folder.</span></span>
  
<span data-ttu-id="371d4-233">Cet exemple suppose que le **service** est un valide objet[ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="371d4-233">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that itemId is the ItemId of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="371d4-234">La variable locale*itemId* est la[Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="371d4-234">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

<span data-ttu-id="371d4-235">Pour plus d’informations sur la suppression d’éléments, voir [supprime les éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-235">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="371d4-236">Pour découvrir comment supprimer un élément de réunion ou de rendez-vous à l’aide de l’API managée EWS, voir [ Supprimer des rendez-vous et annuler des réunions à l’aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-236">For more details about deleting items, see Deleting items by using EWS in Exchange. To learn how to delete a meeting or appointment item by using the EWS Managed API, see How to: Delete appointments and cancel meetings by using EWS in Exchange.</span></span>
  
## <a name="delete-an-item-by-using-ews"></a><span data-ttu-id="371d4-237">Suppression d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="371d4-237">Delete an item by using EWS</span></span>
<span data-ttu-id="371d4-238"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-238"></span></span>

<span data-ttu-id="371d4-239">Vous pouvez supprimer un élément à l’aide de l’opération [DeleteItem](../web-service-reference/deleteitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-239">You can delete an item by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> 
  
<span data-ttu-id="371d4-p128">L’exemple suivant présente la demande XML qui est envoyée au serveur pour déplacer le message vers le dossier Éléments supprimés. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="371d4-p128">The following example shows the XML request that is sent to the server to move the email message to the Deleted Items folder. The values of some attributes and elements have been shortened for readability.</span></span>
  
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

<span data-ttu-id="371d4-242">Le serveur répond à la requête **UpdateItem** par un message [UpdateItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) comprenant la valeur [ResponseCode](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, qui indique que l’élément a été supprimé avec succès.</span><span class="sxs-lookup"><span data-stu-id="371d4-242">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes the a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/fr-FR/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span>
  
<span data-ttu-id="371d4-243">Pour plus d’informations sur la suppression d’éléments, voir [supprime les éléments à l’aide d’EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-243">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="371d4-244">Pour découvrir comment supprimer un élément de réunion ou de rendez-vous à l’aide d’EWS, voir [ Supprimer des rendez-vous et annuler des réunions à l’aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-244">For more details about deleting items, see Deleting items by using EWS in Exchange. To learn how to delete a meeting or appointment item by using EWS, see How to: Delete appointments and cancel meetings by using EWS in Exchange.</span></span>
  
## <a name="move-or-copy-items-to-another-mailbox"></a><span data-ttu-id="371d4-245">Déplacement ou copie d’éléments vers une autre boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="371d4-245">Move or copy items to another mailbox</span></span>
<span data-ttu-id="371d4-246"><a name="bk_movecopybtnmailboxes"> </a></span><span class="sxs-lookup"><span data-stu-id="371d4-246"></span></span>

<span data-ttu-id="371d4-247">Vous pouvez déplacer ou copier des éléments d’une boîte aux lettres vers une autre à l’aide des opérations [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) et [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="371d4-247">You can move or copy items between mailboxes by using the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) and [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) operations. To learn more, see Importing and exporting items by using EWS in Exchange.</span></span> <span data-ttu-id="371d4-248">Pour plus d’informations, voir [Exportation et importation d’éléments à l’aide d’EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="371d4-248">To learn more, see [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="371d4-249">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="371d4-249">See also</span></span>

- [<span data-ttu-id="371d4-250">Dossiers et éléments dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="371d4-250">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="371d4-251">Utiliser des dossiers à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="371d4-251">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="371d4-252">Supprimer des éléments à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="371d4-252">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)
    

