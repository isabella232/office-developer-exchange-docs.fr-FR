---
title: Utilisation de la réponse d’applet de commande Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Découvrez comment utiliser la réponse à partir d’une applet de commande Exchange Management Shell dans votre application Exchange géré.
ms.openlocfilehash: 5edf75afd556f67e815bc519c87586f2f62f057b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755078"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a><span data-ttu-id="d266d-103">Utilisation de la réponse d’applet de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d266d-103">Use the Exchange Management Shell cmdlet response</span></span>

<span data-ttu-id="d266d-104">Découvrez comment utiliser la réponse à partir d’une applet de commande Exchange Management Shell dans votre application Exchange géré.</span><span class="sxs-lookup"><span data-stu-id="d266d-104">Learn how to use the response from an Exchange Management Shell cmdlet in your Exchange managed application.</span></span>
  
<span data-ttu-id="d266d-105">**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="d266d-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="d266d-106">Chaque applet de commande Exchange Management Shell renvoie une ou plusieurs instances [PSObject](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject%28VS.85%29.aspx) qui fournissent une vue cohérente de n’importe quel objet dans l’environnement Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="d266d-106">Each Exchange Management Shell cmdlet returns one or more [PSObject](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject%28VS.85%29.aspx) instances that provide a consistent view of any object in the Exchange Management Shell environment.</span></span> <span data-ttu-id="d266d-107">Cet article fournit des informations sur la façon d’utiliser les propriétés d’une instance de **PSObject** pour renvoyer les valeurs de propriété de l’objet d’API d’Exchange Server 2013 sous-jacent.</span><span class="sxs-lookup"><span data-stu-id="d266d-107">This article provides information about how to use the properties of a **PSObject** instance to return the property values of the underlying Exchange Server 2013 API object.</span></span> 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a><span data-ttu-id="d266d-108">Conditions préalables à l’aide de réponses de l’applet de commande</span><span class="sxs-lookup"><span data-stu-id="d266d-108">Prerequisites for using cmdlet responses</span></span>
<span data-ttu-id="d266d-109"><a name="prerequisites_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="d266d-109"></span></span>

<span data-ttu-id="d266d-110">Pour utiliser les réponses de l’applet de commande, vous avez besoin d’une référence à l’espace de noms **System.Automation.Management** .</span><span class="sxs-lookup"><span data-stu-id="d266d-110">To use cmdlet responses, you need a reference to the **System.Automation.Management** namespace.</span></span> 
  
> [!NOTE]
>  <span data-ttu-id="d266d-111">Lorsque vous utilisez Visual Studio pour créer une application, vous devez ajouter une référence à l’assembly System.Mangagement.Automation.dll au projet.</span><span class="sxs-lookup"><span data-stu-id="d266d-111">When you are using Visual Studio to create an application, you must add a reference to the System.Mangagement.Automation.dll assembly to the project.</span></span> <span data-ttu-id="d266d-112">Vous pouvez trouver l’assembly dans un des emplacements suivants :</span><span class="sxs-lookup"><span data-stu-id="d266d-112">You can find the assembly in one of the following locations:</span></span> 
> - <span data-ttu-id="d266d-113">Pour les systèmes d’exploitation Windows XP et Windows Vista, le répertoire d’installation de Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="d266d-113">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span> 
> - <span data-ttu-id="d266d-114">Pour les systèmes d’exploitation Windows 7 et Windows 8, le dossier suivant : Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="d266d-114">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
## <a name="windows-powershell-remote-runspace"></a><span data-ttu-id="d266d-115">Instance d’exécution à distance Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="d266d-115">Windows PowerShell remote runspace</span></span>
<span data-ttu-id="d266d-116"><a name="usingremoterunspace_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="d266d-116"></span></span>

<span data-ttu-id="d266d-117">Exchange Management Shell utilise les fonctionnalités de Windows PowerShell à distance pour toutes les commandes, même les commandes qui sont exécutés sur le serveur local.</span><span class="sxs-lookup"><span data-stu-id="d266d-117">The Exchange Management Shell uses remote Windows PowerShell features for all commands, even commands that are run on the local server.</span></span> <span data-ttu-id="d266d-118">Par conséquent, toutes les réponses des applets de commande Exchange Management Shell sérialisées XML.</span><span class="sxs-lookup"><span data-stu-id="d266d-118">As a result, all responses from Exchange Management Shell cmdlets are serialized XML.</span></span> <span data-ttu-id="d266d-119">Cela signifie que bien que l’objet de réponse indique le type d’objet Exchange qui a été utilisé pour générer la réponse, l’objet de réponse ne peut pas être convertie pour le type d’objet Exchange ; au lieu de cela, vous devez utiliser le conteneur de propriétés qui est exposé par l’objet response pour obtenir les valeurs du type d’objet Exchange.</span><span class="sxs-lookup"><span data-stu-id="d266d-119">This means that although the response object indicates the Exchange object type that was used to generate the response, the response object cannot be cast to the Exchange object type; instead, you must use the property bag that is exposed by the response object to obtain the values from the Exchange object type.</span></span>
  
