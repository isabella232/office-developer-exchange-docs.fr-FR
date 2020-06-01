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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435701"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Utiliser la réponse de cmdlet de l’environnement de commande Exchange Management Shell

Découvrez comment utiliser la réponse d’une cmdlet de l’environnement de commande Exchange Management Shell dans votre application managée Exchange.
  
**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365
  
Chaque cmdlet Exchange Management Shell renvoie une ou plusieurs instances [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) qui fournissent une vue cohérente de tout objet dans l’environnement de l’environnement de commande Exchange Management Shell. Cet article fournit des informations sur l’utilisation des propriétés d’une instance **PSObject** pour renvoyer les valeurs de propriété de l’objet de l’API Exchange Server 2013 sous-jacent. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Conditions préalables à l’utilisation des réponses aux cmdlets
<a name="prerequisites_bk"> </a>

Pour utiliser les réponses de cmdlet, vous avez besoin d’une référence à l’espace de noms **System. Automation. Management** . 
  
> [!NOTE]
>  Lorsque vous utilisez Visual Studio pour créer une application, vous devez ajouter une référence à l’assembly System. Mangagement. Automation. dll dans le projet. L’assembly se trouve à l’un des emplacements suivants : 
> - Pour les systèmes d’exploitation Windows XP et Windows Vista, le répertoire d’installation de Windows PowerShell ($PSHOME). 
> - Pour les systèmes d’exploitation Windows 7 et Windows 8, le dossier suivant : Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Instance d’exécution distante Windows PowerShell
<a name="usingremoterunspace_bk"> </a>

L’environnement de commande Exchange Management Shell utilise des fonctionnalités Windows PowerShell distantes pour toutes les commandes, y compris les commandes exécutées sur le serveur local. Par conséquent, toutes les réponses des cmdlets de l’environnement de commande Exchange Management Shell sont sérialisées XML. Cela signifie que bien que l’objet de réponse indique le type d’objet Exchange qui a été utilisé pour générer la réponse, l’objet de réponse ne peut pas être casté en type d’objet Exchange ; au lieu de cela, vous devez utiliser le conteneur de propriétés qui est exposé par l’objet de réponse pour obtenir les valeurs du type d’objet Exchange.
  
Le conteneur des propriétés de l’objet Response contient une paire clé/valeur pour chaque propriété ou méthode publique dans le type d’objet Exchange. L’objet Response contient le nom du type d’objet Exchange sous-jacent ; vous pouvez utiliser ce nom pour déterminer le type d’objet Exchange qui est représenté par l’objet Response afin que vous puissiez extraire la propriété appropriée. Chaque valeur dans le conteneur de propriétés inclut également des informations de type afin que vous puissiez effectuer un cast de la valeur de propriété en type géré approprié.
  
## <a name="use-the-cmdlet-response"></a>Utiliser la réponse de l’applet de commande
<a name="usingPSObject_bk"> </a>

La classe [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) expose les trois propriétés publiques suivantes qui contiennent les valeurs de l’objet de l’API Exchange 2013 sous-jacent : [Propriétés](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [méthodes](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)et [membres](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx). Chaque propriété qui est exposée par l’objet d’API Exchange 2013 possède une paire clé/valeur correspondante dans les propriétés **Propriétés** et **membres** . Votre application peut indexer la collection **Properties** par le nom d’une propriété pour récupérer la valeur de la propriété. 
  
Vous pouvez utiliser la propriété **TypeName** de l’instance **PSObject** pour déterminer le type de l’objet Exchange sous-jacent encapsulé par l’instance **PSObject** . La propriété **TypeName** est une collection de chaînes qui contient la hiérarchie d’objets du type représenté. Vous pouvez utiliser ces noms pour déterminer l’objet représenté par l’instance **PSObject** afin que vous puissiez extraire la propriété appropriée. 
  
L’exemple de code suivant utilise la réponse de l’applet de commande pour imprimer le contenu de la collection de **Propriétés** d’une instance **PSObject** dans la console. L’exemple de code requiert une référence à l’espace de noms **System. Automation. Management** . 
  
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

- [Créer des outils d’environnement de commande Exchange Management Shell](create-exchange-management-shell-tools.md)   
- [Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement de commande Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

