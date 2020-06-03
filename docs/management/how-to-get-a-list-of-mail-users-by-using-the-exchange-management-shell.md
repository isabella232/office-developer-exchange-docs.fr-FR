---
title: Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement de commande Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Découvrez comment utiliser les applets de commande Exchange Management Shell pour créer un outil qui renvoie la liste des utilisateurs de boîte aux lettres Exchange.
localization_priority: Priority
ms.openlocfilehash: 817d92ef1bb88017f471681b448c052ecaa54e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435708"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a><span data-ttu-id="c5cee-103">Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="c5cee-103">Get a list of mail users by using the Exchange Management Shell</span></span>

<span data-ttu-id="c5cee-104">Découvrez comment utiliser les applets de commande Exchange Management Shell pour créer un outil qui renvoie la liste des utilisateurs de boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5cee-104">Learn how to use Exchange Management Shell cmdlets to create a tool that returns a list of Exchange mailbox users.</span></span>
  
<span data-ttu-id="c5cee-105">**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="c5cee-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span> 
  
<span data-ttu-id="c5cee-106">L’obtention d’une liste d’utilisateurs à partir d’Exchange Online, Exchange Online dans le cadre d’Office 365 ou d’une version d’Exchange à partir d’Exchange 2013 à l’aide d’un outil géré qui appelle une cmdlet de l’environnement de ligne de commande Exchange Management Shell est un processus en deux étapes.</span><span class="sxs-lookup"><span data-stu-id="c5cee-106">Getting a list of users from Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013 by using a managed tool that calls an Exchange Management Shell cmdlet is a two-step process.</span></span> <span data-ttu-id="c5cee-107">Tout d’abord, vous établissez une instance d’exécution distante sur un serveur Exchange ; Ensuite, vous exécutez l’applet de commande pour récupérer les informations utilisateur dans l’instance d’exécution distante.</span><span class="sxs-lookup"><span data-stu-id="c5cee-107">First, you establish a remote runspace on an Exchange server; then, you run the cmdlet to retrieve the user information in the remote runspace.</span></span> 

<span data-ttu-id="c5cee-108">Pour vous connecter à l’instance d’exécution distante, vous devez vous authentifier auprès du serveur Exchange à l’aide du modèle d’authentification qui répond aux exigences de sécurité de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="c5cee-108">To connect to the remote runspace, you have to authenticate with the Exchange server by using the authentication scheme that meets the security requirements of your organization.</span></span> 

<span data-ttu-id="c5cee-109">Cet article fournit des exemples de code que vous pouvez utiliser pour configurer une instance d’exécution distante et exécuter une cmdlet Exchange Management Shell pour obtenir une liste d’utilisateurs à partir d’un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5cee-109">This article provides code examples that you can use to set up a remote runspace and run an Exchange Management Shell cmdlet to get a list of users from an Exchange server.</span></span>

<span data-ttu-id="c5cee-110"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="c5cee-110"><a name="bk_prerequisites"> </a></span></span>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a><span data-ttu-id="c5cee-111">Conditions préalables requises pour obtenir une liste d’utilisateurs de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="c5cee-111">Prerequisites for getting a list of mailbox users</span></span>

<span data-ttu-id="c5cee-112">Pour effectuer cette tâche, vous avez besoin d’une référence aux espaces de noms suivants :</span><span class="sxs-lookup"><span data-stu-id="c5cee-112">To perform this task, you need a reference to the following namespaces:</span></span>
  
- <span data-ttu-id="c5cee-113">**System. Collections. ObjectModel**</span><span class="sxs-lookup"><span data-stu-id="c5cee-113">**System.Collections.ObjectModel**</span></span>
- <span data-ttu-id="c5cee-114">**System. Management. Automation**</span><span class="sxs-lookup"><span data-stu-id="c5cee-114">**System.Management.Automation**</span></span>
- <span data-ttu-id="c5cee-115">**System. Management. Automation. Remoting**</span><span class="sxs-lookup"><span data-stu-id="c5cee-115">**System.Management.Automation.Remoting**</span></span>
- <span data-ttu-id="c5cee-116">**System. Management. Automation. instances**</span><span class="sxs-lookup"><span data-stu-id="c5cee-116">**System.Management.Automation.Runspaces**</span></span>
    
