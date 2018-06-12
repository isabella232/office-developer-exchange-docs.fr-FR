---
title: UserSMIMECertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 66e6b4ba-368d-4469-bd47-e59441b7d64d
description: L’élément UserSMIMECertificate contient une valeur qui code certificat SMIME d’un contact.
ms.openlocfilehash: 8b16f6768e3324c6d725a976210b8f7652155bf5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838986"
---
# <a name="usersmimecertificate"></a><span data-ttu-id="05321-103">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="05321-103">UserSMIMECertificate</span></span>

<span data-ttu-id="05321-104">L’élément **UserSMIMECertificate** contient une valeur qui code certificat SMIME d’un contact.</span><span class="sxs-lookup"><span data-stu-id="05321-104">The **UserSMIMECertificate** element contains a value that encodes a contact's SMIME certificate.</span></span> 
  
```XML
<UserSMIMECertificate/>
```

 <span data-ttu-id="05321-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="05321-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05321-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05321-106">Attributes and elements</span></span>

<span data-ttu-id="05321-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05321-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05321-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="05321-108">Attributes</span></span>

<span data-ttu-id="05321-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05321-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05321-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05321-110">Child elements</span></span>

|<span data-ttu-id="05321-111">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="05321-111">**Element name**</span></span>|<span data-ttu-id="05321-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="05321-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05321-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="05321-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="05321-114">Contient une valeur codée en Base64.</span><span class="sxs-lookup"><span data-stu-id="05321-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05321-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05321-115">Parent elements</span></span>

|<span data-ttu-id="05321-116">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="05321-116">**Element name**</span></span>|<span data-ttu-id="05321-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="05321-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05321-118">Contact</span><span class="sxs-lookup"><span data-stu-id="05321-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="05321-119">Représente un élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="05321-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05321-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="05321-120">Text value</span></span>

<span data-ttu-id="05321-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05321-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05321-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="05321-122">Remarks</span></span>

<span data-ttu-id="05321-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="05321-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="05321-124">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="05321-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05321-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05321-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05321-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05321-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05321-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05321-127">Schema name</span></span>  <br/> |<span data-ttu-id="05321-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="05321-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="05321-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05321-129">Validation file</span></span>  <br/> |<span data-ttu-id="05321-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05321-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05321-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05321-131">Can be empty</span></span>  <br/> |<span data-ttu-id="05321-132">False</span><span class="sxs-lookup"><span data-stu-id="05321-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05321-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05321-133">See also</span></span>



- [<span data-ttu-id="05321-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05321-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="05321-135">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="05321-135">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

