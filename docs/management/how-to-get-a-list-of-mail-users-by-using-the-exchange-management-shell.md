---
title: Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Découvrez comment utiliser les applets de commande Exchange Management Shell pour créer un outil qui renvoie la liste des utilisateurs de boîte aux lettres Exchange.
ms.openlocfilehash: 6f64330a11e372bffbea2fcd88bcfa0231ec0f28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755082"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a>Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement Exchange Management Shell

Découvrez comment utiliser les applets de commande Exchange Management Shell pour créer un outil qui renvoie la liste des utilisateurs de boîte aux lettres Exchange.
  
**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365 
  
Obtention d’une liste d’utilisateurs à partir d’Exchange Online, Exchange Online dans le cadre d’Office 365, ou une version d’Exchange commençant par Exchange 2013 à l’aide d’un outil géré qui appelle une applet de commande Exchange Management Shell est un processus en deux étapes. Tout d’abord, vous établissez une instance d’exécution à distance sur un serveur Exchange ; Ensuite, vous exécutez l’applet de commande pour récupérer les informations utilisateur dans l’instance d’exécution à distance. 

Pour vous connecter à l’instance d’exécution à distance, vous devez authentifier auprès du serveur Exchange à l’aide du schéma d’authentification qui répond aux exigences de sécurité de votre organisation. 

Cet article fournit des exemples de code que vous pouvez utiliser pour configurer une instance d’exécution à distance et d’exécuter une applet de commande Exchange Management Shell pour obtenir une liste d’utilisateurs à partir d’un serveur Exchange.

<a name="bk_prerequisites"> </a>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a>Conditions préalables requises pour obtenir une liste d’utilisateurs de boîte aux lettres

Pour effectuer cette tâche, vous avez besoin d’une référence aux espaces de noms suivants :
  
- **System.Collections.ObjectModel**
- **System.Management.Automation**
- **System.Management.Automation.Remoting**
- **System.Management.Automation.Runspaces**
    
> [!NOTE]
>  Lorsque vous utilisez Visual Studio pour créer une application, vous devez ajouter une référence à l’assembly System.Management.Automation.dll vers le projet. Vous trouverez l’assembly dans l’un des emplacements suivants :
> - Pour les systèmes d’exploitation Windows XP et Windows Vista, le répertoire d’installation de Windows PowerShell ($PSHOME).
> - Pour les systèmes d’exploitation Windows 7 et Windows 8, le dossier suivant : Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
Ne chargez pas le composant logiciel enfichable Gestion d’Exchange 2013 dans l’instance d’exécution sur les ordinateurs qui exécutent des applications qui automatisent les applets de commande Exchange Management Shell. L’application doit au lieu de cela créer une instance d’exécution à distance, comme décrit plus loin dans cet article.

<a name="bk_gettinglistmailbox"> </a>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a>Se connecter à une instance d’exécution distante sur un serveur Exchange

La méthode que vous utilisez pour vous connecter à une instance d’exécution distante pour exécuter l’applet de commande Exchange Management Shell varie selon le modèle d’authentification choisi. Cette section fournit des exemples de code qui illustrent la procédure de connexion à une instance d’exécution distante lorsque vous utilisez une méthode d’authentification répertoriée dans le tableau suivant.
  
