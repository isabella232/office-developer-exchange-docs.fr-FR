---
title: Acheminer les demandes de hiérarchie de dossiers publics
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Toutes les demandes d’informations de dossier public nécessitant des connaissances de la hiérarchie de dossiers publics, telles que le transfert, la mise à jour, la suppression ou la recherche de dossiers publics, doivent être routées vers la boîte aux lettres de hiérarchie de dossiers publics par défaut pour l’utilisateur donné. Pour acheminer les demandes vers cette boîte aux lettres, vous devez définir les en-têtes X-AnchorMailbox et X-PublicFolderMailbox sur des valeurs spécifiques renvoyées par le service de découverte automatique.
ms.openlocfilehash: 2773aa3ab29868c69d1fb088deb6c8a96dfb9ecc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455705"
---
# <a name="route-public-folder-hierarchy-requests"></a><span data-ttu-id="cf0ce-104">Acheminer les demandes de hiérarchie de dossiers publics</span><span class="sxs-lookup"><span data-stu-id="cf0ce-104">Route public folder hierarchy requests</span></span>

<span data-ttu-id="cf0ce-105">Toutes les demandes d’informations de dossier public nécessitant des connaissances de la hiérarchie de dossiers publics, telles que le transfert, la mise à jour, la suppression ou la recherche de dossiers publics, doivent être routées vers la boîte aux lettres de hiérarchie de dossiers publics par défaut pour l’utilisateur donné.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-105">All requests for public folder information that require knowledge of the public folder hierarchy, such as moving, updating, deleting, or finding public folders, need to be routed to the default public folder hierarchy mailbox for the given user.</span></span> <span data-ttu-id="cf0ce-106">Pour acheminer les demandes vers cette boîte aux lettres, vous devez définir les en-têtes **x-AnchorMailbox** et **x-PublicFolderMailbox** sur des valeurs spécifiques renvoyées par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values returned by the Autodiscover service.</span></span> 
  
<span data-ttu-id="cf0ce-107">**Vue d’ensemble des dossiers publics**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-107">**Overview of public folders**</span></span>