> [!NOTE]
>  <span data-ttu-id="c5cee-p102">Lorsque vous utilisez Visual Studio pour créer une application, vous devez ajouter une référence à l’assembly System.Management.Automation.dll vers le projet. Vous trouverez l’assembly dans l’un des emplacements suivants :</span><span class="sxs-lookup"><span data-stu-id="c5cee-p102">When you are using Visual Studio to create an application, you must add a reference to the System.Management.Automation.dll assembly to the project. The assembly can be found in one of the following locations:</span></span>
> - <span data-ttu-id="c5cee-119">Pour les systèmes d’exploitation Windows XP et Windows Vista, le répertoire d’installation de Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="c5cee-119">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span>
> - <span data-ttu-id="c5cee-120">Pour les systèmes d’exploitation Windows 7 et Windows 8, le dossier suivant : Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="c5cee-120">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
<span data-ttu-id="c5cee-121">Ne chargez pas le composant logiciel enfichable de gestion Exchange 2013 dans l’instance d’exécution sur les ordinateurs qui exécutent des applications qui automatisent les cmdlets Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="c5cee-121">Do not load the Exchange 2013 Management snap-in into the runspace on computers that are running applications that automate Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="c5cee-122">L’application doit créer à la place une instance d’exécution distante, comme décrit plus loin dans cet article.</span><span class="sxs-lookup"><span data-stu-id="c5cee-122">The application should instead create a remote runspace, as described later in this article.</span></span>

<span data-ttu-id="c5cee-123"><a name="bk_gettinglistmailbox"> </a></span><span class="sxs-lookup"><span data-stu-id="c5cee-123"><a name="bk_gettinglistmailbox"> </a></span></span>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a><span data-ttu-id="c5cee-124">Se connecter à une instance d’exécution distante sur un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="c5cee-124">Connect to a remote runspace on an Exchange server</span></span>

<span data-ttu-id="c5cee-p104">La méthode que vous utilisez pour vous connecter à une instance d’exécution distante pour exécuter l’applet de commande Exchange Management Shell varie selon le modèle d’authentification choisi. Cette section fournit des exemples de code qui illustrent la procédure de connexion à une instance d’exécution distante lorsque vous utilisez une méthode d’authentification répertoriée dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-p104">The method that you use to connect to a remote runspace to use an Exchange Management Shell cmdlet varies based on the authentication scheme that you are using. This section provides code examples that show how to connect to a remote runspace when you are using an authentication method listed in the following table.</span></span>
  
|<span data-ttu-id="c5cee-127">**Méthode d'authentification**</span><span class="sxs-lookup"><span data-stu-id="c5cee-127">**Authentication method**</span></span>|<span data-ttu-id="c5cee-128">**S’applique à**</span><span class="sxs-lookup"><span data-stu-id="c5cee-128">**Applies to**</span></span>|<span data-ttu-id="c5cee-129">**URI**</span><span class="sxs-lookup"><span data-stu-id="c5cee-129">**URI**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="c5cee-130">Se connecter à une instance d’exécution distante sur Exchange Online à l’aide de l’authentification de base</span><span class="sxs-lookup"><span data-stu-id="c5cee-130">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>](#bk_basic) <br/> |<span data-ttu-id="c5cee-131">Serveurs Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c5cee-131">Exchange Online servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[<span data-ttu-id="c5cee-132">Se connecter à une instance d’exécution distante à l’aide de l’authentification des certificats</span><span class="sxs-lookup"><span data-stu-id="c5cee-132">Connect to a remote runspace by using certificate authentication</span></span>](#bk_cert) <br/> |<span data-ttu-id="c5cee-133">Exchange Online et serveurs locaux Exchange</span><span class="sxs-lookup"><span data-stu-id="c5cee-133">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[<span data-ttu-id="c5cee-134">Se connecter à un espace d’exécution à distance sur un serveur Exchange à l’aide de l’authentification Kerberos</span><span class="sxs-lookup"><span data-stu-id="c5cee-134">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>](#bk_Kerberos) <br/> |<span data-ttu-id="c5cee-135">Exchange Online et serveurs locaux Exchange</span><span class="sxs-lookup"><span data-stu-id="c5cee-135">Exchange Online and Exchange on-premises servers</span></span>  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<span data-ttu-id="c5cee-136"><a name="bk_basic"> </a></span><span class="sxs-lookup"><span data-stu-id="c5cee-136"><a name="bk_basic"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a><span data-ttu-id="c5cee-137">Se connecter à une instance d’exécution distante sur Exchange Online à l’aide de l’authentification de base</span><span class="sxs-lookup"><span data-stu-id="c5cee-137">Connect to a remote runspace on Exchange Online by using basic authentication</span></span>

