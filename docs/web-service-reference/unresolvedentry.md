---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: L’élément UnresolvedEntry contient le nom d’un contact ou d’une liste de distribution à résoudre.
ms.openlocfilehash: 0f157c1be6c327187456a795c4c1000b8c35b620
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459839"
---
# <a name="unresolvedentry"></a><span data-ttu-id="00795-103">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="00795-103">UnresolvedEntry</span></span>

<span data-ttu-id="00795-104">L’élément **UnresolvedEntry** contient le nom d’un contact ou d’une liste de distribution à résoudre.</span><span class="sxs-lookup"><span data-stu-id="00795-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="00795-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="00795-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="00795-106">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="00795-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="00795-107">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="00795-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00795-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00795-108">Attributes and elements</span></span>

<span data-ttu-id="00795-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00795-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00795-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="00795-110">Attributes</span></span>

<span data-ttu-id="00795-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00795-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00795-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00795-112">Child elements</span></span>

<span data-ttu-id="00795-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00795-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00795-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00795-114">Parent elements</span></span>

|<span data-ttu-id="00795-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00795-115">**Element**</span></span>|<span data-ttu-id="00795-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="00795-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00795-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="00795-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="00795-118">Définit une demande de résolution de noms ambigus.</span><span class="sxs-lookup"><span data-stu-id="00795-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00795-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="00795-119">Text value</span></span>

<span data-ttu-id="00795-120">La valeur de texte représente le nom d’un contact public ou d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="00795-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="00795-121">La longueur minimale de la chaîne est d’un caractère.</span><span class="sxs-lookup"><span data-stu-id="00795-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00795-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="00795-122">Remarks</span></span>

<span data-ttu-id="00795-123">La valeur de texte de cet élément est utilisée pour résoudre les noms par rapport aux champs suivants :</span><span class="sxs-lookup"><span data-stu-id="00795-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="00795-124">Prénom</span><span class="sxs-lookup"><span data-stu-id="00795-124">First name</span></span>
    
- <span data-ttu-id="00795-125">Nom de famille</span><span class="sxs-lookup"><span data-stu-id="00795-125">Last name</span></span>
    
- <span data-ttu-id="00795-126">Nom unique (DN)</span><span class="sxs-lookup"><span data-stu-id="00795-126">Display name</span></span>
    
- <span data-ttu-id="00795-127">Nom complet</span><span class="sxs-lookup"><span data-stu-id="00795-127">Full name</span></span>
    
- <span data-ttu-id="00795-128">Office</span><span class="sxs-lookup"><span data-stu-id="00795-128">Office</span></span>
    
- <span data-ttu-id="00795-129">Alias</span><span class="sxs-lookup"><span data-stu-id="00795-129">Alias</span></span>
    
- <span data-ttu-id="00795-130">Adresse SMTP</span><span class="sxs-lookup"><span data-stu-id="00795-130">SMTP address</span></span>
    
<span data-ttu-id="00795-131">Les adresses de messagerie avec des types de routage préfixés, tels que SMTP ou SIP, sont enregistrées dans un tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="00795-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="00795-132">L' [opération ResolveNames](resolvenames-operation.md) effectue une correspondance partielle par rapport à chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « SIP :User1@Contoso.com ».</span><span class="sxs-lookup"><span data-stu-id="00795-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="00795-133">Si vous ne spécifiez pas de type de routage, l’opération **ResolveNames** prend par défaut le type de routage SMTP, le associe à une propriété d’adresse SMTP principale, et non à la recherche dans le tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="00795-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="00795-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="00795-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00795-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00795-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00795-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00795-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00795-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00795-137">Schema Name</span></span>  <br/> |<span data-ttu-id="00795-138">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="00795-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="00795-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00795-139">Validation File</span></span>  <br/> |<span data-ttu-id="00795-140">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="00795-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00795-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00795-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="00795-142">False</span><span class="sxs-lookup"><span data-stu-id="00795-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00795-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00795-143">See also</span></span>



[<span data-ttu-id="00795-144">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="00795-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="00795-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00795-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

