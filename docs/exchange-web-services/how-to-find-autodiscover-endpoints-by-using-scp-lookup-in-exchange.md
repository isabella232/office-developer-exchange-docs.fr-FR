---
title: Trouver des points de terminaison de découverte automatique à l’aide de la recherche SCP dans Exchange
manager: kelbow
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b24228a8-5127-4bac-aef0-9c9e8843c9ff
description: Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment trouver des objets SCP de découverte automatique dans les services de domaine Active Directory (AD DS) et les utiliser pour rechercher des URL de point de terminaison de découverte automatique à utiliser avec le service de découverte automatique Exchange.
ms.openlocfilehash: 59fd316d0aa0feea81b60c279040da018c51b47d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754827"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a><span data-ttu-id="c4503-103">Trouver des points de terminaison de découverte automatique à l’aide de la recherche SCP dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c4503-103">How to: Find Autodisover endpoints by using SCP lookup in Exchange</span></span>

<span data-ttu-id="c4503-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez comment trouver des objets SCP de découverte automatique dans les services de domaine Active Directory (AD DS) et les utiliser pour rechercher des URL de point de terminaison de découverte automatique à utiliser avec le service de découverte automatique Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4503-104">Find out how to locate Autodiscover SCP objects in Active Directory Domain Services (AD DS) and use them to find Autodiscover endpoint URLs to use with the Exchange Autodiscover service.</span></span>
  
<span data-ttu-id="c4503-p101">La découverte automatique facilite la récupération des informations nécessaires pour se connecter aux boîtes aux lettres sur des serveurs Exchange. Toutefois, pour utiliser la découverte automatique, vous avez besoin d'un moyen pour trouver des serveurs de découverte automatique qui sont appropriés pour l'utilisateur pour lequel vous récupérez des paramètres. Les objets de point de connexion de service (SCP) dans AD DS offrent un moyen facile pour que les clients appartenant au domaine recherchent des serveurs de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="c4503-p101">Autodiscover makes it easy to retrieve information that you need to connect to mailboxes on Exchange servers. However, in order to use Autodiscover, you need a way to find Autodiscover servers that are appropriate for the user you're retrieving settings for. Service connection point (SCP) objects in AD DS provide an easy way for domain-joined clients to look up Autodiscover servers.</span></span> 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a><span data-ttu-id="c4503-108">Obtention de la configuration permettant de trouver des points de terminaison de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="c4503-108">Get set up to find Autodiscover endpoints</span></span>
<span data-ttu-id="c4503-109"><a name="bk_PreReqs"> </a></span><span class="sxs-lookup"><span data-stu-id="c4503-109"></span></span>

<span data-ttu-id="c4503-110">Pour localiser des objets SCP de découverte automatique dans AD DS, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="c4503-110">To locate Autodiscover SCP objects in AD DS, you need to have access to the following:</span></span>
  
- <span data-ttu-id="c4503-111">Un serveur qui exécute une version d'Exchange en local à partir d'Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="c4503-111">A server that is running a version of Exchange on-premises starting with Exchange 2007 SP1.</span></span>
    
- <span data-ttu-id="c4503-112">Un ordinateur client qui est joint au domaine sur lequel le serveur Exchange est installé.</span><span class="sxs-lookup"><span data-stu-id="c4503-112">A client computer that is joined to the domain that the Exchange server is installed in.</span></span>
    
- <span data-ttu-id="c4503-113">Un compte d'utilisateur qui a une boîte aux lettres sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4503-113">A user account that has a mailbox on the Exchange server.</span></span> 
    
<span data-ttu-id="c4503-p102">En outre, avant de commencer, vous souhaiterez connaître certains concepts de base. Voici quelques ressources qui vous seront utiles.</span><span class="sxs-lookup"><span data-stu-id="c4503-p102">Also, before you begin, you'll want to be familiar some basic concepts. The following are some resources that you'll find helpful.</span></span>
  
