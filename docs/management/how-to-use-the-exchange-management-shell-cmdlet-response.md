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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755078"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Utilisation de la réponse d’applet de commande Exchange Management Shell

Découvrez comment utiliser la réponse à partir d’une applet de commande Exchange Management Shell dans votre application Exchange géré.
  
**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365
  
Chaque applet de commande Exchange Management Shell renvoie une ou plusieurs instances [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) qui fournissent une vue cohérente de n’importe quel objet dans l’environnement Exchange Management Shell. Cet article fournit des informations sur la façon d’utiliser les propriétés d’une instance de **PSObject** pour renvoyer les valeurs de propriété de l’objet d’API d’Exchange Server 2013 sous-jacent. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Conditions préalables à l’aide de réponses de l’applet de commande
<a name="prerequisites_bk"> </a>

Pour utiliser les réponses de l’applet de commande, vous avez besoin d’une référence à l’espace de noms **System.Automation.Management** . 
  
> [!NOTE]
>  Lorsque vous utilisez Visual Studio pour créer une application, vous devez ajouter une référence à l’assembly System.Mangagement.Automation.dll au projet. Vous pouvez trouver l’assembly dans un des emplacements suivants : 
> - Pour les systèmes d’exploitation Windows XP et Windows Vista, le répertoire d’installation de Windows PowerShell ($PSHOME). 
> - Pour les systèmes d’exploitation Windows 7 et Windows 8, le dossier suivant : Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Instance d’exécution à distance Windows PowerShell
<a name="usingremoterunspace_bk"> </a>

Exchange Management Shell utilise les fonctionnalités de Windows PowerShell à distance pour toutes les commandes, même les commandes qui sont exécutés sur le serveur local. Par conséquent, toutes les réponses des applets de commande Exchange Management Shell sérialisées XML. Cela signifie que bien que l’objet de réponse indique le type d’objet Exchange qui a été utilisé pour générer la réponse, l’objet de réponse ne peut pas être convertie pour le type d’objet Exchange ; au lieu de cela, vous devez utiliser le conteneur de propriétés qui est exposé par l’objet response pour obtenir les valeurs du type d’objet Exchange.
  
Le conteneur des propriétés de l’objet de la réponse contient une paire clé/valeur pour chaque propriété publique ou d’une méthode dans le type d’objet Exchange. L’objet de réponse contient le nom du type d’objet sous-jacent Exchange ; Vous pouvez utiliser ce nom pour déterminer le type d’objet Exchange qui est représenté par l’objet de réponse afin que vous pouvez extraire la propriété appropriée. Chaque valeur dans le conteneur de propriétés consacrée également des informations de type afin que vous pouvez effectuer un cast de la valeur de propriété pour le type managé approprié.
  
## <a name="use-the-cmdlet-response"></a>Utilisation de la réponse de l’applet de commande
<a name="usingPSObject_bk"> </a>

La classe [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) expose les propriétés publiques trois suivantes qui contiennent les valeurs de l’objet Exchange 2013 API sous-jacent : [Propriétés](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [méthodes](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)et [les membres](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx). Chaque propriété exposée par l’objet Exchange 2013 API possède une paire clé/valeur correspondante dans les propriétés de **Propriétés** et des **membres** . Votre application peut indexer la collection **Properties** du nom d’une propriété pour récupérer la valeur de la propriété. 
  
Vous pouvez utiliser la propriété **TypeNames** de l’instance **PSObject** pour déterminer le type de l’objet Exchange sous-jacent encapsulé par l’instance **PSObject** . La propriété **TypeNames** est une collection de chaînes qui contient la hiérarchie d’objets de type représenté. Vous pouvez utiliser ces noms pour déterminer l’objet qui est représenté par l’instance **PSObject** afin que vous pouvez extraire la propriété appropriée. 
  
L’exemple de code suivant utilise la réponse de l’applet de commande pour imprimer le contenu de la collection de **Propriétés** d’une instance de **PSObject** sur la console. L’exemple de code requiert une référence à l’espace de noms **System.Automation.Management** . 
  
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

## <a name="see-also"></a>Voir aussi

- [Créer des outils Exchange Management Shell](create-exchange-management-shell-tools.md)   
- [Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

