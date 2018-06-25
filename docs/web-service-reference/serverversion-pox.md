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
ms.openlocfilehash: ef0562e166094d75d0dd92f5f48bb558e11a2cad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829391"
---
# <a name="serverversion-pox"></a><span data-ttu-id="4ef3f-103">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="4ef3f-103">ServerVersion (POX)</span></span>

<span data-ttu-id="4ef3f-104">L’élément **ServerVersion** représente le numéro de version de l’ordinateur qui exécute Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-104">The **ServerVersion** element represents the version number of the computer that is running Microsoft Exchange Server.</span></span> 
  
- [<span data-ttu-id="4ef3f-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="4ef3f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="4ef3f-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="4ef3f-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="4ef3f-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="4ef3f-107">Account (POX)</span></span>](account-pox.md)
- [<span data-ttu-id="4ef3f-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="4ef3f-108">Protocol (POX)</span></span>](protocol-pox.md)
- [<span data-ttu-id="4ef3f-109">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="4ef3f-109">ServerVersion (POX)</span></span>](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4ef3f-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4ef3f-110">Attributes and elements</span></span>

<span data-ttu-id="4ef3f-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ef3f-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="4ef3f-112">Attributes</span></span>

<span data-ttu-id="4ef3f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ef3f-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4ef3f-114">Child elements</span></span>

<span data-ttu-id="4ef3f-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ef3f-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4ef3f-116">Parent elements</span></span>

|<span data-ttu-id="4ef3f-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4ef3f-117">**Element**</span></span>|<span data-ttu-id="4ef3f-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="4ef3f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ef3f-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="4ef3f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4ef3f-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ef3f-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4ef3f-121">Text value</span></span>

<span data-ttu-id="4ef3f-122">La valeur de texte représente le numéro de version du serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-122">The text value represents the Exchange server version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ef3f-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="4ef3f-123">Remarks</span></span>

<span data-ttu-id="4ef3f-124">La valeur **ServerVersion** est valide uniquement si l’élément de [Type (POX)](type-pox.md) est égal à EXCH ou EXPR.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-124">The **ServerVersion** value is only valid if the [Type (POX)](type-pox.md) element is equal to EXCH or EXPR.</span></span> <span data-ttu-id="4ef3f-125">La valeur **ServerVersion** est un nombre hexadécimal contenant le MajorVersion, MinorVersion et MajorBuildNumber du serveur.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-125">The **ServerVersion** value is a hexadecimal number that contains the MajorVersion, MinorVersion, and MajorBuildNumber of the server.</span></span> 
  
## <a name="example"></a><span data-ttu-id="4ef3f-126">Exemple</span><span class="sxs-lookup"><span data-stu-id="4ef3f-126">Example</span></span>

<span data-ttu-id="4ef3f-127">La suivante convertit exemple un **ServerVersion** valeur qui est retournée dans une réponse de découverte automatique pour obtenir et afficher les MajorVersion, MinorVersion et MajorBuildNumber.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-127">The following example coverts a **ServerVersion** value that is returned in an Autodiscover response to obtain and display the MajorVersion, MinorVersion, and MajorBuildNumber.</span></span> <span data-ttu-id="4ef3f-128">Cet exemple permet d’entrer une valeur hexadécimale pour la valeur **ServerVersion** .</span><span class="sxs-lookup"><span data-stu-id="4ef3f-128">This example enables you to enter a hexadecimal value for the **ServerVersion** value.</span></span> <span data-ttu-id="4ef3f-129">Si aucune valeur **ServerVersion** n’est entré, une valeur par défaut **ServerVersion** 738180DA est utilisée.</span><span class="sxs-lookup"><span data-stu-id="4ef3f-129">If no **ServerVersion** value is entered, a default **ServerVersion** value of 738180DA is used.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="4ef3f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4ef3f-130">See also</span></span>

- [<span data-ttu-id="4ef3f-131">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="4ef3f-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