<span data-ttu-id="d266d-120">Le conteneur des propriétés de l’objet de la réponse contient une paire clé/valeur pour chaque propriété publique ou d’une méthode dans le type d’objet Exchange.</span><span class="sxs-lookup"><span data-stu-id="d266d-120">The property bag in the response object contains a key/value pair for each public property or method in the Exchange object type.</span></span> <span data-ttu-id="d266d-121">L’objet de réponse contient le nom du type d’objet sous-jacent Exchange ; Vous pouvez utiliser ce nom pour déterminer le type d’objet Exchange qui est représenté par l’objet de réponse afin que vous pouvez extraire la propriété appropriée.</span><span class="sxs-lookup"><span data-stu-id="d266d-121">The response object contains the name of the underlying Exchange object type; you can use this name to determine the Exchange object type that is represented by the response object so that you can extract the appropriate property.</span></span> <span data-ttu-id="d266d-122">Chaque valeur dans le conteneur de propriétés consacrée également des informations de type afin que vous pouvez effectuer un cast de la valeur de propriété pour le type managé approprié.</span><span class="sxs-lookup"><span data-stu-id="d266d-122">Each value in the property bag also includes type information so that you can cast the property value to the appropriate managed type.</span></span>
  
## <a name="use-the-cmdlet-response"></a><span data-ttu-id="d266d-123">Utilisation de la réponse de l’applet de commande</span><span class="sxs-lookup"><span data-stu-id="d266d-123">Use the cmdlet response</span></span>
<span data-ttu-id="d266d-124"><a name="usingPSObject_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="d266d-124"></span></span>

<span data-ttu-id="d266d-125">La classe [PSObject](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject%28VS.85%29.aspx) expose les propriétés publiques trois suivantes qui contiennent les valeurs de l’objet Exchange 2013 API sous-jacent : [Propriétés](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [méthodes](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject.methods%28VS.85%29.aspx)et [les membres](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d266d-125">The [PSObject](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject%28VS.85%29.aspx) class exposes the following three public properties that contain the values of the underlying Exchange 2013 API object: [Properties](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [Methods](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject.methods%28VS.85%29.aspx), and [Members](http://msdn.microsoft.com/fr-fr/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span></span> <span data-ttu-id="d266d-126">Chaque propriété exposée par l’objet Exchange 2013 API possède une paire clé/valeur correspondante dans les propriétés de **Propriétés** et des **membres** .</span><span class="sxs-lookup"><span data-stu-id="d266d-126">Each property that is exposed by the Exchange 2013 API object has a corresponding key/value pair in the **Properties** and **Members** properties.</span></span> <span data-ttu-id="d266d-127">Votre application peut indexer la collection **Properties** du nom d’une propriété pour récupérer la valeur de la propriété.</span><span class="sxs-lookup"><span data-stu-id="d266d-127">Your application can index the **Properties** collection by the name of a property to retrieve the value of the property.</span></span> 
  
<span data-ttu-id="d266d-128">Vous pouvez utiliser la propriété **TypeNames** de l’instance **PSObject** pour déterminer le type de l’objet Exchange sous-jacent encapsulé par l’instance **PSObject** .</span><span class="sxs-lookup"><span data-stu-id="d266d-128">You can use the **TypeNames** property of the **PSObject** instance to determine the type of the underlying Exchange object that is encapsulated by the **PSObject** instance.</span></span> <span data-ttu-id="d266d-129">La propriété **TypeNames** est une collection de chaînes qui contient la hiérarchie d’objets de type représenté.</span><span class="sxs-lookup"><span data-stu-id="d266d-129">The **TypeNames** property is a collection of strings that contains the object hierarchy of the represented type.</span></span> <span data-ttu-id="d266d-130">Vous pouvez utiliser ces noms pour déterminer l’objet qui est représenté par l’instance **PSObject** afin que vous pouvez extraire la propriété appropriée.</span><span class="sxs-lookup"><span data-stu-id="d266d-130">You can use these names to determine the object that is represented by the **PSObject** instance so that you can extract the appropriate property.</span></span> 
  
<span data-ttu-id="d266d-131">L’exemple de code suivant utilise la réponse de l’applet de commande pour imprimer le contenu de la collection de **Propriétés** d’une instance de **PSObject** sur la console.</span><span class="sxs-lookup"><span data-stu-id="d266d-131">The following code example uses the cmdlet response to print the contents of the **Properties** collection of a **PSObject** instance on the console.</span></span> <span data-ttu-id="d266d-132">L’exemple de code requiert une référence à l’espace de noms **System.Automation.Management** .</span><span class="sxs-lookup"><span data-stu-id="d266d-132">The code example requires a reference to the **System.Automation.Management** namespace.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="d266d-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d266d-133">See also</span></span>

- [<span data-ttu-id="d266d-134">Créer des outils Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d266d-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="d266d-135">Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d266d-135">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

