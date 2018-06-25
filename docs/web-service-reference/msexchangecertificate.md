---
title: MSExchangeCertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c514f22f-be3e-4cad-ac56-bdff6bafcee6
description: L’élément MSExchangeCertificate contient une valeur qui encode le certificat Microsoft Exchange d’un contact.
ms.openlocfilehash: 8d07198012485b5c6d22e1fb4721890bf9a5eb39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828498"
---
# <a name="msexchangecertificate"></a><span data-ttu-id="e6101-103">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="e6101-103">MSExchangeCertificate</span></span>

<span data-ttu-id="e6101-104">L’élément **MSExchangeCertificate** contient une valeur qui encode le certificat Microsoft Exchange d’un contact.</span><span class="sxs-lookup"><span data-stu-id="e6101-104">The **MSExchangeCertificate** element contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span> 
  
```XML
<MSExchangeCertificate/>
```

 <span data-ttu-id="e6101-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="e6101-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6101-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e6101-106">Attributes and elements</span></span>

<span data-ttu-id="e6101-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e6101-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6101-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e6101-108">Attributes</span></span>

<span data-ttu-id="e6101-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e6101-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6101-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e6101-110">Child elements</span></span>

|<span data-ttu-id="e6101-111">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="e6101-111">**Element name**</span></span>|<span data-ttu-id="e6101-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e6101-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6101-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="e6101-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="e6101-114">Contient une valeur codée en Base64.</span><span class="sxs-lookup"><span data-stu-id="e6101-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6101-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e6101-115">Parent elements</span></span>

|<span data-ttu-id="e6101-116">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="e6101-116">**Element name**</span></span>|<span data-ttu-id="e6101-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e6101-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6101-118">Contact</span><span class="sxs-lookup"><span data-stu-id="e6101-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="e6101-119">Représente un élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6101-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e6101-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e6101-120">Text value</span></span>

<span data-ttu-id="e6101-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e6101-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e6101-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="e6101-122">Remarks</span></span>

<span data-ttu-id="e6101-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6101-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="e6101-124">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="e6101-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6101-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e6101-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6101-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e6101-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6101-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e6101-127">Schema name</span></span>  <br/> |<span data-ttu-id="e6101-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e6101-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6101-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e6101-129">Validation file</span></span>  <br/> |<span data-ttu-id="e6101-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e6101-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6101-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e6101-131">Can be empty</span></span>  <br/> |<span data-ttu-id="e6101-132">False</span><span class="sxs-lookup"><span data-stu-id="e6101-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6101-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e6101-133">See also</span></span>



- [<span data-ttu-id="e6101-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e6101-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e6101-135">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="e6101-135">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