|**Méthode d’authentification**|**S'applique à**|**URI**|
|:-----|:-----|:-----|
|[Se connecter à une instance d’exécution à distance dans Exchange Online à l’aide de l’authentification de base](#bk_basic) <br/> |Serveurs Exchange Online  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[Se connecter à une instance d’exécution à distance à l’aide de l’authentification par certificat](#bk_cert) <br/> |Exchange Online et serveurs locaux Exchange  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[Se connecter à une instance d’exécution à distance sur un serveur Exchange à l’aide de l’authentification Kerberos](#bk_Kerberos) <br/> |Exchange Online et serveurs locaux Exchange  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<a name="bk_basic"> </a>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a>Se connecter à une instance d’exécution distante sur Exchange Online à l’aide de l’authentification de base

L’exemple de code suivant définit la méthode **GetUsersUsingBasicAuth** , qui crée une instance d’exécution Exchange Management Shell sur un serveur Exchange Online à l’aide de l’authentification de base. La méthode appelle ensuite la méthode **GetUserInformation** , telle que définie dans la section [obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution à distance](#bk_remote), pour renvoyer une liste d’utilisateurs sur le serveur distant.
  
Cette méthode requiert les paramètres suivants :
  
-  **liveIDConnectionUri** &ndash; Une chaîne qui contient l’URI du serveur Exchange Online qui authentifie l’application. Si Exchange Online est en cours d’exécution dans Office 365, l’URI est https://outlook.office365.com/PowerShell-LiveID; Sinon, l’URI est https://\<nom_serveur\>/PowerShell-LiveID. 
    
-  **schemaUri** &ndash; Une chaîne qui contient l’URI du document de schéma qui définit le schéma Exchange Management Shell. Le schéma de l’URI est http://schemas.microsoft.com/powershell/Microsoft.Exchange. 
    
-  **informations d’identification** &ndash; Un objet [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) qui contient les informations d’identification de l’utilisateur qui exécute l’application. 
    
-  **nombre** &ndash; Le nombre d’utilisateurs de boîte aux lettres Exchange à renvoyer. 
    
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

<a name="bk_cert"> </a>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a>Se connecter à une instance d’exécution distante à l’aide de l’authentification des certificats

L’exemple de code suivant définit la méthode **GetUsersUsingCertificate** , qui crée une instance d’exécution Exchange Management Shell sur un serveur distant à l’aide d’un certificat. La méthode appelle ensuite la méthode **GetUserInformation** , telle que définie dans la section [obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution à distance](#bk_remote), pour renvoyer une liste d’utilisateurs sur le serveur distant.
  
Cette méthode requiert les paramètres suivants :
  
-  **empreinte numérique** &ndash; Une chaîne qui contient l’empreinte numérique du certificat qui est utilisé pour authentifier l’application. 
    
-  **certConnectionUri** &ndash; Une chaîne qui contient l’URI du serveur qui authentifie le certificat. L’URI sera une de celles répertoriées dans le tableau suivant. 
    
    **Le tableau 1. certConnectionUri URI**

    |**Serveur**|**URI**|
    |:-----|:-----|
    |Serveur Exchange sans SSL  <br/> |`http://<servername>/PowerShell`  <br/> |
    |Serveur Exchange avec SSL  <br/> |`https://<servername>/PowerShell`  <br/> |
    |Exchange Online dans le cadre d’Office 365  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- **schemaUri** &ndash; Une chaîne qui contient l’URI du document de schéma qui définit le schéma Exchange Management Shell. Le schéma de l’URI est http://schemas.microsoft.com/powershell/Microsoft.Exchange. 
    
- **nombre** &ndash; Le nombre d’utilisateurs de boîte aux lettres Exchange à renvoyer. 
    
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

<a name="bk_Kerberos"> </a>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a>Se connecter à un espace d’exécution à distance sur un serveur Exchange à l’aide de l’authentification Kerberos

L’exemple de code suivant définit la méthode **GetUsersUsingKerberos** , qui crée une instance d’exécution Exchange Management Shell sur un serveur distant à l’aide de l’authentification Kerberos. La méthode appelle ensuite la méthode **GetUserInformation** , telle que définie dans la section [obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution à distance](#bk_remote), pour renvoyer une liste d’utilisateurs sur le serveur distant.
  
Cette méthode requiert les paramètres suivants :
  
- **kerberosUri** &ndash; Une chaîne qui contient l’URI du serveur Kerberos authentifie l’application. L’URI sera une de celles répertoriées dans le tableau suivant. 
    
    **Le tableau 2. kerberosUri URI**

    |**Serveur**|**URI**|
    |:-----|:-----|
    |Serveur Exchange sans SSL  <br/> |`http://<servername>/PowerShell`  <br/> |
    |Serveur Exchange avec SSL  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- **schemaUri** &ndash; Une chaîne qui contient l’URI du document de schéma qui définit le schéma Exchange Management Shell. Le schéma de l’URI est http://schemas.microsoft.com/powershell/Microsoft.Exchange. 
    
- **informations d’identification** &ndash; Un objet [PSCredential](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) qui contient les informations d’identification de l’utilisateur qui exécute l’application. 
    
- **nombre** &ndash; Le nombre d’utilisateurs de boîte aux lettres Exchange à renvoyer. 
    
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

<a name="bk_remote"> </a>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a>Obtenir une liste d’utilisateurs de boîte aux lettres à partir d’une instance d’exécution distante

L’exemple de code suivant définit la méthode **GetUserInformation** , qui retourne une collection d’instances [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.pscredential%28VS.85%29.aspx) qui représentent des utilisateurs de boîte aux lettres Exchange. Cette méthode est appelée par les méthodes **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate**et **GetUsersUsingKerberos** pour renvoyer la liste des utilisateurs à partir du serveur distant. 
  
Cette méthode requiert les paramètres suivants :
  
- **nombre** &ndash; Le nombre d’utilisateurs de boîte aux lettres Exchange à renvoyer. 
    
- **instance d’exécution** &ndash; L’instance d’exécution à distance établie pour le serveur Exchange distant. 
    
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

La méthode **GetUserInformation** ne retournera aucuns plus que le _nombre de_ boîtes aux lettres. Pour simplifier le code de cet exemple, la méthode ne pas filtrer ou autrement limiter les utilisateurs de boîte aux lettres qui sont retournés. 
  
## <a name="see-also"></a>Voir aussi

- [Créer des outils Exchange Management Shell](create-exchange-management-shell-tools.md)   
- [Utilisation de la réponse d’applet de commande Exchange Management Shell](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