|<span data-ttu-id="cf0ce-108">En-tête</span><span class="sxs-lookup"><span data-stu-id="cf0ce-108">Header</span></span>|<span data-ttu-id="cf0ce-109">De quoi ai-je besoin ?</span><span class="sxs-lookup"><span data-stu-id="cf0ce-109">What do I need?</span></span>|<span data-ttu-id="cf0ce-110">Comment puis-je l’obtenir ?</span><span class="sxs-lookup"><span data-stu-id="cf0ce-110">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cf0ce-111">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-111">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="cf0ce-112">Valeur [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) d’une réponse SOAP de découverte automatique [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) , qui devient la valeur de l’en-tête **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-112">The [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) value from a [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) Autodiscover SOAP response, which becomes the value of the **X-AnchorMailbox** header.</span></span><br/><br/> <span data-ttu-id="cf0ce-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span><span class="sxs-lookup"><span data-stu-id="cf0ce-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span></span>| <span data-ttu-id="cf0ce-114">1. envoyez une demande **GetUserSetting** avec l’adresse SMTP de la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-114">1. Send a **GetUserSetting** request with the SMTP address for the user's mailbox.</span></span><br/><br/><span data-ttu-id="cf0ce-115">2. mettre en cache la valeur de l’élément **PublicFolderInformation** renvoyé par le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-115">2. Cache the value of the **PublicFolderInformation** element that the Autodiscover service returns.</span></span> <span data-ttu-id="cf0ce-116">Cela peut être mis en cache à partir d’un appel de découverte automatique existant dans votre code ou d’un nouvel [appel GetUserSettings d’API managée EWS](#bk_getpfinfoewsma) ou d’une [requête SOAP GetUserSettings](#bk_getpfinfoews).</span><span class="sxs-lookup"><span data-stu-id="cf0ce-116">This can be a cached from an existing Autodiscover call in your code, or a new [EWS Managed API GetUserSettings call](#bk_getpfinfoewsma) or a [GetUserSettings SOAP request](#bk_getpfinfoews).</span></span>  <br/><br/><span data-ttu-id="cf0ce-117">3. Utilisez l’élément **PublicFolderInformation** pour renseigner la valeur de l’en-tête **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-117">3. Use the **PublicFolderInformation** element to populate the value of the **X-AnchorMailbox** header.</span></span> <span data-ttu-id="cf0ce-118">La valeur de l’élément **PublicFolderInformation** est une adresse SMTP.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-118">The value of the **PublicFolderInformation** element is an SMTP address.</span></span>  <br/> |
|<span data-ttu-id="cf0ce-119">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-119">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="cf0ce-120">Valeur de [serveur](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) d’une [réponse de découverte automatique pox](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx)qui devient la valeur de l’en-tête **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-120">The [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) value from a [POX Autodiscover response](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx), which becomes the value of the **X-PublicFolderMailbox** header.</span></span><br/><br/> <span data-ttu-id="cf0ce-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span><span class="sxs-lookup"><span data-stu-id="cf0ce-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span></span>|<span data-ttu-id="cf0ce-122">1. [appelez le service de découverte automatique pox](#bk_makeautodrequest) à l’aide de l’adresse de messagerie **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-122">1. [Call the POX Autodiscover](#bk_makeautodrequest) service using the **X-AnchorMailbox** email address.</span></span>  <br/><br/><span data-ttu-id="cf0ce-123">2. Utilisez l’élément **serveur** renvoyé par le service de découverte automatique pour renseigner la valeur de l’en-tête **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-123">2. Use the **Server** element returned by the Autodiscover service to populate the value of the **X-PublicFolderMailbox** header.</span></span> <span data-ttu-id="cf0ce-124">La valeur de **X-PublicFolderMailbox** est une adresse SMTP où le nom d’utilisateur est un GUID.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-124">The value of the **X-PublicFolderMailbox** is an SMTP address where the username is a GUID.</span></span>  <br/> |

<br/>

<span data-ttu-id="cf0ce-125">Une fois que vous avez déterminé les valeurs d’en-tête, incluez-les [lorsque vous effectuez des demandes de hiérarchie de dossiers publics](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="cf0ce-125">After you have determined the header values, include them [when you make public folder hierarchy requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="cf0ce-126">Les étapes décrites dans cet article sont spécifiques aux demandes de hiérarchie de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-126">The steps in this article are specific to public folder hierarchy requests.</span></span> <span data-ttu-id="cf0ce-127">Pour déterminer si votre requête est une hiérarchie de dossiers publics ou une demande de contenu, consultez la rubrique [Routing Public Folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span><span class="sxs-lookup"><span data-stu-id="cf0ce-127">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a><span data-ttu-id="cf0ce-128">Déterminer la valeur de l’en-tête X-AnchorMailbox à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="cf0ce-128">Determine the value of the X-AnchorMailbox header by using the EWS Managed API</span></span>
<span data-ttu-id="cf0ce-129"><a name="bk_getpfinfoewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="cf0ce-129"><a name="bk_getpfinfoewsma"> </a></span></span>

<span data-ttu-id="cf0ce-130">Pour récupérer la valeur [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) à l’aide de l’API managée EWS, vous pouvez mettre en cache la valeur de l’élément **PublicFolderInformation** qu’un appel existant au service de découverte automatique renvoie ou effectuer un nouvel appel.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-130">To retrieve the [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) value by using the EWS Managed API, you can either cache the value of the **PublicFolderInformation** element that an existing call to the Autodiscover service returns, or make a new call.</span></span> 
  
<span data-ttu-id="cf0ce-131">Si vous effectuez un nouvel appel, vous pouvez [obtenir les paramètres utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[obtenir les paramètres utilisateur à l’aide de l’API managée EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) pour votre code, puis appeler l’exemple de méthode **GetUserSettings** à l’aide du code suivant, qui récupère uniquement la valeur de l’élément **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-131">If you're making a new call, you can [Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) to your code, and then call the **GetUserSettings** sample method by using the following code, which retrieves only the value of the **PublicFolderInformation** element.</span></span> <span data-ttu-id="cf0ce-132">Incluez l’adresse SMTP de l’utilisateur de boîte aux lettres en tant que paramètre d’entrée.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-132">Include the SMTP address of the mailbox user as an input parameter.</span></span> 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

<span data-ttu-id="cf0ce-133">Après avoir exécuté le code, les informations suivantes s’affichent dans la console :</span><span class="sxs-lookup"><span data-stu-id="cf0ce-133">After running the code, the following information is displayed on the console:</span></span>
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

<span data-ttu-id="cf0ce-134">Maintenant que vous avez la valeur **PublicFolderInformation** , incluez-la comme valeur pour l’en-tête X-AnchorMailbox dans toutes les demandes de hiérarchie de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-134">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a><span data-ttu-id="cf0ce-135">Déterminer la valeur de l’en-tête X-AnchorMailbox à l’aide de SOAP</span><span class="sxs-lookup"><span data-stu-id="cf0ce-135">Determine the value of the X-AnchorMailbox header using SOAP</span></span>
<span data-ttu-id="cf0ce-136"><a name="bk_getpfinfoews"> </a></span><span class="sxs-lookup"><span data-stu-id="cf0ce-136"><a name="bk_getpfinfoews"> </a></span></span>

<span data-ttu-id="cf0ce-137">L’exemple de code suivant montre comment récupérer la valeur **PublicFolderInformation** à l’aide de l’opération SOAP [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-137">The following code example shows how to retrieve the **PublicFolderInformation** value by using the [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) SOAP operation.</span></span> <span data-ttu-id="cf0ce-138">L’utilisateur de boîte aux lettres est spécifié dans l’élément [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) et l’élément [RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) limite la réponse à la valeur [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-138">The mailbox user is specified in the [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) element, and the [RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) element limits the response to the [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) value.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="cf0ce-139">La réponse inclut la valeur **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-139">The response includes the **PublicFolderInformation** value.</span></span> 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

<span data-ttu-id="cf0ce-140">Maintenant que vous avez la valeur **PublicFolderInformation** , incluez-la comme valeur pour l’en-tête X-AnchorMailbox dans toutes les demandes de hiérarchie de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-140">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a><span data-ttu-id="cf0ce-141">Effectuer une demande de découverte automatique pour déterminer la valeur X-PublicFolderInformation</span><span class="sxs-lookup"><span data-stu-id="cf0ce-141">Make an Autodiscover request to determine the X-PublicFolderInformation value</span></span>
<span data-ttu-id="cf0ce-142"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="cf0ce-142"><a name="bk_makeautodrequest"> </a></span></span>

<span data-ttu-id="cf0ce-143">Effectuez une demande de découverte automatique à l’aide de l’adresse SMTP **PublicFolderInformation** , qui est maintenant utilisée en tant que valeur **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-143">Make an Autodiscover request by using the **PublicFolderInformation** SMTP address, which is now being used as the **X-AnchorMailbox** value.</span></span> <span data-ttu-id="cf0ce-144">Utilisez l’exemple de code [Exchange 2013 : Get User Settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) pour appeler le service de découverte automatique, car il simplifie le processus de découverte automatique pour vous.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-144">Use the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="cf0ce-145">Cet exemple de code utilise les arguments de ligne de commande présentés dans le tableau suivant pour appeler le service de découverte automatique POX sur l’adresse SMTP **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-145">This code sample uses the command line arguments listed in the following table to call the POX Autodiscover service on the **PublicFolderInformation** SMTP address.</span></span> 
  
|<span data-ttu-id="cf0ce-146">**Argument de ligne de commande**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-146">**Command-line argument**</span></span>|<span data-ttu-id="cf0ce-147">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-147">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cf0ce-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cf0ce-148">emailAddress</span></span>  <br/> |<span data-ttu-id="cf0ce-149">L’adresse SMTP **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-149">The **PublicFolderInformation** SMTP address.</span></span>  <br/> |
|<span data-ttu-id="cf0ce-150">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="cf0ce-150">-skipSOAP</span></span>  <br/> | <span data-ttu-id="cf0ce-151">Utilisez les requêtes de découverte automatique POX pour ce scénario.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-151">Use POX Autodiscover requests for this scenario.</span></span>  <br/> |
|<span data-ttu-id="cf0ce-152">-authEmailAddress auth</span><span class="sxs-lookup"><span data-stu-id="cf0ce-152">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="cf0ce-153">L’adresse de messagerie de l’utilisateur de la boîte aux lettres, qui est utilisée pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-153">The mailbox user's email address, which is used for authentication.</span></span> <span data-ttu-id="cf0ce-154">Vous serez invité à entrer le mot de passe de l’utilisateur de boîte aux lettres lors de l’exécution de l’exemple.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-154">You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="cf0ce-155">Par exemple, quand SharedPublicFolder@contoso.com est l’adresse SMTP de l’élément **PublicFolderInformation** et sonyaf@contoso.com est l’utilisateur de boîte aux lettres, les arguments de ligne de commande doivent ressembler à ce qui suit.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-155">For example, when SharedPublicFolder@contoso.com is the SMTP address of the **PublicFolderInformation** element, and sonyaf@contoso.com is the mailbox user, the command-line arguments should look like this.</span></span> 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="cf0ce-156">Lorsque vous exécutez l’exemple de code **Exchange 2013 : Get User Settings with Autodiscover** , la dernière réponse de découverte automatique doit réussir et inclure tous les paramètres utilisateur associés au GUID de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-156">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="cf0ce-157">La valeur de [serveur](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) associée à l’élément de[type](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) de [protocole](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)Exch est la valeur d’en-tête **X-PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-157">The [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) value associated with the EXCH [Protocol](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)[Type](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) element is the **X-PublicFolderInformation** header value.</span></span> 
  
```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

<span data-ttu-id="cf0ce-158">Par ailleurs, si vous ne souhaitez pas utiliser l’exemple **Exchange 2013 : Get User Settings with Autodiscover** , vous pouvez obtenir la valeur du **serveur** en [générant une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md), puis en envoyant la demande de découverte automatique pox suivante à chaque URL jusqu’à ce que vous obteniez une réponse réussie.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-158">Alternatively, if you do not want to use the **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **Server** value by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span> <span data-ttu-id="cf0ce-159">SharedPublicFolder@contoso.com est la valeur de l’en-tête **X-PublicFolderMailbox** .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-159">SharedPublicFolder@contoso.com is the value of the **X-PublicFolderMailbox** header.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="cf0ce-160">Pour plus d’informations sur le processus de découverte automatique, voir [Autodiscover pour Exchange](autodiscover-for-exchange.md), [générer une liste des points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)et [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de la découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span><span class="sxs-lookup"><span data-stu-id="cf0ce-160">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="cf0ce-161">Définir les valeurs des en-têtes X-AnchorMailbox et X-PublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="cf0ce-161">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="cf0ce-162"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="cf0ce-162"><a name="bk_setheadervalues"> </a></span></span>

<span data-ttu-id="cf0ce-163">En utilisant la valeur de l’adresse SMTP **PublicFolderInformation** acquise dans [determine la valeur de l’en-tête x-AnchorMailbox à l’aide de l’API managée EWS](#bk_getpfinfoewsma) ou en [déterminant la valeur de l’en-tête x-ANCHORMAILBOX à l’aide de SOAP](#bk_getpfinfoews) **, ainsi que** la valeur du **serveur** acquise dans la **demande de** [découverte automatique pour déterminer la valeur x-PublicFolderInformation](#bk_makeautodrequest)</span><span class="sxs-lookup"><span data-stu-id="cf0ce-163">Using the value of the **PublicFolderInformation** SMTP address acquired in [Determine the value of the X-AnchorMailbox header by using the EWS Managed API](#bk_getpfinfoewsma) or [Determine the value of the X-AnchorMailbox header using SOAP](#bk_getpfinfoews) and the **Server** value acquired in [Make an Autodiscover request to determine the X-PublicFolderInformation value](#bk_makeautodrequest), set the values of **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="cf0ce-164">Par exemple, étant donné une adresse SMTP **PublicFolderInformation** de SharedPublicFolder@contoso.com et une valeur de **serveur** de 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, incluez les en-têtes suivants lors de l’appel aux méthodes ou opérations suivantes.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-164">For example, given a **PublicFolderInformation** SMTP address of SharedPublicFolder@contoso.com and a **Server** value of 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, include the following headers when making calls to the following methods or operations.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

<span data-ttu-id="cf0ce-165">**Appels de dossier public nécessitant les en-têtes X-AnchorMailbox et X-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-165">**Public folder calls that require the X-AnchorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="cf0ce-166">**Méthodes d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-166">**EWS Managed API methods**</span></span>|<span data-ttu-id="cf0ce-167">**Opérations EWS**</span><span class="sxs-lookup"><span data-stu-id="cf0ce-167">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf0ce-168">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="cf0ce-168">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="cf0ce-169">Folder. Delete</span><span class="sxs-lookup"><span data-stu-id="cf0ce-169">Folder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="cf0ce-170">Folder. Update</span><span class="sxs-lookup"><span data-stu-id="cf0ce-170">Folder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="cf0ce-171">Folder. Move</span><span class="sxs-lookup"><span data-stu-id="cf0ce-171">Folder.Move</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="cf0ce-172">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="cf0ce-172">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="cf0ce-173">FindFolder</span><span class="sxs-lookup"><span data-stu-id="cf0ce-173">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="cf0ce-174">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="cf0ce-174">DeleteFolder</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [<span data-ttu-id="cf0ce-175">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="cf0ce-175">UpdateFolder</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [<span data-ttu-id="cf0ce-176">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="cf0ce-176">MoveFolder</span></span>](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="cf0ce-177">Pour ajouter ces en-têtes à l’aide de l’API managée EWS, utilisez la méthode [HttpHeaders. Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="cf0ce-177">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

<span data-ttu-id="cf0ce-178">Par exemple, le code suivant montre une requête [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) avec l’en-tête **x-AnchorMailbox** et **x-PublicFolderMailbox** défini sur les valeurs récupérées dans les exemples de cet article.</span><span class="sxs-lookup"><span data-stu-id="cf0ce-178">For example, the following code shows a [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="cf0ce-179">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf0ce-179">See also</span></span>

- [<span data-ttu-id="cf0ce-180">Accéder aux dossiers publics avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cf0ce-180">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="cf0ce-181">Acheminer les demandes de contenu de dossier public</span><span class="sxs-lookup"><span data-stu-id="cf0ce-181">Route public folder content requests</span></span>](how-to-route-public-folder-content-requests.md)    
- [<span data-ttu-id="cf0ce-182">Obtenir les paramètres utilisateur à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="cf0ce-182">Get user settings by using the EWS Managed API</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

