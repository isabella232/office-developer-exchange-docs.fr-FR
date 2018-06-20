---
title: Obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Découvrez comment obtenir les photos de l’utilisateur qui sont associés à une boîte aux lettres ou de contact à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754871"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a><span data-ttu-id="b0aaa-103">Obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b0aaa-103">Get user photos by using EWS in Exchange</span></span>

<span data-ttu-id="b0aaa-104">Découvrez comment obtenir les photos de l’utilisateur qui sont associés à une boîte aux lettres ou de contact à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-104">Learn how to get user photos that are associated with a mailbox or contact by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b0aaa-105">C’est agréable à associer un visage à un nom.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-105">It's nice to put a face to a name.</span></span> <span data-ttu-id="b0aaa-106">Si vos utilisateurs comme mettre des noms aux faces, votre application peut demander une image, généralement une photo, à partir d’Exchange qui représente un compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-106">If your users like to put names to faces, your application can request an image, typically a photo, from Exchange that represents an email account.</span></span> <span data-ttu-id="b0aaa-107">Vous pouvez obtenir une photo stockée sur un serveur Exchange pour une boîte aux lettres de l’utilisateur, ou vous pouvez obtenir une photo du contact à partir de contacts stockés dans votre boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-107">You can get a user photo stored on an Exchange server for a mailbox, or you can get a contact photo from contacts stored in your mailbox.</span></span>
  
<span data-ttu-id="b0aaa-108">Vous pouvez utiliser les différentes technologies pour obtenir des photos à partir des boîtes aux lettres ou les Services de domaine Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="b0aaa-108">You can use several different technologies to get photos from mailboxes or Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="b0aaa-109">La meilleure façon pour obtenir une photo varie selon le type de contact que vous souhaitez obtenir à partir d’une photo.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-109">The best way to get a photo depends on the type of contact that you want to get a photo from.</span></span> 
  
<span data-ttu-id="b0aaa-110">**Le tableau 1. Technologies à utiliser pour obtenir les photos de l’utilisateur selon le type de contact**</span><span class="sxs-lookup"><span data-stu-id="b0aaa-110">**Table 1. Technologies to use to get user photos based on contact type**</span></span>

