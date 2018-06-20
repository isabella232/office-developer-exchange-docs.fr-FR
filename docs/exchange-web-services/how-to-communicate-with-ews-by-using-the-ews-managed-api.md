---
title: Communiquer avec EWS à l’aide de l’API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Trouvez des informations sur l’utilisation de l’API managée EWS pour communiquer avec EWS dans Exchange.
ms.openlocfilehash: 773fcc3f7e95d25effb5a686d4b79ec22610df8c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754821"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a><span data-ttu-id="be59b-103">Communiquer avec EWS à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="be59b-103">Communicate with EWS by using the EWS Managed API</span></span>

<span data-ttu-id="be59b-104">Trouvez des informations sur l’utilisation de l’API managée EWS pour communiquer avec EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="be59b-104">Find information about how to use the EWS Managed API to communicate with EWS in Exchange.</span></span>
  
<span data-ttu-id="be59b-105">La classe [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) dans l’API managée EWS contient les méthodes et propriétés que vous utilisez pour définir les informations d’identification utilisateur, identifier le point de terminaison EWS, envoyer et recevoir des messages SOAP et configurer la liaison de communiquer avec EWS.</span><span class="sxs-lookup"><span data-stu-id="be59b-105">The [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the EWS Managed API contains the methods and properties that you use to set user credentials, identify the EWS endpoint, send and receive SOAP messages, and configure the binding to communicate with EWS.</span></span> <span data-ttu-id="be59b-106">Avant de pouvoir utiliser l’API managée EWS pour accomplir une tâche, vous devez créer une instance de la classe **ExchangeService** et le lier à EWS.</span><span class="sxs-lookup"><span data-stu-id="be59b-106">Before you can use the EWS Managed API to perform any task, you have to create an instance of the **ExchangeService** class and bind it to EWS.</span></span> 
  
<span data-ttu-id="be59b-107">Après avoir configuré un objet [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) avec les informations d’identification utilisateur et le point de terminaison EWS, n’importe quel objet boîte aux lettres qui fait référence à l’objet [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) peut utiliser les types suivants de la méthode pour communiquer avec EWS :</span><span class="sxs-lookup"><span data-stu-id="be59b-107">After you set up an [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) object with user credentials and the EWS endpoint, any mailbox object that references the [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) object can use the following method types to communicate with EWS:</span></span> 
  
- <span data-ttu-id="be59b-108">Méthodes de l’objet ExchangeService — toutes les méthodes de l’objet **ExchangeService** qui ne sont pas héritées le type **d’objet** base appeler EWS.</span><span class="sxs-lookup"><span data-stu-id="be59b-108">ExchangeService object methods — All the methods on the **ExchangeService** object that are not inherited from the base **Object** type make calls to EWS.</span></span> 
    
- <span data-ttu-id="be59b-109">Élément de boîte aux lettres Exchange et dossier type de méthodes.</span><span class="sxs-lookup"><span data-stu-id="be59b-109">Exchange mailbox item and folder type methods.</span></span>
    
<span data-ttu-id="be59b-110">**Le tableau 1. Élément de boîte aux lettres et de dossiers tapez méthodes qui communiquent avec EWS**</span><span class="sxs-lookup"><span data-stu-id="be59b-110">**Table 1. Mailbox item and folder type methods that communicate with EWS**</span></span>

|<span data-ttu-id="be59b-111">Méthode</span><span class="sxs-lookup"><span data-stu-id="be59b-111">Method</span></span>|<span data-ttu-id="be59b-112">Fonction</span><span class="sxs-lookup"><span data-stu-id="be59b-112">What it does</span></span>|<span data-ttu-id="be59b-113">Opérations qu’elle appelle</span><span class="sxs-lookup"><span data-stu-id="be59b-113">Operations that it calls</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="be59b-114">Load</span><span class="sxs-lookup"><span data-stu-id="be59b-114">Load</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="be59b-115">Obtient les propriétés sur un objet de configuration utilisateur, pièces jointes ou élément.</span><span class="sxs-lookup"><span data-stu-id="be59b-115">Gets properties on an item, attachment, or user configuration object.</span></span>  <br/> |[<span data-ttu-id="be59b-116">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="be59b-116">GetItem operation</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="be59b-117">Opération GetAttachment</span><span class="sxs-lookup"><span data-stu-id="be59b-117">GetAttachment operation</span></span>](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="be59b-118">Opération GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="be59b-118">GetUserConfiguration operation</span></span>](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="be59b-119">Créer une liaison</span><span class="sxs-lookup"><span data-stu-id="be59b-119">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="be59b-120">Remplit un nouvel élément sur le client avec des informations à partir d’un élément existant sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="be59b-120">Populates a new item on the client with information from an existing item on the server.</span></span>  <br/> |[<span data-ttu-id="be59b-121">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="be59b-121">GetItem operation</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="be59b-122">Save</span><span class="sxs-lookup"><span data-stu-id="be59b-122">Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="be59b-123">Enregistre la copie de l’élément client sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="be59b-123">Saves the copy of the client item on the server.</span></span>  <br/> |[<span data-ttu-id="be59b-124">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="be59b-124">UpdateItem operation</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="be59b-125">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="be59b-125">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[<span data-ttu-id="be59b-126">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="be59b-126">CreateItem operation</span></span>](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[<span data-ttu-id="be59b-127">Opération CreateFolder</span><span class="sxs-lookup"><span data-stu-id="be59b-127">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="be59b-128">Mettre à jour</span><span class="sxs-lookup"><span data-stu-id="be59b-128">Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="be59b-129">Met à jour le serveur avec les modifications effectuées sur le client.</span><span class="sxs-lookup"><span data-stu-id="be59b-129">Updates the server with the changes made on the client.</span></span><br/><br/><span data-ttu-id="be59b-130">Pour les éléments et les dossiers, la méthode de **mise à jour** utilise l' [opération UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) et l' [opération UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="be59b-130">For items and folders, the **Update** method uses the [UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) and the [UpdateFolder operation](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).</span></span>  <br/> |[<span data-ttu-id="be59b-131">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="be59b-131">UpdateItem operation</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[<span data-ttu-id="be59b-132">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="be59b-132">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="be59b-133">Supprimer</span><span class="sxs-lookup"><span data-stu-id="be59b-133">Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="be59b-134">Supprime un élément sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="be59b-134">Deletes an item on the server.</span></span><br/><br/><span data-ttu-id="be59b-135">Pour les éléments et les dossiers, la méthode **Delete** utilise l' [opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="be59b-135">For items and folders, the **Delete** method uses the and the [DeleteFolder operation](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).</span></span>  <br/> |[<span data-ttu-id="be59b-136">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="be59b-136">DeleteItem operation</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="be59b-137">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="be59b-137">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="be59b-138">Copier</span><span class="sxs-lookup"><span data-stu-id="be59b-138">Copy</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="be59b-139">Crée une copie de l’élément ou les dossiers sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="be59b-139">Creates a copy of the item or folders on the server.</span></span>  <br/> |[<span data-ttu-id="be59b-140">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="be59b-140">CopyItem operation</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="be59b-141">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="be59b-141">CopyFolder operation</span></span>](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="be59b-142">Déplacer</span><span class="sxs-lookup"><span data-stu-id="be59b-142">Move</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="be59b-143">Déplace les éléments ou des dossiers sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="be59b-143">Moves items or folders on the server.</span></span>  <br/> |[<span data-ttu-id="be59b-144">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="be59b-144">MoveItem operation</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [<span data-ttu-id="be59b-145">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="be59b-145">MoveFolder operation</span></span>](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a><span data-ttu-id="be59b-146">Pour utiliser l’API managée EWS pour communiquer avec EWS</span><span class="sxs-lookup"><span data-stu-id="be59b-146">To use the EWS Managed API to communicate with EWS</span></span>

1. <span data-ttu-id="be59b-147">Instanciez la classe **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="be59b-147">Instantiate the **ExchangeService** class.</span></span> 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > <span data-ttu-id="be59b-148">L’instanciation de **ExchangeService** avec un constructeur vide créera une instance qui est liée à la dernière version connue d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="be59b-148">Instantiating **ExchangeService** with an empty constructor will create an instance that is bound to the latest known version of Exchange.</span></span> <span data-ttu-id="be59b-149">Vous pouvez également cibler une version spécifique d’Exchange en spécifiant la version en tant que paramètre.</span><span class="sxs-lookup"><span data-stu-id="be59b-149">Alternatively, you can target a specific version of Exchange by specifying version as a parameter.</span></span> `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. <span data-ttu-id="be59b-150">Définir les informations d’identification de l’utilisateur qui envoie des requêtes sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="be59b-150">Set the credentials of the user who sends requests to the Exchange server.</span></span> <span data-ttu-id="be59b-151">Si vous souhaitez vous connecter à EWS depuis un ordinateur qui est connecté au domaine, les informations d’identification de l’utilisateur authentifié, définissez la propriété **UseDefaultCredentials** sur l’objet **ExchangeService** sur **true**.</span><span class="sxs-lookup"><span data-stu-id="be59b-151">If you want to connect to EWS from a computer that is logged on to the domain, using the credentials of the authenticated user, set the **UseDefaultCredentials** property on the **ExchangeService** object to **true**.</span></span>
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   <span data-ttu-id="be59b-152">Si vous ne souhaitez pas vous connecter en utilisant les informations d’identification des utilisateurs par défaut, définissez la propriété **d’informations d’identification** sur l’objet **ExchangeService** spécifier de manière explicite les informations d’identification d’un autre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="be59b-152">If you do not want to connect by using the default user credentials, set the **Credentials** property on the **ExchangeService** object to explicitly specify the credentials of a different user.</span></span> <span data-ttu-id="be59b-153">Si vous utilisez Exchange Online ou Exchange Online dans le cadre d’Office 365, vous allez utiliser l’authentification de base, avec uniquement un nom d’utilisateur et un mot de passe.</span><span class="sxs-lookup"><span data-stu-id="be59b-153">If you are using Exchange Online or Exchange Online as part of Office 365, you'll use basic authentication, with just a user name and password.</span></span> <span data-ttu-id="be59b-154">Un nom de domaine est requis pour l’authentification NTLM.</span><span class="sxs-lookup"><span data-stu-id="be59b-154">A domain name is required for NTLM authentication.</span></span> 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   <span data-ttu-id="be59b-155">Vous pouvez également spécifier les informations d’identification de l’utilisateur à l’aide de nom de domaine de l’utilisateur et le mot de passe.</span><span class="sxs-lookup"><span data-stu-id="be59b-155">You can also specify the credentials of the user by using the user's domain name and password.</span></span>
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > <span data-ttu-id="be59b-156">Si la propriété **UseDefaultCredentials** est définie sur **true**, la valeur de la propriété **Credentials** est ignorée.</span><span class="sxs-lookup"><span data-stu-id="be59b-156">If the **UseDefaultCredentials** property is set to **true**, the value of the **Credentials** property is ignored.</span></span> 
  
3. <span data-ttu-id="be59b-157">Définir l’URL du point de terminaison EWS.</span><span class="sxs-lookup"><span data-stu-id="be59b-157">Set the URL of the EWS endpoint.</span></span> <span data-ttu-id="be59b-158">Cette URL localise le fichier exchange.asmx sur le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="be59b-158">This URL locates the exchange.asmx file on Client Access server.</span></span>
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  <span data-ttu-id="be59b-159">Vous pouvez définir explicitement la propriété **Url** de **ExchangeService** sur une valeur codée en dur, nous vous recommandons d’utiliser le service de découverte automatique au lieu de cela, pour les raisons suivantes : > découverte automatique détermine le point de terminaison meilleures pour un utilisateur donné (le point de terminaison le plus proche de serveur de boîtes aux lettres de l’utilisateur).</span><span class="sxs-lookup"><span data-stu-id="be59b-159">Although you can explicitly set the **Url** property of the **ExchangeService** to a hardcoded value, we recommend that you use the Autodiscover service instead, for the following reasons: >  Autodiscover determines the best endpoint for a given user (the endpoint that is closest to the user's Mailbox server).</span></span> <span data-ttu-id="be59b-160">> L’URL EWS peut changer si les nouveaux serveurs d’accès au Client sont déployés.</span><span class="sxs-lookup"><span data-stu-id="be59b-160">>  The EWS URL might change if new Client Access servers are deployed.</span></span> <span data-ttu-id="be59b-161">Dans ce scénario, l’utilisation [d’Autodiscover](autodiscover-for-exchange.md) signifie qu'aucune modification de code n’est nécessaires.</span><span class="sxs-lookup"><span data-stu-id="be59b-161">In this scenario, using [Autodiscover](autodiscover-for-exchange.md) means no code changes are necessary.</span></span> <span data-ttu-id="be59b-162">> Vous devez définir l’URL de manière explicite ou appel **AutodiscoverUrl**, mais vous ne devez pas effectuer les deux.</span><span class="sxs-lookup"><span data-stu-id="be59b-162">>  You should either set the URL explicitly or call **AutodiscoverUrl**, but you should not do both.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="be59b-163">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="be59b-163">See also</span></span>

- [<span data-ttu-id="be59b-164">Prise en main des applications clientes d'API managée EWS</span><span class="sxs-lookup"><span data-stu-id="be59b-164">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md) 
- [<span data-ttu-id="be59b-165">Utiliser la découverte automatique pour rechercher les points de connexion</span><span class="sxs-lookup"><span data-stu-id="be59b-165">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)   
- [<span data-ttu-id="be59b-166">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="be59b-166">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
