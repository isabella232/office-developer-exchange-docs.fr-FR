---
title: Utiliser la réponse de cmdlet de l’environnement de commande Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Découvrez comment utiliser la réponse d’une cmdlet de l’environnement de commande Exchange Management Shell dans votre application managée Exchange.
ms.openlocfilehash: c1b81356ab5dc288ab08287d47581871c36beb05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435701"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a><span data-ttu-id="1d658-103">Utiliser la réponse de cmdlet de l’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="1d658-103">Use the Exchange Management Shell cmdlet response</span></span>

<span data-ttu-id="1d658-104">Découvrez comment utiliser la réponse d’une cmdlet de l’environnement de commande Exchange Management Shell dans votre application managée Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d658-104">Learn how to use the response from an Exchange Management Shell cmdlet in your Exchange managed application.</span></span>
  
<span data-ttu-id="1d658-105">**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="1d658-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="1d658-106">Chaque cmdlet Exchange Management Shell renvoie une ou plusieurs instances [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) qui fournissent une vue cohérente de tout objet dans l’environnement de l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="1d658-106">Each Exchange Management Shell cmdlet returns one or more [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) instances that provide a consistent view of any object in the Exchange Management Shell environment.</span></span> <span data-ttu-id="1d658-107">Cet article fournit des informations sur l’utilisation des propriétés d’une instance **PSObject** pour renvoyer les valeurs de propriété de l’objet de l’API Exchange Server 2013 sous-jacent.</span><span class="sxs-lookup"><span data-stu-id="1d658-107">This article provides information about how to use the properties of a **PSObject** instance to return the property values of the underlying Exchange Server 2013 API object.</span></span> 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a><span data-ttu-id="1d658-108">Conditions préalables à l’utilisation des réponses aux cmdlets</span><span class="sxs-lookup"><span data-stu-id="1d658-108">Prerequisites for using cmdlet responses</span></span>
<span data-ttu-id="1d658-109"><a name="prerequisites_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="1d658-109"><a name="prerequisites_bk"> </a></span></span>

<span data-ttu-id="1d658-110">Pour utiliser les réponses de cmdlet, vous avez besoin d’une référence à l’espace de noms **System. Automation. Management** .</span><span class="sxs-lookup"><span data-stu-id="1d658-110">To use cmdlet responses, you need a reference to the **System.Automation.Management** namespace.</span></span> 
  
> [!NOTE]
>  <span data-ttu-id="1d658-111">Lorsque vous utilisez Visual Studio pour créer une application, vous devez ajouter une référence à l’assembly System. Mangagement. Automation. dll dans le projet.</span><span class="sxs-lookup"><span data-stu-id="1d658-111">When you are using Visual Studio to create an application, you must add a reference to the System.Mangagement.Automation.dll assembly to the project.</span></span> <span data-ttu-id="1d658-112">L’assembly se trouve à l’un des emplacements suivants :</span><span class="sxs-lookup"><span data-stu-id="1d658-112">You can find the assembly in one of the following locations:</span></span> 
> - <span data-ttu-id="1d658-113">Pour les systèmes d’exploitation Windows XP et Windows Vista, le répertoire d’installation de Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="1d658-113">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span> 
> - <span data-ttu-id="1d658-114">Pour les systèmes d’exploitation Windows 7 et Windows 8, le dossier suivant : Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="1d658-114">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
## <a name="windows-powershell-remote-runspace"></a><span data-ttu-id="1d658-115">Instance d’exécution distante Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="1d658-115">Windows PowerShell remote runspace</span></span>
<span data-ttu-id="1d658-116"><a name="usingremoterunspace_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="1d658-116"><a name="usingremoterunspace_bk"> </a></span></span>

<span data-ttu-id="1d658-117">L’environnement de commande Exchange Management Shell utilise des fonctionnalités Windows PowerShell distantes pour toutes les commandes, y compris les commandes exécutées sur le serveur local.</span><span class="sxs-lookup"><span data-stu-id="1d658-117">The Exchange Management Shell uses remote Windows PowerShell features for all commands, even commands that are run on the local server.</span></span> <span data-ttu-id="1d658-118">Par conséquent, toutes les réponses des cmdlets de l’environnement de commande Exchange Management Shell sont sérialisées XML.</span><span class="sxs-lookup"><span data-stu-id="1d658-118">As a result, all responses from Exchange Management Shell cmdlets are serialized XML.</span></span> <span data-ttu-id="1d658-119">Cela signifie que bien que l’objet de réponse indique le type d’objet Exchange qui a été utilisé pour générer la réponse, l’objet de réponse ne peut pas être casté en type d’objet Exchange ; au lieu de cela, vous devez utiliser le conteneur de propriétés qui est exposé par l’objet de réponse pour obtenir les valeurs du type d’objet Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d658-119">This means that although the response object indicates the Exchange object type that was used to generate the response, the response object cannot be cast to the Exchange object type; instead, you must use the property bag that is exposed by the response object to obtain the values from the Exchange object type.</span></span>
  
