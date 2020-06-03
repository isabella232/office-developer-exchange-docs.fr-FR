---
title: UserSMIMECertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 66e6b4ba-368d-4469-bd47-e59441b7d64d
description: L’élément UserSMIMECertificate contient une valeur qui code le certificat SMIME d’un contact.
ms.openlocfilehash: 7e2dbc6a9c8b04758ba99db036e237d8837850aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467654"
---
# <a name="usersmimecertificate"></a><span data-ttu-id="55468-103">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="55468-103">UserSMIMECertificate</span></span>

<span data-ttu-id="55468-104">L’élément **UserSMIMECertificate** contient une valeur qui code le certificat SMIME d’un contact.</span><span class="sxs-lookup"><span data-stu-id="55468-104">The **UserSMIMECertificate** element contains a value that encodes a contact's SMIME certificate.</span></span> 
  
```XML
<UserSMIMECertificate/>
```

 <span data-ttu-id="55468-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="55468-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55468-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55468-106">Attributes and elements</span></span>

<span data-ttu-id="55468-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55468-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55468-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="55468-108">Attributes</span></span>

<span data-ttu-id="55468-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="55468-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55468-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55468-110">Child elements</span></span>

|<span data-ttu-id="55468-111">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="55468-111">**Element name**</span></span>|<span data-ttu-id="55468-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="55468-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55468-113">Au base64Binary</span><span class="sxs-lookup"><span data-stu-id="55468-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="55468-114">Contient une valeur encodée en base 64.</span><span class="sxs-lookup"><span data-stu-id="55468-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55468-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55468-115">Parent elements</span></span>

|<span data-ttu-id="55468-116">**Nom de l'élément**</span><span class="sxs-lookup"><span data-stu-id="55468-116">**Element name**</span></span>|<span data-ttu-id="55468-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="55468-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55468-118">Contact</span><span class="sxs-lookup"><span data-stu-id="55468-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="55468-119">Représente un élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="55468-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55468-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="55468-120">Text value</span></span>

<span data-ttu-id="55468-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55468-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55468-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="55468-122">Remarks</span></span>

<span data-ttu-id="55468-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="55468-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="55468-124">Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="55468-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55468-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55468-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55468-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55468-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55468-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55468-127">Schema name</span></span>  <br/> |<span data-ttu-id="55468-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="55468-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="55468-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55468-129">Validation file</span></span>  <br/> |<span data-ttu-id="55468-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55468-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55468-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55468-131">Can be empty</span></span>  <br/> |<span data-ttu-id="55468-132">False</span><span class="sxs-lookup"><span data-stu-id="55468-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55468-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55468-133">See also</span></span>



- [<span data-ttu-id="55468-134">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="55468-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="55468-135">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="55468-135">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