<span data-ttu-id="c5cee-138">L’exemple suivant définit la méthode **GetUsersUsingBasicAuth**, qui crée une instance d’exécution Exchange Management Shell sur un serveur Exchange Online à l’aide de l’authentification de base.</span><span class="sxs-lookup"><span data-stu-id="c5cee-138">The following code example defines the **GetUsersUsingBasicAuth** method, which creates an Exchange Management Shell runspace on a remote Exchange Online server by using basic authentication.</span></span> <span data-ttu-id="c5cee-139">La méthode appelle ensuite la méthode **GetUserInformation** comme décrit à la section [Obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution distante](#bk_remote) pour renvoyer la liste des utilisateurs du serveur distant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-139">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="c5cee-140">Cette méthode requiert les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="c5cee-140">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="c5cee-141">**liveIDConnectionUri** &ndash; Chaîne qui contient l’URI du serveur Exchange Online qui authentifiera l’application.</span><span class="sxs-lookup"><span data-stu-id="c5cee-141">**liveIDConnectionUri** &ndash; A string that contains the URI of the Exchange Online server that will authenticate the application.</span></span> <span data-ttu-id="c5cee-142">Si Exchange Online est en cours d’exécution dans Office 365, l’URI est `https://outlook.office365.com/PowerShell-LiveID` ; sinon, l’URI est `https://<servername>/PowerShell-LiveID` .</span><span class="sxs-lookup"><span data-stu-id="c5cee-142">If Exchange Online is running in Office 365, the URI is `https://outlook.office365.com/PowerShell-LiveID`; otherwise, the URI is `https://<servername>/PowerShell-LiveID`.</span></span> 
    
-  <span data-ttu-id="c5cee-143">**schemaUri** &ndash; Chaîne qui contient l’URI du document de schéma qui définit le schéma de l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="c5cee-143">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="c5cee-144">L’URI du schéma est `https://schemas.microsoft.com/powershell/Microsoft.Exchange` .</span><span class="sxs-lookup"><span data-stu-id="c5cee-144">The schema URI is `https://schemas.microsoft.com/powershell/Microsoft.Exchange`.</span></span> 
    
-  <span data-ttu-id="c5cee-145">**informations d’identification** &ndash; Objet [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) qui contient les informations d’identification de l’utilisateur qui exécute l’application.</span><span class="sxs-lookup"><span data-stu-id="c5cee-145">**credentials** &ndash; A [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
-  <span data-ttu-id="c5cee-146">**nombre** &ndash; Nombre d’utilisateurs de boîtes aux lettres Exchange à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="c5cee-146">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingBasicAuth(
    string liveIDConnectionUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(liveIDConnectionUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingBasicAuth( _
    ByVal LiveIDConnectionUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(LiveIDConnectionUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="c5cee-147"><a name="bk_cert"> </a></span><span class="sxs-lookup"><span data-stu-id="c5cee-147"><a name="bk_cert"> </a></span></span>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a><span data-ttu-id="c5cee-148">Se connecter à une instance d’exécution distante à l’aide de l’authentification des certificats</span><span class="sxs-lookup"><span data-stu-id="c5cee-148">Connect to a remote runspace by using certificate authentication</span></span>

<span data-ttu-id="c5cee-149">L’exemple suivant définit la méthode **GetUsersUsingCertificate**, qui crée une instance d’exécution Exchange Management Shell sur un serveur distant à l’aide d’un certificat.</span><span class="sxs-lookup"><span data-stu-id="c5cee-149">The following code example defines the **GetUsersUsingCertificate** method, which creates an Exchange Management Shell runspace on a remote server by using a certificate.</span></span> <span data-ttu-id="c5cee-150">La méthode appelle ensuite la méthode **GetUserInformation** comme décrit à la section [Obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution distante](#bk_remote) pour renvoyer la liste des utilisateurs du serveur distant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-150">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="c5cee-151">Cette méthode requiert les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="c5cee-151">This method requires the following parameters:</span></span>
  
-  <span data-ttu-id="c5cee-152">**empreinte numérique** &ndash; Chaîne qui contient l’empreinte numérique du certificat utilisé pour authentifier l’application.</span><span class="sxs-lookup"><span data-stu-id="c5cee-152">**thumbprint** &ndash; A string that contains the thumbprint of the certificate that is used to authenticate the application.</span></span> 
    
-  <span data-ttu-id="c5cee-153">**certConnectionUri** &ndash; Chaîne qui contient l’URI du serveur qui authentifiera le certificat.</span><span class="sxs-lookup"><span data-stu-id="c5cee-153">**certConnectionUri** &ndash; A string that contains the URI of the server that will authenticate the certificate.</span></span> <span data-ttu-id="c5cee-154">L’URI correspond à l’une des adresses répertoriées dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-154">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="c5cee-155">**Tableau 1. URI certConnectionUri**</span><span class="sxs-lookup"><span data-stu-id="c5cee-155">**Table 1. certConnectionUri URIs**</span></span>

    |<span data-ttu-id="c5cee-156">**Server**</span><span class="sxs-lookup"><span data-stu-id="c5cee-156">**Server**</span></span>|<span data-ttu-id="c5cee-157">**URI**</span><span class="sxs-lookup"><span data-stu-id="c5cee-157">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="c5cee-158">Serveur Exchange sans SSL</span><span class="sxs-lookup"><span data-stu-id="c5cee-158">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="c5cee-159">Serveur Exchange avec SSL</span><span class="sxs-lookup"><span data-stu-id="c5cee-159">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="c5cee-160">Exchange Online dans le cadre d’Office 365</span><span class="sxs-lookup"><span data-stu-id="c5cee-160">Exchange Online as part of Office 365</span></span>  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- <span data-ttu-id="c5cee-161">**schemaUri** &ndash; Chaîne qui contient l’URI du document de schéma qui définit le schéma de l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="c5cee-161">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="c5cee-162">L’URI du schéma est https://schemas.microsoft.com/powershell/Microsoft.Exchange .</span><span class="sxs-lookup"><span data-stu-id="c5cee-162">The schema URI is https://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="c5cee-163">**nombre** &ndash; Nombre d’utilisateurs de boîtes aux lettres Exchange à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="c5cee-163">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingCertificate(
    string thumbprint, string certConnectionUri, string schemaUri, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(certConnectionUri),
        schemaUri,
        thumbprint)
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingCertificate( _
    ByVal Thumbprint As String, ByVal CertConnectionUri As String, _
    ByVal SchemaUri As String, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo
    ConnectionInfo = New WSManConnectionInfo(New Uri(CertConnectionUri), SchemaUri, Thumbprint)
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="c5cee-164"><a name="bk_Kerberos"> </a></span><span class="sxs-lookup"><span data-stu-id="c5cee-164"><a name="bk_Kerberos"> </a></span></span>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a><span data-ttu-id="c5cee-165">Se connecter à un espace d’exécution à distance sur un serveur Exchange à l’aide de l’authentification Kerberos</span><span class="sxs-lookup"><span data-stu-id="c5cee-165">Connect to a remote runspace on an Exchange server by using Kerberos authentication</span></span>

<span data-ttu-id="c5cee-166">L’exemple suivant définit la méthode **GetUsersUsingKerberos**, qui crée une instance d’exécution Exchange Management Shell sur un serveur distant à l’aide de l’authentification Kerberos.</span><span class="sxs-lookup"><span data-stu-id="c5cee-166">The following code example defines the **GetUsersUsingKerberos** method, which creates an Exchange Management Shell runspace on a remote server by using Kerberos authentication.</span></span> <span data-ttu-id="c5cee-167">La méthode appelle ensuite la méthode **GetUserInformation** comme décrit à la section [Obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution distante](#bk_remote) pour renvoyer la liste des utilisateurs du serveur distant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-167">The method then calls the **GetUserInformation** method, as defined in the section [Get a list of mailbox users from a remote runspace](#bk_remote), to return a list of users on the remote server.</span></span>
  
<span data-ttu-id="c5cee-168">Cette méthode requiert les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="c5cee-168">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="c5cee-169">**kerberosUri** &ndash; Chaîne qui contient l’URI du serveur Kerberos qui authentifiera l’application.</span><span class="sxs-lookup"><span data-stu-id="c5cee-169">**kerberosUri** &ndash; A string that contains the URI of the Kerberos server that will authenticate the application.</span></span> <span data-ttu-id="c5cee-170">L’URI correspond à l’une des adresses répertoriées dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-170">The URI will be one of those listed in the following table.</span></span> 
    
    <span data-ttu-id="c5cee-171">**Tableau 2. URI kerberosUri**</span><span class="sxs-lookup"><span data-stu-id="c5cee-171">**Table 2. kerberosUri URIs**</span></span>

    |<span data-ttu-id="c5cee-172">**Server**</span><span class="sxs-lookup"><span data-stu-id="c5cee-172">**Server**</span></span>|<span data-ttu-id="c5cee-173">**URI**</span><span class="sxs-lookup"><span data-stu-id="c5cee-173">**URI**</span></span>|
    |:-----|:-----|
    |<span data-ttu-id="c5cee-174">Serveur Exchange sans SSL</span><span class="sxs-lookup"><span data-stu-id="c5cee-174">Exchange server without using SSL</span></span>  <br/> |`http://<servername>/PowerShell`  <br/> |
    |<span data-ttu-id="c5cee-175">Serveur Exchange avec SSL</span><span class="sxs-lookup"><span data-stu-id="c5cee-175">Exchange server using SSL</span></span>  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- <span data-ttu-id="c5cee-176">**schemaUri** &ndash; Chaîne qui contient l’URI du document de schéma qui définit le schéma de l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="c5cee-176">**schemaUri** &ndash; A string that contains the URI of the schema document that defines the Exchange Management Shell schema.</span></span> <span data-ttu-id="c5cee-177">L’URI du schéma est https://schemas.microsoft.com/powershell/Microsoft.Exchange .</span><span class="sxs-lookup"><span data-stu-id="c5cee-177">The schema URI is https://schemas.microsoft.com/powershell/Microsoft.Exchange.</span></span> 
    
- <span data-ttu-id="c5cee-178">**informations d’identification** &ndash; Objet [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) qui contient les informations d’identification de l’utilisateur qui exécute l’application.</span><span class="sxs-lookup"><span data-stu-id="c5cee-178">**credentials** &ndash; A [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) object that contains the credentials of the user who is running the application.</span></span> 
    
- <span data-ttu-id="c5cee-179">**nombre** &ndash; Nombre d’utilisateurs de boîtes aux lettres Exchange à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="c5cee-179">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
```cs
public Collection<PSObject> GetUsersUsingKerberos(
    string kerberosUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(kerberosUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```

```vb
  Function GetUsersUsingKerberos( _
    ByVal KerberosUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(KerberosUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<span data-ttu-id="c5cee-180"><a name="bk_remote"> </a></span><span class="sxs-lookup"><span data-stu-id="c5cee-180"><a name="bk_remote"> </a></span></span>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a><span data-ttu-id="c5cee-181">Obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution distante</span><span class="sxs-lookup"><span data-stu-id="c5cee-181">Get a list of mailbox users from a remote runspace</span></span>

<span data-ttu-id="c5cee-182">L’exemple de code suivant définit la méthode **GetUserInformation** , qui retourne une collection d’instances [PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) qui représentent les utilisateurs de boîte aux lettres Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5cee-182">The following code example defines the **GetUserInformation** method, which returns a collection of [PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) instances that represent Exchange mailbox users.</span></span> <span data-ttu-id="c5cee-183">Cette méthode est appelée par les méthodes **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate** et **GetUsersUsingKerberos** pour renvoyer la liste des utilisateurs à partir du serveur distant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-183">This method is called by the **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**, and **GetUsersUsingKerberos** methods to return the list of users from the remote server.</span></span> 
  
<span data-ttu-id="c5cee-184">Cette méthode requiert les paramètres suivants :</span><span class="sxs-lookup"><span data-stu-id="c5cee-184">This method requires the following parameters:</span></span>
  
- <span data-ttu-id="c5cee-185">**nombre** &ndash; Nombre d’utilisateurs de boîtes aux lettres Exchange à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="c5cee-185">**count** &ndash; The number of Exchange mailbox users to return.</span></span> 
    
- <span data-ttu-id="c5cee-186">**instance d’exécution** &ndash; L’instance d’exécution distante qui est établie pour le serveur Exchange distant.</span><span class="sxs-lookup"><span data-stu-id="c5cee-186">**runspace** &ndash; The remote runspace that is established for the remote Exchange server.</span></span> 
    
```cs
public Collection<PSObject> GetUserInformation(int count, Runspace runspace)
{
    using (PowerShell powershell = PowerShell.Create())
    {
        powershell.AddCommand("Get-Users");
        powershell.AddParameter("ResultSize", count);
        runspace.Open();
        powershell.Runspace = runspace;
        return powershell.Invoke();
    }
}
```

```vb
Function GetUserInformation(ByVal Count As Integer, ByVal RemoteRunspace As Runspace) As Collection(Of PSObject)
    Dim RemotePowerShell As PowerShell = PowerShell.Create
    RemotePowerShell.AddCommand("Get-Users")
    RemotePowerShell.AddParameter("ResultSize", Count)
    ' Open the remote runspace on the server.
    RemoteRunspace.Open()
    ' Associate the runspace with the Exchange Management Shell.
    RemotePowerShell.Runspace = RemoteRunspace
    ' Invoke the Exchange Management Shell to run the command.
    Return RemotePowerShell.Invoke
End Function

```

<span data-ttu-id="c5cee-187">La méthode **GetUserInformation** ne renverra pas plus de _nombre_ d’utilisateurs de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c5cee-187">The **GetUserInformation** method will return no more than  _count_ mailbox users.</span></span> <span data-ttu-id="c5cee-188">Pour simplifier le code de cet exemple, la méthode ne filtre ni ne limite les utilisateurs de boîte aux lettres qui sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="c5cee-188">To simplify the code for this example, the method does not filter or otherwise limit the mailbox users that are returned.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c5cee-189">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c5cee-189">See also</span></span>

- [<span data-ttu-id="c5cee-190">Créer des outils d’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="c5cee-190">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="c5cee-191">Utiliser la réponse de cmdlet de l’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="c5cee-191">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