<span data-ttu-id="c4503-116">**Tableau 1. Articles relatifs à la recherche de points de terminaison de découverte automatique à partir d'objets SCP**</span><span class="sxs-lookup"><span data-stu-id="c4503-116">**Table 1. Related articles for finding Autodiscover endpoints from SCP objects**</span></span>

|<span data-ttu-id="c4503-117">**Lire cet article**</span><span class="sxs-lookup"><span data-stu-id="c4503-117">**Read this article**</span></span>|<span data-ttu-id="c4503-118">**Pour en savoir plus sur...**</span><span class="sxs-lookup"><span data-stu-id="c4503-118">**To learn about…**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4503-119">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c4503-119">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="c4503-120">Fonctionnement du service de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="c4503-120">How the Autodiscover service works.</span></span>  <br/> |
|[<span data-ttu-id="c4503-121">Publication avec des points de connexion de service</span><span class="sxs-lookup"><span data-stu-id="c4503-121">Publishing with Service Connection Points</span></span>](http://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |<span data-ttu-id="c4503-122">Utilisation des objets SCP pour publier des données spécifiques du service</span><span class="sxs-lookup"><span data-stu-id="c4503-122">How SCP objects are used to publish service-specific data.</span></span>  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a><span data-ttu-id="c4503-123">Localisation d'objets SCP de découverte automatique dans AD DS</span><span class="sxs-lookup"><span data-stu-id="c4503-123">Locate Autodiscover SCP objects in AD DS</span></span>
<span data-ttu-id="c4503-124"><a name="bk_LocateScpObjects"> </a></span><span class="sxs-lookup"><span data-stu-id="c4503-124"></span></span>

<span data-ttu-id="c4503-p103">La première étape de la recherche de points de terminaison de découverte automatique publiés dans AD DS consiste à localiser les objets SCP de découverte automatique. Exchange publie deux types d'objets SCP de découverte automatique :</span><span class="sxs-lookup"><span data-stu-id="c4503-p103">The first step toward finding Autodiscover endpoints published in AD DS is to locate the Autodiscover SCP objects. Exchange publishes two types of SCP objects for Autodiscover:</span></span>
  
- <span data-ttu-id="c4503-p104">**Pointeurs SCP**: ils contiennent des informations qui pointent vers des serveurs LDAP spécifiques qui doivent être utilisés afin de localiser des objets SCP de découverte automatique pour le domaine de l'utilisateur. Les pointeurs SCP sont marqués avec le GUID suivant : 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span><span class="sxs-lookup"><span data-stu-id="c4503-p104">**SCP pointers** — These contain information that points to specific LDAP servers that should be used to locate Autodiscover SCP objects for the user's domain. SCP pointers are stamped with the following GUID: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span></span> 
    
- <span data-ttu-id="c4503-p105">**URL SCP**: elles contiennent les URL des points de terminaison de découverte automatique. Les URL SCP sont marquées avec le GUID suivant : 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span><span class="sxs-lookup"><span data-stu-id="c4503-p105">**SCP URLs** — These contain URLs for Autodiscover endpoints. SCP URLs are stamped with the following GUID: 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span></span> 
    
### <a name="to-locate-autodiscover-scp-objects"></a><span data-ttu-id="c4503-131">Pour localiser des objets SCP de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="c4503-131">To locate Autodiscover SCP objects</span></span>

1. <span data-ttu-id="c4503-p106">Lisez la propriété **configurationNamingContext** de l'entrée DSE racine dans AD DS pour obtenir le chemin d'accès au contexte d'appellation de configuration pour le domaine. Pour ce faire, utilisez la classe [DirectoryEntry](http://msdn2.microsoft.com/fr-FR/library/z9cddzaa) ou toute autre API qui peut accéder à AD DS.</span><span class="sxs-lookup"><span data-stu-id="c4503-p106">Read the **configurationNamingContext** property of the root DSE entry in AD DS to get the path to the configuration naming context for the domain. You can do this by using the [DirectoryEntry](http://msdn2.microsoft.com/fr-FR/library/z9cddzaa) class, or any other API that can acces AD DS.</span></span> 
    
2. <span data-ttu-id="c4503-134">Recherchez dans le contexte d'appellation de configuration des objets SCP qui ont soit le GUID de pointeur SCP ou le GUID d'URL SCP dans la propriété **keywords**.</span><span class="sxs-lookup"><span data-stu-id="c4503-134">Search for SCP objects in the configuration naming context that have either the SCP pointer GUID or the SCP URL GUID in the **keywords** property.</span></span> 
    
3. <span data-ttu-id="c4503-135">Vérifiez les objets SCP que vous avez trouvés pour un pointeur SCP inclus dans le domaine de l'utilisateur en vérifiant la propriété **keywords** d'une entrée égale à`"Domain=<domain>"`.</span><span class="sxs-lookup"><span data-stu-id="c4503-135">Check the SCP objects you found for an SCP pointer that is scoped to the user's domain by checking the **keywords** property for an entry equal to "Domain=`"Domain=<domain>"`".</span></span> <span data-ttu-id="c4503-136">Par exemple, si l'adresse e-mail de l'utilisateur est elvin@contoso.com, vous rechercherez un pointeur SCP avec une entrée dans la propriété** keywords**qui est égale à`"Domain=contoso.com"`.</span><span class="sxs-lookup"><span data-stu-id="c4503-136">For example, if the user's email address is elvin@contoso.com, you would look for an SCP pointer with an entry in the keywords property that is equal to "Domain=contoso.com".</span></span> <span data-ttu-id="c4503-137">Si un pointeur SCP correspondant est trouvé, abandonnez le jeu d'objets SCP et recommencez à l'étape 1 en utilisant la valeur de la propriété **serviceBindingInformation** comme serveur pour se connecter à l'entrée DSE racine.</span><span class="sxs-lookup"><span data-stu-id="c4503-137">If a matching SCP pointer is found, discard the set of SCP objects and start over at step 1 using the value of the **serviceBindingInformation** property as the server to connect to for the Root DSE entry.</span></span> 
    
4. <span data-ttu-id="c4503-138">Si vous ne trouvez pas de pointeurs SCP inclus dans le domaine de l'utilisateur, recherchez des pointeurs SCP qui ne sont pas inclus dans un domaine, puis enregistrez la valeur de la propriété **serviceBindingInformation** comme serveur « de secours », au cas où le serveur actuel ne donne pas de résultats.</span><span class="sxs-lookup"><span data-stu-id="c4503-138">If you don't find any SCP pointers scoped to the user's domain, check for any SCP pointers that aren't scoped to any domain, and save the value of the **serviceBindingInformation** property as a "fallback" server, in case the current server doesn't give you any results.</span></span> 
    
5. <span data-ttu-id="c4503-139">Si vous ne trouvez pas de pointeurs SCP inclus dans le domaine, vous êtes prêt à passer à l'étape suivante, à savoir la génération d'une liste de points de terminaison de découverte automatique triés par priorité à partir de vos résultats.</span><span class="sxs-lookup"><span data-stu-id="c4503-139">If you didn't find any SCP pointers scoped to the domain, you're ready to move on to the next step: generating a prioritized list of Autodiscover endpoints from your results.</span></span>
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a><span data-ttu-id="c4503-140">Génération d'une liste de points de terminaison de découverte automatique triés par priorité</span><span class="sxs-lookup"><span data-stu-id="c4503-140">Generate a prioritized list of Autodiscover endpoints</span></span>
<span data-ttu-id="c4503-141"><a name="bk_GenerateList"> </a></span><span class="sxs-lookup"><span data-stu-id="c4503-141"></span></span>

<span data-ttu-id="c4503-142">Vous pouvez générer une liste d'URL de point de terminaison de découverte automatique triées par priorité, en utilisant le jeu d'objets SCP que vous avez trouvé, en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="c4503-142">You can generate a prioritized list of Autodiscover endpoint URLs, using the set of SCP objects that you located, by doing the following:</span></span>
  
1. <span data-ttu-id="c4503-143">Obtenez le nom du site Active Directory de l'ordinateur client.</span><span class="sxs-lookup"><span data-stu-id="c4503-143">Get the Active Directory site name of the client computer.</span></span>
    
2. <span data-ttu-id="c4503-144">Vérifiez la propriété **keywords** sur chaque URL SCP dans le jeu d'objets SCP que vous avez trouvé, et attribuez une priorité à l'URL en fonction des règles suivantes :</span><span class="sxs-lookup"><span data-stu-id="c4503-144">Check the **keywords** property on each SCP URL in the set of SCP objects you found, and assign a priority to the URL based on the following rules:</span></span> 
    
  - <span data-ttu-id="c4503-145">Si la propriété **keywords** contient la valeur du`"Site=<site name>"`, où `<site name>` est égal au nom du site Active Directory que vous avez récupéré à l'étape précédente, attribuez à l'URL une priorité de 1.</span><span class="sxs-lookup"><span data-stu-id="c4503-145">If the **keywords** property contains a value of "Site=`"Site=<site name>"`", where `<site name>` equals the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 1.</span></span> 
    
  - <span data-ttu-id="c4503-146">Si la propriété **keywords** ne contient pas d'entrée avec une valeur qui commence par`"Site="`, attribuez à l'URL une priorité de 2.</span><span class="sxs-lookup"><span data-stu-id="c4503-146">If the keywords property does not contain an entry with a value that starts with "Site=", assign the URL a priority of 2.</span></span> 
    
  - <span data-ttu-id="c4503-147">Si la propriété **keywords** contient la valeur de`"Site=<site name>`, où `<site name>` n'est pas égal au nom du site Active Directory que vous avez récupéré à l'étape précédente, attribuez à l'URL une priorité de 3.</span><span class="sxs-lookup"><span data-stu-id="c4503-147">If the **keywords** property contains a value of "Site=`"Site=<site name>`, where `<site name>` does not equal the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 3.</span></span> 
    
## <a name="code-example-performing-an-scp-lookup"></a><span data-ttu-id="c4503-148">Exemple de code : Exécution une recherche CSP</span><span class="sxs-lookup"><span data-stu-id="c4503-148">Code example: Performing an SCP lookup</span></span>
<span data-ttu-id="c4503-149"><a name="bk_CodeExample"> </a></span><span class="sxs-lookup"><span data-stu-id="c4503-149"></span></span>

<span data-ttu-id="c4503-150">Dans l'exemple de code suivant, vous verrez comment localiser des objets SCP de découverte automatique et générer une liste de points de terminaison de découverte automatique triés par priorité.</span><span class="sxs-lookup"><span data-stu-id="c4503-150">In the following code example, you'll see how to locate Autodiscover SCP objects and generate a prioritized list of Autodiscover endpoints.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using System.DirectoryServices;
using System.DirectoryServices.ActiveDirectory;
namespace ScpLookup
{
    // This sample is for demonstration purposes only. Before you run this sample, make sure 
    // that the code meets the coding requirements of your organization. 
    class Program
    {
        static void Main(string[] args)
        {
            string domain = args[0];
            Console.WriteLine("Performing SCP lookup for {0}.", domain);
            List<string> scpUrls = GetScpUrls(null, domain);
            Console.WriteLine("\nOrdered List of Autodiscover endpoints:");
            foreach (string url in scpUrls)
            {
                Console.WriteLine("  {0}", url);
            }
            Console.WriteLine("SCP lookup done.");
        }
        // GUID for SCP URL keyword.
        private const string ScpUrlGuidString = @"77378F46-2C66-4aa9-A6A6-3E7A48B19596";
        // GUID for SCP pointer keyword.
        private const string ScpPtrGuidString = @"67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68";
        static List<string> GetScpUrls(string ldapServer, string domain)
        {
            // Create a new list to return.
            List<string> scpUrlList = new List<string>();
            string rootDSEPath = null;
            // If ldapServer is null/empty, use LDAP://RootDSE to
            // connect to Active Directory Domain Services (AD DS). Otherwise, use
            // LDAP://SERVERNAME/RootDSE to connect to a specific server.
            if (string.IsNullOrEmpty(ldapServer))
            {
                rootDSEPath = "LDAP://RootDSE";
            }
            else
            {
                rootDSEPath = ldapServer + "/RootDSE";
            }
            SearchResultCollection scpEntries = null;
            try
            {
                // Get the root directory entry.
                DirectoryEntry rootDSE = new DirectoryEntry(rootDSEPath);
                // Get the configuration path.
                string configPath = rootDSE.Properties["configurationNamingContext"].Value as string;
                // Get the configuration entry.
                DirectoryEntry configEntry = new DirectoryEntry("LDAP://" + configPath);
                // Create a search object for the configuration entry.
                DirectorySearcher configSearch = new DirectorySearcher(configEntry);
                // Set the search filter to find SCP URLs and SCP pointers.
                configSearch.Filter = "(&amp;(objectClass=serviceConnectionPoint)" +
                    "(|(keywords=" + ScpPtrGuidString + ")(keywords=" + ScpUrlGuidString + ")))";
                // Specify which properties you want to retrieve.
                configSearch.PropertiesToLoad.Add("keywords");
                configSearch.PropertiesToLoad.Add("serviceBindingInformation");
                scpEntries = configSearch.FindAll();
            }
            catch (Exception ex)
            {
                Console.WriteLine("SCP lookup failed with: ");
                Console.WriteLine(ex.ToString());
            }
            // If no SCP entries were found, then exit.
            if (scpEntries == null || scpEntries.Count <= 0)
            {
                Console.WriteLine("No SCP records found.");
                return null;
            }
            string fallBackLdapPath = null;
            // Check for SCP pointers.
            foreach (SearchResult scpEntry in scpEntries)
            {
                ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                if (CollectionContainsExactValue(entryKeywords, ScpPtrGuidString))
                {
                    string ptrLdapPath = scpEntry.Properties["serviceBindingInformation"][0] as string;
                    // Determine whether this pointer is scoped to the user's domain.
                    if (CollectionContainsExactValue(entryKeywords, "Domain=" + domain))
                    {
                        Console.WriteLine("Found SCP pointer for " + domain + " in " + scpEntry.Path);
                        // Restart SCP lookup with the server assigned for the domain.
                        Console.WriteLine("Restarting SCP lookup in " + ptrLdapPath);
                        return GetScpUrls(ptrLdapPath, domain);
                    }
                    else
                    {
                        // Save the first SCP pointer that is not scoped to a domain as a fallback
                        // in case you do not get any results from this server.
                        if (entryKeywords.Count == 1 &amp;&amp; string.IsNullOrEmpty(fallBackLdapPath))
                        {
                            fallBackLdapPath = ptrLdapPath;
                            Console.WriteLine("Saved fallback SCP pointer: " + fallBackLdapPath);
                        }
                    }
                }
            }
            string computerSiteName = null;
            try
            {
                // Get the name of the ActiveDirectorySite the computer
                // belongs to (if it belongs to one).
                ActiveDirectorySite site = ActiveDirectorySite.GetComputerSite();
                computerSiteName = site.Name;
                Console.WriteLine("Local computer in site: " + computerSiteName);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Unable to get computer site name.");
                Console.WriteLine(ex.ToString());
            }
            if (!string.IsNullOrEmpty(computerSiteName))
            {
                // Scan the search results for SCP URLs.
                // SCP URLs fit into three tiers:
                //   Priority 1: The URL is scoped to the computer's Active Directory site.
                //   Priority 2: The URL is not scoped to any Active Directory site.
                //   Priority 3: The URL is scoped to a different Active Directory site.
                // Temporary lists to hold priority 2 and 3 URLs.
                List<string> priorityTwoUrls = new List<string>();
                List<string> priorityThreeUrls = new List<string>();
                foreach (SearchResult scpEntry in scpEntries)
                {
                    ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                    // Check for SCP URLs.
                    if (CollectionContainsExactValue(entryKeywords, ScpUrlGuidString))
                    {
                        string scpUrlPath = scpEntry.Properties["adsPath"][0] as string;
                        Console.WriteLine("SCP URL found at {0}", scpUrlPath);
                        string scpUrl = scpEntry.Properties["serviceBindingInformation"][0] as string;
                        scpUrl = scpUrl.ToLower();
                        // Determine whether this entry is scoped to the computer's site.
                        if (CollectionContainsExactValue(entryKeywords, "Site=" + computerSiteName))
                        {
                            // Priority 1.
                            if (!scpUrlList.Contains(scpUrl.ToLower()))
                            {
                                Console.WriteLine("Adding priority 1 SCP URL: {0}", scpUrl.ToLower());
                                scpUrlList.Add(scpUrl);
                            }
                            else
                            {
                                Console.WriteLine("Priority 1 SCP URL already found: {0}", scpUrl);
                            }
                        }
                        else
                        {
                            // Determine whether this is a priority 2 or 3 URL.
                            if (CollectionContainsPrefixValue(entryKeywords, "Site="))
                            {
                                // Priority 3.
                                if (!priorityThreeUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 3 SCP URL: {0}", scpUrl);
                                    priorityThreeUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 3 SCP URL already found: {0}", scpUrl);
                                }
                            }
                            else
                            {
                                // Priority 2.
                                if (!priorityTwoUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 2 SCP URL: {0}", scpUrl);
                                    priorityTwoUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 2 SCP URL already found: {0}", scpUrl);
                                }
                            }
                        }
                    }
                }
                // Now add the priority 2 URLs into the main list.
                foreach (string priorityTwoUrl in priorityTwoUrls)
                {
                    // If the URL is already in the list as a priority 1, 
                    // don't add it again.
                    if (!scpUrlList.Contains(priorityTwoUrl))
                    {
                        scpUrlList.Add(priorityTwoUrl);
                    }
                }
                // Now add the priority 3 URLs into the main list.
                foreach (string priorityThreeUrl in priorityThreeUrls)
                {
                    // If the URL is already in the list as a priority 1
                    // or priority 2, don't add it again.
                    if (!scpUrlList.Contains(priorityThreeUrl))
                    {
                        scpUrlList.Add(priorityThreeUrl);
                    }
                }
                // If after all this, you still have no URLs in your list,
                // try the fallback SCP pointer, if you have one.
                if (scpUrlList.Count == 0 &amp;&amp; fallBackLdapPath != null)
                {
                    return GetScpUrls(fallBackLdapPath, domain);
                }
            }
            return scpUrlList;
        }
        private static bool CollectionContainsExactValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (string.Compare(value, entry, true) == 0)
                        return true;
                }
            }
            return false;
        }
        private static bool CollectionContainsPrefixValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (entry.StartsWith(value))
                        return true;
                }
            }
            return false;
        }
    }
}
```

## <a name="next-steps"></a><span data-ttu-id="c4503-151">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="c4503-151">Next steps</span></span>
<span data-ttu-id="c4503-152"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="c4503-152"></span></span>

<span data-ttu-id="c4503-p108">L'étape suivante du processus de découverte automatique consiste à envoyer des demandes de découverte automatique aux URL que vous avez trouvées, en commençant par les URL de priorité 1, puis en passant aux URL de priorité 2 et en finissant par les URL de priorité 3. Pour savoir comment envoyer des demandes de découverte automatique et gérer les réponses, lisez les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="c4503-p108">The next step in the Autodiscover process is to send Autodiscover requests to the URLs that you found, starting with priority 1 URLs, then priority 2 URLs, and finally priority 3 URLs. To learn more about how to send Autodiscover requests and handle responses, read the following articles:</span></span>
  
- [<span data-ttu-id="c4503-155">Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="c4503-155">How to: Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="c4503-156">Gestion des messages d'erreur de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="c4503-156">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a><span data-ttu-id="c4503-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4503-157">See also</span></span>

- [<span data-ttu-id="c4503-158">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c4503-158">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)   
- [<span data-ttu-id="c4503-159">La configuration de vos applications EWS</span><span class="sxs-lookup"><span data-stu-id="c4503-159">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    

