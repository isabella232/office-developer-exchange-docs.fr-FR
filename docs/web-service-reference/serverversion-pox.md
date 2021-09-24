---
title: ServerVersion (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a
description: L’élément ServerVersion représente le numéro de version de l’ordinateur qui exécute Microsoft Exchange Server.
ms.openlocfilehash: bc7f9daa62e628e41f7541a609550e90af211928
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527376"
---
# <a name="serverversion-pox"></a>ServerVersion (POX)

**L’élément ServerVersion** représente le numéro de version de l’ordinateur qui exécute Microsoft Exchange Server. 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md)
- [Account (POX)](account-pox.md)
- [Protocol (POX)](protocol-pox.md)
- [ServerVersion (POX)](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange sur qui le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le Exchange de version du serveur.
  
## <a name="remarks"></a>Remarques

La **valeur ServerVersion** n’est valide que si l’élément [Type (POX)](type-pox.md) est égal à EXCH ou EXPR. La **valeur ServerVersion** est un nombre hexadécimal qui contient les valeurs MajorVersion, MinorVersion et MajorBuildNumber du serveur. 
  
## <a name="example"></a>Exemple

L’exemple suivant couvre une valeur **ServerVersion** renvoyée dans une réponse de découverte automatique pour obtenir et afficher les valeurs MajorVersion, MinorVersion et MajorBuildNumber. Cet exemple vous permet d’entrer une valeur hexadécimale pour la **valeur ServerVersion.** Si aucune **valeur ServerVersion** n’est entrée, une valeur **ServerVersion** par défaut de 738180DA est utilisée. 
  
```csharp
static void Main(string[] args)
{
    // Convert a ServerVersion value that is returned from an Autodiscover request.
    // The value is a hex value and can be converted to the MajorVersion, MinorVersion,
    // and MajorBuildNumber.
    Console.WriteLine("Enter ServerVersion returned from the Autodiscover (eg. 738180DA) and Enter.");
    Console.WriteLine("To use the default ServerVersion of 738180DA, just hit Enter.");
    // Get the hexadecimal ServerVersion value.
    string serverversionhex = Console.ReadLine();
    // If nothing is entered, use the default server version of "738180DA"
    if (serverversionhex == "")
    {
        serverversionhex = "738180DA";
    }
    Console.WriteLine("ServerVersion (Hex) = " + serverversionhex);
    string serverversionbinary = Convert.ToString(Convert.ToInt32(serverversionhex, 16), 2);
    // The ServerVersion (binary) should be 32 bits in length. If the 
    // server version in binary is a length of 31 characters, the leading
    // zero has been removed in the conversion process. Put the missing zero back.
    if (serverversionbinary.Length == 31)
    {
        serverversionbinary = String.Concat("0", serverversionbinary);
    }
    Console.WriteLine("ServerVersion (bin) = " + serverversionbinary);
    // The first 4 bits represent a number used for comparison against  
    // older version number structures. You can ignore this.
    // The next 6 bits represent the major version number.
    int majorversion = Convert.ToInt32(serverversionbinary.Substring(4, 6), 2);
    Console.WriteLine("MajorVersion: " + majorversion);
    // The next 6 bits represent the minor version number.
    int minorversion = Convert.ToInt32(serverversionbinary.Substring(10, 6), 2);
    Console.WriteLine("MinorVersion: " + minorversion);
    
    // The next bit represent a flag - you can ignore this.
    // The next 15 bits represent the major build number.
    int majorbuild = Convert.ToInt32(serverversionbinary.Substring(17, 15), 2);
    Console.WriteLine("MajorBuildVersion: " + majorbuild);
    Console.WriteLine("\n\nPress any key to continue");
    Console.ReadKey();
}
```

## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

