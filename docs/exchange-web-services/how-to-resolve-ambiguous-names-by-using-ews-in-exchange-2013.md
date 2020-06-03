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
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a><span data-ttu-id="40bcd-103">Résoudre des noms ambigus à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="40bcd-103">Resolve ambiguous names by using EWS in Exchange 2013</span></span>

<span data-ttu-id="40bcd-104">Découvrez comment utiliser l’API managée EWS ou EWS pour résoudre des noms ambigus en obtenant les correspondances possibles des services de domaine Active Directory (AD DS) ou d’un dossier de contacts dans la boîte aux lettres de votre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="40bcd-104">Learn how to use the EWS Managed API or EWS to resolve ambiguous names by getting possible matches from Active Directory Domain Services (AD DS) or a contacts folder in your user's mailbox.</span></span>
  
<span data-ttu-id="40bcd-105">Un utilisateur de votre organisation reçoit une liste manuscrite de noms et d’adresses pour les employés qui ont participé à une session de formation.</span><span class="sxs-lookup"><span data-stu-id="40bcd-105">A user in your organization is given a hand-written list of names and addresses for employees that attended a training session.</span></span> <span data-ttu-id="40bcd-106">Ils veulent envoyer un courrier électronique contenant des informations supplémentaires à des personnes figurant dans la liste, mais ils ne peuvent pas lire l’adresse de messagerie de tous les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="40bcd-106">They want to send an email with some additional information to people on the list, but they can't read everyone's email address.</span></span> <span data-ttu-id="40bcd-107">Si vous souhaitez résoudre ce problème pour vos utilisateurs dans votre application, EWS peut vous aider.</span><span class="sxs-lookup"><span data-stu-id="40bcd-107">If you want to solve this problem for your users in your application, EWS can help.</span></span> <span data-ttu-id="40bcd-108">Vous pouvez utiliser la méthode de l’API managée EWS [ExchangeService. ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) ou l’opération EWS [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) pour renvoyer une liste de correspondances potentielles pour une sélection de texte, telle qu’une partie d’un nom de famille.</span><span class="sxs-lookup"><span data-stu-id="40bcd-108">You can use the [ExchangeService.ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API method or the [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to return a list of potential matches for a selection of text, such as part of a last name.</span></span> <span data-ttu-id="40bcd-109">Les éléments renvoyés peuvent être des boîtes aux lettres utilisateur publiques, des groupes de distribution et des contacts.</span><span class="sxs-lookup"><span data-stu-id="40bcd-109">The returned items can be public user mailboxes, distribution groups, and contacts.</span></span> 
  
<span data-ttu-id="40bcd-110">Notez qu’Exchange enregistre les adresses de messagerie avec des types de routage préfixés, tels que SMTP ou SIP, dans un tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="40bcd-110">Note that Exchange saves email addresses with prefixed routing types, such as smtp or sip, in a multivalue array.</span></span> <span data-ttu-id="40bcd-111">La méthode **ResolveName** et l’opération **ResolveNames** effectuent une correspondance partielle par rapport à chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « SIP : utilisateur1 ».</span><span class="sxs-lookup"><span data-stu-id="40bcd-111">The **ResolveName** method and the **ResolveNames** operation perform a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1".</span></span> <span data-ttu-id="40bcd-112">Si vous ne spécifiez pas de type de routage, la méthode ou l’opération prend par défaut la valeur SMTP, la associe à une propriété d’adresse SMTP principale, et non à la recherche dans le tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="40bcd-112">If you don't specify a routing type, the method or operation will default to smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> <span data-ttu-id="40bcd-113">Par exemple, si vous recherchez Utilisateur1 et que vous n’incluez pas le préfixe SIP, vous ne recevrez pas sip :User1@Contoso.com comme résultat, même s’il s’agit d’une boîte aux lettres valide.</span><span class="sxs-lookup"><span data-stu-id="40bcd-113">For example, if you search for User1 and do not include the sip prefix, you will not receive sip:User1@Contoso.com as a result, even if that is a valid mailbox.</span></span> 
  
<span data-ttu-id="40bcd-114">Vous ne pouvez spécifier qu’un seul nom ambigu dans une seule demande.</span><span class="sxs-lookup"><span data-stu-id="40bcd-114">You can only specify one ambiguous name in a single request.</span></span> <span data-ttu-id="40bcd-115">Si vous avez une liste de noms ambigus à résoudre, vous devrez parcourir la liste et appeler la méthode ou l’opération pour chaque entrée.</span><span class="sxs-lookup"><span data-stu-id="40bcd-115">If you have a list of ambiguous names to resolve, you will need to loop through the list and call the method or operation for each entry.</span></span> <span data-ttu-id="40bcd-116">Les candidats du dossier de contacts d’un utilisateur auront une valeur d’ID d’élément non null, qui peut ensuite être utilisée dans un appel de méthode [contact. bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) ou une demande d’opération [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) pour extraire des informations supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="40bcd-116">Candidates from a user's Contacts folder will have a non-null item ID value, which can then be used in a [Contact.Bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) method call or [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request to retrieve additional information.</span></span> <span data-ttu-id="40bcd-117">Si le candidat est un groupe de distribution, vous pouvez utiliser la méthode de l’API managée EWS [expandgroup, (itemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) ou l’opération EWS [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) pour obtenir la liste des membres.</span><span class="sxs-lookup"><span data-stu-id="40bcd-117">If the candidate is a distribution group, you can use the [ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS operation to get the list of members.</span></span> <span data-ttu-id="40bcd-118">Si le paramètre _returnContactDetails_ ou l’attribut EWS **ReturnFullContactData** est défini sur true, les entrées Active Directory renvoyées via une méthode **ResolveName** ou **ResolveNames** incluent des propriétés supplémentaires qui décrivent le contact.</span><span class="sxs-lookup"><span data-stu-id="40bcd-118">If the  _returnContactDetails_ parameter or the **ReturnFullContactData** EWS attribute is set to true, Active Directory entries returned via a **ResolveName** method or **ResolveNames** operation will include additional properties that describe the contact.</span></span> <span data-ttu-id="40bcd-119">Le paramètre _returnContactDetails_ ou l’attribut **ReturnFullContactData** n’affecte pas les données renvoyées pour les contacts et les groupes de contacts.</span><span class="sxs-lookup"><span data-stu-id="40bcd-119">The  _returnContactDetails_ parameter or the **ReturnFullContactData** attribute does not affect the data that is returned for contacts and contact groups.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a><span data-ttu-id="40bcd-120">Résoudre les noms ambigus à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="40bcd-120">Resolve ambiguous names by using EWS Managed API</span></span>
<span data-ttu-id="40bcd-121"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="40bcd-121"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="40bcd-122">Vous pouvez utiliser la méthode [ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) pour rechercher les candidats qui correspondent au nom ambigu que vous transmettez.</span><span class="sxs-lookup"><span data-stu-id="40bcd-122">You can use the [ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) method to find candidates that match the ambiguous name you pass.</span></span> <span data-ttu-id="40bcd-123">Vous pouvez utiliser des surcharges de la méthode **ResolveName** pour rechercher des candidats de cinq manières différentes.</span><span class="sxs-lookup"><span data-stu-id="40bcd-123">You can use overloads of the **ResolveName** method to search for candidates in five different ways.</span></span> 
  
<span data-ttu-id="40bcd-124">**Tableau 1. Méthodes ResolveName surchargées**</span><span class="sxs-lookup"><span data-stu-id="40bcd-124">**Table 1. Overloaded ResolveName methods**</span></span>

|<span data-ttu-id="40bcd-125">**Méthode**</span><span class="sxs-lookup"><span data-stu-id="40bcd-125">**Method**</span></span>|<span data-ttu-id="40bcd-126">**Fonctionnement**</span><span class="sxs-lookup"><span data-stu-id="40bcd-126">**How it works**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40bcd-127">ResolveName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="40bcd-127">ResolveName(String)</span></span>](https://msdn.microsoft.com/library/dd635548%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40bcd-128">Recherche les contacts dans le dossier contacts de l’utilisateur et dans la liste d’adresses globale (LAG), dans cet ordre.</span><span class="sxs-lookup"><span data-stu-id="40bcd-128">Finds contacts in the user's Contacts folder and the Global Address List (GAL) — in that order.</span></span> <span data-ttu-id="40bcd-129">La variable de chaîne est le nom ambigu que vous tentez de résoudre.</span><span class="sxs-lookup"><span data-stu-id="40bcd-129">The string variable is the ambiguous name you are trying to resolve.</span></span>  <br/> |
|[<span data-ttu-id="40bcd-130">ResolveName (String, ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="40bcd-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span></span>](https://msdn.microsoft.com/library/dd634595%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40bcd-131">Recherche des contacts dans le dossier de contacts par défaut et/ou dans la liste d’adresses globale (LAG).</span><span class="sxs-lookup"><span data-stu-id="40bcd-131">Finds contacts in the default Contacts folder and/or the Global Address List (GAL).</span></span> <span data-ttu-id="40bcd-132">La valeur de chaîne est le nom ambigu, l’emplacement de recherche spécifie le dossier contacts et/ou la liste d’adresses globale, et la valeur booléenne indique s’il faut renvoyer les informations de contact complètes.</span><span class="sxs-lookup"><span data-stu-id="40bcd-132">The string value is the ambiguous name, the search location specifies the Contacts folder and/or the GAL, and the Boolean value indicates whether to return the full contact information.</span></span>  <br/> |
|[<span data-ttu-id="40bcd-133">ResolveName (String, ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="40bcd-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](https://msdn.microsoft.com/library/hh532803%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40bcd-134">Recherche des contacts dans le dossier de contacts par défaut et/ou dans la liste d’adresses globale (LAG).</span><span class="sxs-lookup"><span data-stu-id="40bcd-134">Finds contacts in the default Contacts folder and/or Global Address List (GAL).</span></span> <span data-ttu-id="40bcd-135">Cette méthode vous permet de définir les propriétés qui sont renvoyées.</span><span class="sxs-lookup"><span data-stu-id="40bcd-135">This method enables you to set the properties that are returned.</span></span>  <br/> |
|[<span data-ttu-id="40bcd-136">ResolveName (String, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="40bcd-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span></span>](https://msdn.microsoft.com/library/dd636014%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40bcd-137">Recherche des contacts dans les dossiers de contacts spécifiés et/ou dans la liste d’adresses globale (LAG).</span><span class="sxs-lookup"><span data-stu-id="40bcd-137">Finds contacts in specified contact folders and/or the Global Address List (GAL).</span></span> <span data-ttu-id="40bcd-138">Vous pouvez utiliser cette méthode pour transmettre une collection de dossiers à rechercher.</span><span class="sxs-lookup"><span data-stu-id="40bcd-138">You can use this method to pass a collection of folders to search.</span></span> <span data-ttu-id="40bcd-139">Cela vous permet de regarder dans des dossiers de contacts autres que le dossier de contacts par défaut.</span><span class="sxs-lookup"><span data-stu-id="40bcd-139">This enables you to look in contact folders other than the default Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="40bcd-140">ResolveName (String, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="40bcd-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](https://msdn.microsoft.com/library/hh532581%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40bcd-141">Recherche des contacts dans la liste d’adresses globale (LAG) et/ou dans des dossiers de contacts spécifiques.</span><span class="sxs-lookup"><span data-stu-id="40bcd-141">Finds contacts in the Global Address List (GAL) and/or in specific contact folders.</span></span> <span data-ttu-id="40bcd-142">Cette méthode vous permet de définir les propriétés qui sont renvoyées.</span><span class="sxs-lookup"><span data-stu-id="40bcd-142">This method enables you to set the properties that are returned.</span></span>  <br/> |
   
<span data-ttu-id="40bcd-143">Commençons par un exemple simple.</span><span class="sxs-lookup"><span data-stu-id="40bcd-143">Let's start with a simple example.</span></span> <span data-ttu-id="40bcd-144">L’exemple suivant montre comment résoudre la chaîne de texte « Dan » et générer le nom et l’adresse de messagerie de chaque candidat trouvé.</span><span class="sxs-lookup"><span data-stu-id="40bcd-144">The following example shows how to resolve the text string "dan" and output the name and email address of each candidate found.</span></span> <span data-ttu-id="40bcd-145">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="40bcd-145">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="40bcd-146">La réponse renvoie un maximum de 100 candidats, bien qu’il puisse y avoir plus de 100 candidats potentiels.</span><span class="sxs-lookup"><span data-stu-id="40bcd-146">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates.</span></span> <span data-ttu-id="40bcd-147">Pour déterminer si seuls les 100 premiers candidats d’un plus grand nombre de candidats ont été renvoyés, vérifiez la valeur de [IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) dans l’objet [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="40bcd-147">To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of [IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) in the [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="40bcd-148">Si la valeur est true, il n’y a pas de candidats possibles ; Si la valeur est false, la méthode renvoie uniquement le premier 100 d’un plus grand nombre de candidats potentiels.</span><span class="sxs-lookup"><span data-stu-id="40bcd-148">If the value is true, there are no more possible candidates; if the value is false, the method only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="40bcd-149">Si vous travaillez dans une grande organisation, il est probable qu’un nom tel que « Dan » renvoie le nombre maximal de candidats de 100.</span><span class="sxs-lookup"><span data-stu-id="40bcd-149">If you work in a large organization, it's likely that a name like "dan" will return the maximum number of 100 candidates.</span></span> <span data-ttu-id="40bcd-150">Pour réduire le nombre de candidats renvoyés, limitez l’emplacement de la recherche.</span><span class="sxs-lookup"><span data-stu-id="40bcd-150">To reduce the number of candidates returned, limit where you search.</span></span> <span data-ttu-id="40bcd-151">L’exemple suivant utilise l’énumération [ResolveNameSearchLocation](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) pour indiquer où Rechercher pour résoudre le nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="40bcd-151">The next example uses the [ResolveNameSearchLocation](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) enumeration to specify where to search to resolve the ambiguous name.</span></span> 
  
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

<span data-ttu-id="40bcd-152">Si vous stockez vos contacts dans un dossier autre que le dossier contacts bien connu, utilisez l’une des méthodes surchargées pour spécifier où rechercher les candidats.</span><span class="sxs-lookup"><span data-stu-id="40bcd-152">If you store your contacts in a folder other than the well-known Contacts folder, use one of the overloaded methods to specify where to look for candidates.</span></span> <span data-ttu-id="40bcd-153">L’exemple suivant crée une liste de dossiers pour la méthode **ResolveName** en fonction de l’ID de dossier.</span><span class="sxs-lookup"><span data-stu-id="40bcd-153">The following example creates a folder list for the **ResolveName** method based on the folder ID.</span></span> <span data-ttu-id="40bcd-154">Le **FolderId** a été raccourci pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="40bcd-154">The **FolderId** has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="40bcd-155">Si vous appliquez des filtres et qu’aucun candidat n’est renvoyé, le [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) ne contient aucune entrée.</span><span class="sxs-lookup"><span data-stu-id="40bcd-155">If you apply filters and no candidates are returned, the [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) will contain zero entries.</span></span> <span data-ttu-id="40bcd-156">Vous pouvez vérifier cela en examinant la propriété [Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) de la collection.</span><span class="sxs-lookup"><span data-stu-id="40bcd-156">You can verify this by looking at the [Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) property of the collection.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a><span data-ttu-id="40bcd-157">Résoudre des noms ambigus à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="40bcd-157">Resolve ambiguous names by using EWS</span></span>
<span data-ttu-id="40bcd-158"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="40bcd-158"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="40bcd-159">Vous pouvez utiliser l’opération EWS [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) pour identifier les candidats possibles pour un nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="40bcd-159">You can use the [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to identify possible candidates for an ambiguous name.</span></span> <span data-ttu-id="40bcd-160">L’élément [UnresolvedEntry](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) contient le nom ambigu à résoudre.</span><span class="sxs-lookup"><span data-stu-id="40bcd-160">The [UnresolvedEntry](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) element contains the ambiguous name you want to resolve.</span></span> <span data-ttu-id="40bcd-161">L’exemple suivant montre comment résoudre le nom Sadie.</span><span class="sxs-lookup"><span data-stu-id="40bcd-161">The following example shows how to resolve the name Sadie.</span></span> <span data-ttu-id="40bcd-162">Il s’agit également de la requête XML que l’API managée EWS utilise lorsque vous [Utilisez la méthode ResolveName](#bk_EWSMA), à la différence qu’elle utilise un autre nom pour les exemples de sortie valides.</span><span class="sxs-lookup"><span data-stu-id="40bcd-162">This is also the XML request that the EWS Managed API uses when you [use the ResolveName method](#bk_EWSMA), except that it uses a different name for valid output examples.</span></span>
  
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

<span data-ttu-id="40bcd-163">La réponse renvoie un maximum de 100 candidats, bien qu’il puisse y avoir plus de 100 candidats potentiels pour déterminer si seuls les 100 premiers candidats d’un plus grand nombre de candidats ont été renvoyés, vérifiez la valeur de l’attribut [IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) de l’élément [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="40bcd-163">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of the [IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribute of the [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="40bcd-164">Si la valeur est true, il n’y a pas de candidats possibles ; Si la valeur est false, l’opération renvoie uniquement le premier 100 d’un plus grand nombre de candidats potentiels.</span><span class="sxs-lookup"><span data-stu-id="40bcd-164">If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="40bcd-165">L’exemple suivant montre la réponse XML lorsqu’un candidat est trouvé.</span><span class="sxs-lookup"><span data-stu-id="40bcd-165">The following example shows the XML response when one candidate is found.</span></span> <span data-ttu-id="40bcd-166">N’oubliez pas que le [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) peut contenir jusqu’à 100 candidats, chacun étant représenté par l’élément de [résolution](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) et ses éléments enfants.</span><span class="sxs-lookup"><span data-stu-id="40bcd-166">Remember, the [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) can contain up to 100 candidates, each one represented by the [Resolution](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) element and its child elements.</span></span> 
  
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

<span data-ttu-id="40bcd-167">Vous n’allez pas toujours trouver des candidats pour votre nom ambigu.</span><span class="sxs-lookup"><span data-stu-id="40bcd-167">You're not always going to come up with candidates for your ambiguous name.</span></span> <span data-ttu-id="40bcd-168">L’exemple suivant montre la réponse XML, comme une erreur, lorsqu’aucun candidat n’est trouvé.</span><span class="sxs-lookup"><span data-stu-id="40bcd-168">The following example shows the XML response, as an error, when no candidates are found.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="40bcd-169">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="40bcd-169">See also</span></span>


- [<span data-ttu-id="40bcd-170">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="40bcd-170">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="40bcd-171">Développer des groupes de distribution à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="40bcd-171">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

