---
title: Utiliser la réponse Exchange cmdlet Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Découvrez comment utiliser la réponse d’une cmdlet Exchange Management Shell dans Exchange application gérée.
ms.openlocfilehash: be66be31e435be1553eba16d8f367a79317618f2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520962"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Utiliser la réponse Exchange cmdlet Management Shell

Découvrez comment utiliser la réponse d’une cmdlet Exchange Management Shell dans Exchange application gérée.
  
**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365
  
Chaque Exchange cmdlet Management Shell renvoie une ou plusieurs instances [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) qui fournissent une vue cohérente de n’importe quel objet dans l’environnement Exchange Management Shell. Cet article fournit des informations sur l’utilisation des propriétés d’une instance **PSObject** pour renvoyer les valeurs de propriété de l’objet Exchange Server API 2013 sous-jacent. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Conditions préalables à l’utilisation des réponses de cmdlet
<a name="prerequisites_bk"> </a>

Pour utiliser des réponses de cmdlet, vous avez besoin d’une référence à l’espace de noms **System.Automation.Management.** 
  
> [!NOTE]
>  Lorsque vous utilisez Visual Studio pour créer une application, vous devez ajouter une référence à l’assembly System.Mangagement.Automation.dll au projet. Vous pouvez trouver l’assembly dans l’un des emplacements suivants : 
> - Pour les systèmes d’exploitation Windows XP et Windows Vista, le répertoire d’installation de Windows PowerShell ($PSHOME). 
> - Pour les systèmes d’exploitation Windows 7 et Windows 8, le dossier suivant : Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Windows PowerShell runspace distant
<a name="usingremoterunspace_bk"> </a>

L Exchange Management Shell utilise des fonctionnalités de Windows PowerShell distante pour toutes les commandes, même les commandes qui sont exécutés sur le serveur local. Par conséquent, toutes les réponses des cmdlets Exchange Management Shell sont sérialisées XML. Cela signifie que bien que l’objet de réponse indique le type d’objet Exchange qui Exchange été utilisé pour générer la réponse, l’objet de réponse ne peut pas être casté vers le type d’objet Exchange; Au lieu de cela, vous devez utiliser le sac de propriétés qui est exposé par l’objet de réponse pour obtenir les valeurs du type Exchange’objet.
  
Le sac de propriétés dans l’objet de réponse contient une paire clé/valeur pour chaque propriété ou méthode publique dans le type Exchange’objet. L’objet de réponse contient le nom du type d’Exchange sous-jacent ; vous pouvez utiliser ce nom pour déterminer Exchange type d’objet représenté par l’objet de réponse afin de pouvoir extraire la propriété appropriée. Chaque valeur dans le sac de propriétés inclut également des informations de type afin que vous pouvez caster la valeur de propriété vers le type géré approprié.
  
## <a name="use-the-cmdlet-response"></a>Utiliser la réponse de cmdlet
<a name="usingPSObject_bk"> </a>

La [classe PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) expose les trois propriétés publiques suivantes qui contiennent les valeurs de l’objet API Exchange 2013 sous-jacent : [Propriétés,](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)Méthodes et [Membres.](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx) [](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx) Chaque propriété exposée par l’objet EXCHANGE 2013 possède une paire clé/valeur correspondante dans les propriétés **Properties** et **Members.** Votre application peut indexer la collection **Properties** par le nom d’une propriété pour récupérer la valeur de la propriété. 
  
Vous pouvez utiliser la propriété **TypeNames** de l’instance **PSObject** pour déterminer le type de l’objet Exchange sous-jacent encapsulé par l’instance **PSObject.** La **propriété TypeNames est** une collection de chaînes qui contient la hiérarchie d’objets du type représenté. Vous pouvez utiliser ces noms pour déterminer l’objet représenté par l’instance **PSObject** afin de pouvoir extraire la propriété appropriée. 
  
L’exemple de code suivant utilise la réponse de l’cmdlet pour imprimer le contenu de la collection **Properties** d’une instance **PSObject** sur la console. L’exemple de code requiert une référence à **l’espace de noms System.Automation.Management.** 
  
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

- [Créer des outils d’environnement de ligne de commande Exchange Management Shell](create-exchange-management-shell-tools.md)   
- [Obtenir la liste des utilisateurs de messagerie à l’aide de Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

