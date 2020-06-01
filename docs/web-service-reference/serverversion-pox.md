---
title: ServerVersion (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a
description: L’élément ServerVersion représente le numéro de version de l’ordinateur qui exécute Microsoft Exchange Server.
ms.openlocfilehash: 3ef531a69d2dd00ee9784c9eb191684ce517e842
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461967"
---
# <a name="serverversion-pox"></a><span data-ttu-id="29f94-103">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="29f94-103">ServerVersion (POX)</span></span>

<span data-ttu-id="29f94-104">L’élément **ServerVersion** représente le numéro de version de l’ordinateur qui exécute Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="29f94-104">The **ServerVersion** element represents the version number of the computer that is running Microsoft Exchange Server.</span></span> 
  
- [<span data-ttu-id="29f94-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="29f94-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="29f94-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="29f94-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="29f94-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="29f94-107">Account (POX)</span></span>](account-pox.md)
- [<span data-ttu-id="29f94-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="29f94-108">Protocol (POX)</span></span>](protocol-pox.md)
- [<span data-ttu-id="29f94-109">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="29f94-109">ServerVersion (POX)</span></span>](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="29f94-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="29f94-110">Attributes and elements</span></span>

<span data-ttu-id="29f94-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="29f94-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29f94-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="29f94-112">Attributes</span></span>

<span data-ttu-id="29f94-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="29f94-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29f94-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="29f94-114">Child elements</span></span>

<span data-ttu-id="29f94-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="29f94-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29f94-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="29f94-116">Parent elements</span></span>

|<span data-ttu-id="29f94-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29f94-117">**Element**</span></span>|<span data-ttu-id="29f94-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="29f94-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29f94-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="29f94-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="29f94-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="29f94-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="29f94-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="29f94-121">Text value</span></span>

<span data-ttu-id="29f94-122">La valeur texte représente le numéro de version d’Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="29f94-122">The text value represents the Exchange server version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="29f94-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="29f94-123">Remarks</span></span>

<span data-ttu-id="29f94-124">La valeur **ServerVersion** est valide uniquement si l’élément [type (POX)](type-pox.md) est égal à Exch ou Expr.</span><span class="sxs-lookup"><span data-stu-id="29f94-124">The **ServerVersion** value is only valid if the [Type (POX)](type-pox.md) element is equal to EXCH or EXPR.</span></span> <span data-ttu-id="29f94-125">La valeur **ServerVersion** est un nombre hexadécimal qui contient les valeurs MajorVersion, MinorVersion et MajorBuildNumber du serveur.</span><span class="sxs-lookup"><span data-stu-id="29f94-125">The **ServerVersion** value is a hexadecimal number that contains the MajorVersion, MinorVersion, and MajorBuildNumber of the server.</span></span> 
  
## <a name="example"></a><span data-ttu-id="29f94-126">Exemple</span><span class="sxs-lookup"><span data-stu-id="29f94-126">Example</span></span>

<span data-ttu-id="29f94-127">L’exemple suivant permet d’extraire une valeur **ServerVersion** qui est renvoyée dans une réponse de découverte automatique pour obtenir et afficher les options MajorVersion, MinorVersion et MajorBuildNumber.</span><span class="sxs-lookup"><span data-stu-id="29f94-127">The following example coverts a **ServerVersion** value that is returned in an Autodiscover response to obtain and display the MajorVersion, MinorVersion, and MajorBuildNumber.</span></span> <span data-ttu-id="29f94-128">Cet exemple vous permet d’entrer une valeur hexadécimale pour la valeur **ServerVersion** .</span><span class="sxs-lookup"><span data-stu-id="29f94-128">This example enables you to enter a hexadecimal value for the **ServerVersion** value.</span></span> <span data-ttu-id="29f94-129">Si aucune valeur **ServerVersion** n’est entrée, une valeur **ServerVersion** par défaut de 738180DA est utilisée.</span><span class="sxs-lookup"><span data-stu-id="29f94-129">If no **ServerVersion** value is entered, a default **ServerVersion** value of 738180DA is used.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="29f94-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="29f94-130">See also</span></span>

- [<span data-ttu-id="29f94-131">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="29f94-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

