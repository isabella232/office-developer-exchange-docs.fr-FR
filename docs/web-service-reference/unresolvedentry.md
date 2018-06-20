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
description: L’élément UnresolvedEntry contient le nom d’une liste de contacts ou de distribution à résoudre.
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838836"
---
# <a name="unresolvedentry"></a><span data-ttu-id="14838-103">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="14838-103">UnresolvedEntry</span></span>

<span data-ttu-id="14838-104">L’élément **UnresolvedEntry** contient le nom d’une liste de contacts ou de distribution à résoudre.</span><span class="sxs-lookup"><span data-stu-id="14838-104">The **UnresolvedEntry** element contains the name of a contact or distribution list to resolve.</span></span> 
  
[<span data-ttu-id="14838-105">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="14838-105">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="14838-106">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="14838-106">UnresolvedEntry</span></span>](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 <span data-ttu-id="14838-107">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="14838-107">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14838-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="14838-108">Attributes and elements</span></span>

<span data-ttu-id="14838-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="14838-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14838-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="14838-110">Attributes</span></span>

<span data-ttu-id="14838-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="14838-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14838-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="14838-112">Child elements</span></span>

<span data-ttu-id="14838-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="14838-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="14838-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="14838-114">Parent elements</span></span>

|<span data-ttu-id="14838-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="14838-115">**Element**</span></span>|<span data-ttu-id="14838-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="14838-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14838-117">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="14838-117">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="14838-118">Définit une demande de résolution de noms ambigus.</span><span class="sxs-lookup"><span data-stu-id="14838-118">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14838-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="14838-119">Text value</span></span>

<span data-ttu-id="14838-120">La valeur de texte représente le nom d’une liste de contacts ou de distribution public.</span><span class="sxs-lookup"><span data-stu-id="14838-120">The text value represents the name of a public contact or distribution list.</span></span> <span data-ttu-id="14838-121">La longueur minimale de la chaîne est un caractère.</span><span class="sxs-lookup"><span data-stu-id="14838-121">The minimum length of the string is one character.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14838-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="14838-122">Remarks</span></span>

<span data-ttu-id="14838-123">La valeur de texte de cet élément est utilisée pour résoudre des noms sur les champs suivants :</span><span class="sxs-lookup"><span data-stu-id="14838-123">The text value of this element is used to resolve names against the following fields:</span></span>
  
- <span data-ttu-id="14838-124">Prénom</span><span class="sxs-lookup"><span data-stu-id="14838-124">First name</span></span>
    
- <span data-ttu-id="14838-125">Nom</span><span class="sxs-lookup"><span data-stu-id="14838-125">Last name</span></span>
    
- <span data-ttu-id="14838-126">Nom d’affichage</span><span class="sxs-lookup"><span data-stu-id="14838-126">Display name</span></span>
    
- <span data-ttu-id="14838-127">Nom complet</span><span class="sxs-lookup"><span data-stu-id="14838-127">Full name</span></span>
    
- <span data-ttu-id="14838-128">Office</span><span class="sxs-lookup"><span data-stu-id="14838-128">Office</span></span>
    
- <span data-ttu-id="14838-129">Alias</span><span class="sxs-lookup"><span data-stu-id="14838-129">Alias</span></span>
    
- <span data-ttu-id="14838-130">adresse SMTP</span><span class="sxs-lookup"><span data-stu-id="14838-130">SMTP address</span></span>
    
<span data-ttu-id="14838-131">Adresses de messagerie avec des types de routage préfixés, tel que smtp ou sip, sont enregistrés dans un tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="14838-131">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="14838-132">L' [opération ResolveNames](resolvenames-operation.md) effectue une correspondance partielle dans chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « sip:User1@Contoso.com ».</span><span class="sxs-lookup"><span data-stu-id="14838-132">The [ResolveNames operation](resolvenames-operation.md) performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="14838-133">Si vous ne spécifiez pas un type de routage, l’opération **ResolveNames** par défaut pour le type de routage du service smtp, faire correspondre à une propriété d’adresse SMTP principale et recherche pas dans le tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="14838-133">If you don't specify a routing type, the **ResolveNames** operation will default to the routing type of smtp, match it to a primary SMTP address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="14838-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="14838-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14838-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="14838-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14838-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="14838-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="14838-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="14838-137">Schema Name</span></span>  <br/> |<span data-ttu-id="14838-138">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="14838-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="14838-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="14838-139">Validation File</span></span>  <br/> |<span data-ttu-id="14838-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="14838-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14838-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="14838-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="14838-142">False</span><span class="sxs-lookup"><span data-stu-id="14838-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14838-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="14838-143">See also</span></span>



[<span data-ttu-id="14838-144">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="14838-144">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="14838-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="14838-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