|<span data-ttu-id="b0aaa-111">**Type de contact**</span><span class="sxs-lookup"><span data-stu-id="b0aaa-111">**Contact type**</span></span>|<span data-ttu-id="b0aaa-112">**Technologies à utiliser**</span><span class="sxs-lookup"><span data-stu-id="b0aaa-112">**Technologies to use**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0aaa-113">Photo de boîte aux lettres utilisateur</span><span class="sxs-lookup"><span data-stu-id="b0aaa-113">Mailbox user photo</span></span>  <br/> |[<span data-ttu-id="b0aaa-114">Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de REST</span><span class="sxs-lookup"><span data-stu-id="b0aaa-114">Get a mailbox user photo by using REST</span></span>](#bk_REST)<br/><br/> [<span data-ttu-id="b0aaa-115">Obtenir une photo de l’utilisateur à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b0aaa-115">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |
|<span data-ttu-id="b0aaa-116">Photo de contacter l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="b0aaa-116">Contact user photo</span></span>  <br/> |[<span data-ttu-id="b0aaa-117">Obtenir une photo de contacter l’utilisateur à l’aide des API managées</span><span class="sxs-lookup"><span data-stu-id="b0aaa-117">Get a contact user photo by using EWS Managed API</span></span>](#bk_EWSMA)<br/><br/> [<span data-ttu-id="b0aaa-118">Obtenir une photo de l’utilisateur à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b0aaa-118">Get a user photo by using EWS</span></span>](#bk_EWS) <br/> |

<span data-ttu-id="b0aaa-119"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="b0aaa-119"></span></span>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a><span data-ttu-id="b0aaa-120">Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de REST</span><span class="sxs-lookup"><span data-stu-id="b0aaa-120">Get a mailbox user photo by using REST</span></span>

<span data-ttu-id="b0aaa-121">Vous pouvez demander des photos de l’utilisateur à partir d’un serveur Exchange à l’aide d’une demande HTTPS **GET** standard.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-121">You can request user photos from an Exchange server by using a standard HTTPS **GET** request.</span></span> <span data-ttu-id="b0aaa-122">Dans la demande, spécifiez l’adresse électronique du compte et un code de taille de l’image, comme indiqué dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-122">In the request, specify the email account address and a size code for the image, as shown in the following example.</span></span> 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

<span data-ttu-id="b0aaa-123">L’opération de [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) de service de découverte automatique permet de récupérer le paramètre **ExternalEwsUrl** , qui contient l’URL du point de terminaison Exchange Web Services (EWS) et l’emplacement du gestionnaire **Exchange.asmx** HTTP qui renvoie le photos de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-123">Use the Autodiscover service [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) operation to retrieve the **ExternalEwsUrl** setting, which contains the URL of the Exchange Web Services (EWS) endpoint and the location of the **Exchange.asmx** HTTP handler that returns the user photos.</span></span> 
  
<span data-ttu-id="b0aaa-124">Chaque code taille indique la hauteur et la largeur de l’image en pixels.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-124">Each size code indicates the height and width of the image in pixels.</span></span> <span data-ttu-id="b0aaa-125">Par exemple, le code de taille **HR48x48** renvoie une image qui est 48 pixels de haut 48 pixels de large.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-125">For example, the size code **HR48x48** returns an image that is 48 pixels high by 48 pixels wide.</span></span> <span data-ttu-id="b0aaa-126">Les valeurs possibles pour le paramètre de code de taille sont les mêmes que les valeurs possibles pour l’élément [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b0aaa-126">The possible values for the size code parameter are the same as the possible values for the [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="b0aaa-127">Si la demande spécifie une taille qui n’est pas disponible, la plus grande photo disponible est retournée.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-127">If the request specifies a size that is not available, the largest available photo will be returned.</span></span> <span data-ttu-id="b0aaa-128">Si aucune photo n’est stocké sur le serveur Exchange, l’image miniature stocké dans AD DS pour le compte est retournée.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-128">If no photo is stored on the Exchange server, the thumbnail image stored in AD DS for the account will be returned.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b0aaa-129">Le code de taille **HR48x48** renvoie toujours l’image miniature de domaine Active Directory si elle est disponible.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-129">The **HR48x48** size code always returns the AD DS thumbnail image if it is available.</span></span> 
  
<span data-ttu-id="b0aaa-130">L’exemple suivant montre comment vous pouvez utiliser la requête GET pour récupérer la photo d’utilisateur pour Sadie et enregistrez-le sur votre ordinateur local.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-130">The following example shows how you can use the GET request to retrieve the user photo for Sadie and save it to your local computer.</span></span>
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

<span data-ttu-id="b0aaa-131">La requête retourne une réponse HTTP.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-131">The request will return an HTTP response.</span></span> 
  
<span data-ttu-id="b0aaa-132">**Le tableau 2. Codes de réponse pour une demande de GetUserPhoto**</span><span class="sxs-lookup"><span data-stu-id="b0aaa-132">**Table 2. Response codes for a GetUserPhoto request**</span></span>

|<span data-ttu-id="b0aaa-133">**Code de réponse**</span><span class="sxs-lookup"><span data-stu-id="b0aaa-133">**Response code**</span></span>|<span data-ttu-id="b0aaa-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0aaa-134">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0aaa-135">200</span><span class="sxs-lookup"><span data-stu-id="b0aaa-135">200</span></span>  <br/> |<span data-ttu-id="b0aaa-136">Une image est disponible pour le compte de messagerie spécifié et l’image binaire est contenue dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-136">An image is available for the specified email account and the binary image is contained in the response.</span></span>  <br/> |
|<span data-ttu-id="b0aaa-137">304</span><span class="sxs-lookup"><span data-stu-id="b0aaa-137">304</span></span>  <br/> |<span data-ttu-id="b0aaa-138">L’image n’a pas été modifié depuis la dernière exécution de que l' **ETag** a été renvoyée à l’application.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-138">The image has not changed since the last time the **ETag** was returned to the application.</span></span>  <br/> |
|<span data-ttu-id="b0aaa-139">404</span><span class="sxs-lookup"><span data-stu-id="b0aaa-139">404</span></span>  <br/> |<span data-ttu-id="b0aaa-140">Aucune image n’est disponible pour le compte de messagerie spécifié.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-140">No image is available for the specified email account.</span></span>  <br/> |

<span data-ttu-id="b0aaa-141"><a name="bk_REST"> </a></span><span class="sxs-lookup"><span data-stu-id="b0aaa-141"></span></span>

## <a name="cache-user-photos"></a><span data-ttu-id="b0aaa-142">Photos de l’utilisateur du cache</span><span class="sxs-lookup"><span data-stu-id="b0aaa-142">Cache user photos</span></span>

<span data-ttu-id="b0aaa-143">Exchange renvoie les données avec un type de contenu d’image/jpeg, ainsi que d’une collection de valeurs d’en-tête.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-143">Exchange returns the data with a content type of image/jpeg, along with a collection of header values.</span></span> <span data-ttu-id="b0aaa-144">L’en-tête **ETag** est similaire à une clé de modification.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-144">The **ETag** header is similar to a change key.</span></span> <span data-ttu-id="b0aaa-145">La valeur est une chaîne qui représente la dernière mise à jour de la photo.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-145">The value is a string that represents the last time the photo was updated.</span></span> <span data-ttu-id="b0aaa-146">L' **ETag** reste identique pour la photo d’utilisateur jusqu'à ce que la photo est modifiée.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-146">The **ETag** remains the same for the user photo until the photo is changed.</span></span> <span data-ttu-id="b0aaa-147">Vous pouvez envoyer cette valeur **ETag** sur le serveur de la demande dans un en-tête **If-None-Match** HTTPS à **obtenir** .</span><span class="sxs-lookup"><span data-stu-id="b0aaa-147">You can send this **ETag** value to the server in the HTTPS **GET** request in an **If-None-Match** header.</span></span> <span data-ttu-id="b0aaa-148">Si la photo n’a pas changé depuis la dernière demande, le serveur répond avec une réponse HTTP 304 indiquant en tant que telles.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-148">If the photo hasn't changed since the last request, the server will respond with an HTTP 304 response that indicates as such.</span></span> <span data-ttu-id="b0aaa-149">Cela signifie que vous pouvez utiliser la photo de l’utilisateur demandé et enregistré précédemment au lieu de traitement d’une autre.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-149">This means that you can use the user photo that you previously requested and saved rather than processing a new one.</span></span> 

<span data-ttu-id="b0aaa-150"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="b0aaa-150"></span></span>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a><span data-ttu-id="b0aaa-151">Obtenir une photo de contacter l’utilisateur à l’aide des API managées</span><span class="sxs-lookup"><span data-stu-id="b0aaa-151">Get a contact user photo by using EWS Managed API</span></span>

<span data-ttu-id="b0aaa-152">Votre application peut utiliser l’API managée EWS pour récupérer les photos des contacts, si le contact est stocké dans un dossier de contacts dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-152">Your application can use the EWS Managed API to retrieve photos for contacts, if the contact is stored in a contact folder in the user's mailbox.</span></span> <span data-ttu-id="b0aaa-153">Pour ce faire, tout d’abord, recherchez l' **ID d’élément** pour le contact vous souhaitez utiliser.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-153">To do this, first, find the **ItemId** for the contact you want use.</span></span> <span data-ttu-id="b0aaa-154">Ensuite, après avoir lié à ce contact, charger à la collection attachments.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-154">Then, after you bind to that contact, load it to the attachments collection.</span></span> <span data-ttu-id="b0aaa-155">Si le contact dispose d’une photo, la photo sera une des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-155">If the contact has a photo, the photo will be one of the attachments.</span></span> <span data-ttu-id="b0aaa-156">Boucle sur la collection de pièces jointes, en vérifiant la valeur de la propriété **IsContactPhoto** .</span><span class="sxs-lookup"><span data-stu-id="b0aaa-156">Loop through the attachments collection, checking the value of the **IsContactPhoto** property.</span></span> <span data-ttu-id="b0aaa-157">Lorsque vous avez trouvé la photo du contact, vous pouvez l’enregistrer sur votre ordinateur local et vos applications peuvent y accéder.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-157">When you find the contact photo, you can save it to your local computer, and your application can access it.</span></span> 
  
<span data-ttu-id="b0aaa-158">L’exemple suivant illustre ce processus.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-158">The following example shows this process.</span></span> <span data-ttu-id="b0aaa-159">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-159">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<span data-ttu-id="b0aaa-160"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="b0aaa-160"></span></span>

## <a name="get-a-user-photo-by-using-ews"></a><span data-ttu-id="b0aaa-161">Obtenir une photo de l’utilisateur à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="b0aaa-161">Get a user photo by using EWS</span></span>

<span data-ttu-id="b0aaa-162">Si vous recevez une photo de l’utilisateur de domaine Active Directory, vous pouvez utiliser l’opération [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (si vous connaissez l’adresse de messagerie) ou [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (si vous ne connaissez pas l’adresse de messagerie).</span><span class="sxs-lookup"><span data-stu-id="b0aaa-162">If you're getting a user photo from AD DS, you can use the [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) operation (if you know the email address) or the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation (if you don't know the email address).</span></span> <span data-ttu-id="b0aaa-163">Si vous recevez une photo de l’utilisateur à partir d’un dossier contacts dans la boîte aux lettres, utilisez l’opération [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) suivie de l’opération [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b0aaa-163">If you're getting a user photo from a contacts folder in the mailbox, use the [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) operation followed by the [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="b0aaa-164">Dans les deux cas, la photo est renvoyée sous forme de chaîne codée en Base64 dans la réponse XML.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-164">In either case, the photo is returned as a Base64-encoded string in the XML response.</span></span> 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a><span data-ttu-id="b0aaa-165">Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de l’opération GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="b0aaa-165">Get a mailbox user photo by using the GetUserPhoto operation</span></span>

<span data-ttu-id="b0aaa-166">Utilisation de l’opération **GetUserPhoto** est simple.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-166">Using the **GetUserPhoto** operation is straightforward.</span></span> <span data-ttu-id="b0aaa-167">Dans la demande XML, spécifiez l’adresse de messagerie de l’utilisateur et la [taille de la photo](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) à renvoyer (dans l’élément [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ).</span><span class="sxs-lookup"><span data-stu-id="b0aaa-167">In the XML request, specify the email address of the user, and the [size of the photo](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) to return (in the [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) element).</span></span> <span data-ttu-id="b0aaa-168">L’exemple de requête XML suivant montre comment obtenir une photo pour Sadie Daniels 360 pixels de large par 360 pixels de haut.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-168">The following XML request example shows how to get a photo for Sadie Daniels that's 360 pixels wide by 360 pixels high.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="b0aaa-169">Voici la réponse XML.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-169">The following is the XML response.</span></span> <span data-ttu-id="b0aaa-170">La photo codé en Base64 est contenue dans l’élément [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (le contenu a été raccourci pour des raisons de lisibilité).</span><span class="sxs-lookup"><span data-stu-id="b0aaa-170">The Base64-encoded photo is contained in the [PictureData](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) element (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a><span data-ttu-id="b0aaa-171">Obtenir une photo d’utilisateur de boîte aux lettres à l’aide de l’opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="b0aaa-171">Get a mailbox user photo by using the ResolveNames operation</span></span>

<span data-ttu-id="b0aaa-172">Si vous ne connaissez pas l’adresse de messagerie de l’utilisateur pour lequel vous obtenez une photo, vous pouvez [utiliser l’opération ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) pour obtenir des candidats pour une correspondance possible.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-172">If you don't know the email address of the user for whom you are getting a photo, you can [use the ResolveNames operation](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) to get candidates for a possible match.</span></span> <span data-ttu-id="b0aaa-173">Si vous spécifiez « AllProperties » pour l’attribut **ContactDataShape** de l’élément [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) , une grande quantité de données, y compris les photos de l’utilisateur, s’afficheront pour chaque candidat.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-173">If you specify "AllProperties" for the **ContactDataShape** attribute of the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) element, a lot of data, including user photos, will be returned for each candidate.</span></span> <span data-ttu-id="b0aaa-174">L’exemple suivant montre la demande XML pour résoudre le nom « Sadie » et de renvoyer toutes les propriétés pour chaque candidat.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-174">The following example shows the XML request to resolve the name "Sadie" and return all the properties for each candidate.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b0aaa-175">Une grande quantité de données s’afficheront dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-175">A lot of data will be returned in the response.</span></span> <span data-ttu-id="b0aaa-176">L’exemple suivant montre uniquement les données relatives à la photo de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-176">The following example shows only the data that is relevant to the user photo.</span></span> <span data-ttu-id="b0aaa-177">L’élément **Photo** contient la photo d’utilisateur codé en Base64 (le contenu a été raccourci pour des raisons de lisibilité).</span><span class="sxs-lookup"><span data-stu-id="b0aaa-177">The **Photo** element contains the Base64-encoded user photo (the content has been shortened for readability).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a><span data-ttu-id="b0aaa-178">Obtenir une photo de contacter l’utilisateur à l’aide de l’opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="b0aaa-178">Get a contact user photo by using the GetAttachment operation</span></span>

<span data-ttu-id="b0aaa-179">Vous pouvez utiliser EWS pour obtenir les photos des contacts stockés dans votre boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-179">You can use EWS to get photos from contacts stored in your mailbox.</span></span> <span data-ttu-id="b0aaa-180">Tout d’abord, vous utilisez l’opération **GetItem** pour renvoyer toutes les propriétés afin de vous permet de rechercher des photos.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-180">First, you use the **GetItem** operation to return all properties so you can look for photos.</span></span> <span data-ttu-id="b0aaa-181">L’exemple suivant montre une requête XML pour obtenir un élément de contact.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-181">The following example shows an XML request to get a contact item.</span></span> <span data-ttu-id="b0aaa-182">L’ID d’élément a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-182">The item ID has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="b0aaa-183">Recherchez l’élément [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) vérifier que le contact dispose d’une photo associée.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-183">Look for the [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) element to verify that the contact has an associated photo.</span></span> <span data-ttu-id="b0aaa-184">Recherchez par le biais de la collection de pièces jointes celui qui possède la valeur true pour l’élément [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="b0aaa-184">Then look through the collection of attachments for one that has a value of true for the [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="b0aaa-185">L’exemple suivant de la réponse n'indique que les données pertinentes.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-185">The following response example shows only the relevant data.</span></span> <span data-ttu-id="b0aaa-186">Les valeurs d’ID sont raccourcis pour améliorer la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-186">The ID values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

Ensuite, utilisez l’opération **GetAttachment** avec **AttachmentId** pour demander la pièce jointe ayant la photo du contact. L’exemple suivant montre la demande XML pour obtenir la pièce jointe. <span data-ttu-id="b0aaa-189">L’ID est réduite pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-189">The ID is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

L’exemple suivant montre la réponse XML avec les informations sur la pièce jointe que vous avez demandé. <span data-ttu-id="b0aaa-191">L’élément de [contenu](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) contient la chaîne codée en Base64 pour la photo de l’utilisateur, raccourcie dans cet exemple, pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-191">The [Content](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) element contains the Base64-encoded string for the user photo, shortened in this example for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="b0aaa-192"><a name="bk_EWS"> </a></span><span class="sxs-lookup"><span data-stu-id="b0aaa-192"></span></span>

## <a name="decode-a-base64-encoded-string"></a><span data-ttu-id="b0aaa-193">Décoder une chaîne codée en Base64</span><span class="sxs-lookup"><span data-stu-id="b0aaa-193">Decode a Base64-encoded string</span></span>

<span data-ttu-id="b0aaa-194">Quel que soit l’opération que vous permet d’obtenir une photo de l’utilisateur, vous devez décoder cette chaîne, vous pouvez l’utiliser dans votre application.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-194">Regardless of the operation you use to get a user photo, you'll need to decode that string so you can use it in your application.</span></span> <span data-ttu-id="b0aaa-195">L’exemple suivant montre comment décoder la chaîne et enregistrez-le sur votre ordinateur local afin de l’application vous pouvez y accéder ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="b0aaa-195">The following example shows how to decode the string, and then save it to your local computer so you application can access it later.</span></span>
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a><span data-ttu-id="b0aaa-196">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b0aaa-196">See also</span></span>

- [<span data-ttu-id="b0aaa-197">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b0aaa-197">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)    
- [<span data-ttu-id="b0aaa-198">Résoudre des noms ambigus en utilisant EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b0aaa-198">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [<span data-ttu-id="b0aaa-199">Contacts processus par lots à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b0aaa-199">Process contacts in batches by using EWS in Exchange</span></span>](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