<span data-ttu-id="1d658-120">Le conteneur des propriétés de l’objet Response contient une paire clé/valeur pour chaque propriété ou méthode publique dans le type d’objet Exchange.</span><span class="sxs-lookup"><span data-stu-id="1d658-120">The property bag in the response object contains a key/value pair for each public property or method in the Exchange object type.</span></span> <span data-ttu-id="1d658-121">L’objet Response contient le nom du type d’objet Exchange sous-jacent ; vous pouvez utiliser ce nom pour déterminer le type d’objet Exchange qui est représenté par l’objet Response afin que vous puissiez extraire la propriété appropriée.</span><span class="sxs-lookup"><span data-stu-id="1d658-121">The response object contains the name of the underlying Exchange object type; you can use this name to determine the Exchange object type that is represented by the response object so that you can extract the appropriate property.</span></span> <span data-ttu-id="1d658-122">Chaque valeur dans le conteneur de propriétés inclut également des informations de type afin que vous puissiez effectuer un cast de la valeur de propriété en type géré approprié.</span><span class="sxs-lookup"><span data-stu-id="1d658-122">Each value in the property bag also includes type information so that you can cast the property value to the appropriate managed type.</span></span>
  
## <a name="use-the-cmdlet-response"></a><span data-ttu-id="1d658-123">Utiliser la réponse de l’applet de commande</span><span class="sxs-lookup"><span data-stu-id="1d658-123">Use the cmdlet response</span></span>
<span data-ttu-id="1d658-124"><a name="usingPSObject_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="1d658-124"><a name="usingPSObject_bk"> </a></span></span>

<span data-ttu-id="1d658-125">La classe [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) expose les trois propriétés publiques suivantes qui contiennent les valeurs de l’objet de l’API Exchange 2013 sous-jacent : [Propriétés](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [méthodes](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)et [membres](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1d658-125">The [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) class exposes the following three public properties that contain the values of the underlying Exchange 2013 API object: [Properties](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [Methods](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx), and [Members](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span></span> <span data-ttu-id="1d658-126">Chaque propriété qui est exposée par l’objet d’API Exchange 2013 possède une paire clé/valeur correspondante dans les propriétés **Propriétés** et **membres** .</span><span class="sxs-lookup"><span data-stu-id="1d658-126">Each property that is exposed by the Exchange 2013 API object has a corresponding key/value pair in the **Properties** and **Members** properties.</span></span> <span data-ttu-id="1d658-127">Votre application peut indexer la collection **Properties** par le nom d’une propriété pour récupérer la valeur de la propriété.</span><span class="sxs-lookup"><span data-stu-id="1d658-127">Your application can index the **Properties** collection by the name of a property to retrieve the value of the property.</span></span> 
  
<span data-ttu-id="1d658-128">Vous pouvez utiliser la propriété **TypeName** de l’instance **PSObject** pour déterminer le type de l’objet Exchange sous-jacent encapsulé par l’instance **PSObject** .</span><span class="sxs-lookup"><span data-stu-id="1d658-128">You can use the **TypeNames** property of the **PSObject** instance to determine the type of the underlying Exchange object that is encapsulated by the **PSObject** instance.</span></span> <span data-ttu-id="1d658-129">La propriété **TypeName** est une collection de chaînes qui contient la hiérarchie d’objets du type représenté.</span><span class="sxs-lookup"><span data-stu-id="1d658-129">The **TypeNames** property is a collection of strings that contains the object hierarchy of the represented type.</span></span> <span data-ttu-id="1d658-130">Vous pouvez utiliser ces noms pour déterminer l’objet représenté par l’instance **PSObject** afin que vous puissiez extraire la propriété appropriée.</span><span class="sxs-lookup"><span data-stu-id="1d658-130">You can use these names to determine the object that is represented by the **PSObject** instance so that you can extract the appropriate property.</span></span> 
  
<span data-ttu-id="1d658-131">L’exemple de code suivant utilise la réponse de l’applet de commande pour imprimer le contenu de la collection de **Propriétés** d’une instance **PSObject** dans la console.</span><span class="sxs-lookup"><span data-stu-id="1d658-131">The following code example uses the cmdlet response to print the contents of the **Properties** collection of a **PSObject** instance on the console.</span></span> <span data-ttu-id="1d658-132">L’exemple de code requiert une référence à l’espace de noms **System. Automation. Management** .</span><span class="sxs-lookup"><span data-stu-id="1d658-132">The code example requires a reference to the **System.Automation.Management** namespace.</span></span> 
  
```cs
foreach (PSPropertyInfo propertyInfo in psObject.Properties)
{
    Console.WriteLine(string.Format("{0}: {1}",
        propertyInfo.Name, propertyInfo.Value);
}
```

<br/>

```vb
For Each PropertyInfo As PSProperty In ObjectInfo.Properties
    Console.WriteLine(String.Format("{0}: {1}", PropertyInfo.Name, PropertyInfo.Value))
Next

```

## <a name="see-also"></a><span data-ttu-id="1d658-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d658-133">See also</span></span>

- [<span data-ttu-id="1d658-134">Créer des outils d’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="1d658-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="1d658-135">Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="1d658-135">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

