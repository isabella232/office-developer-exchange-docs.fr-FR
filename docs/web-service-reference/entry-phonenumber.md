---
title: Entrée (PhoneNumber)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: L’élément Entry représente un numéro de téléphone pour un contact.
ms.openlocfilehash: 62f7091bb750dc7ca74b1e5637a437e2cdad4f1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459636"
---
# <a name="entry-phonenumber"></a><span data-ttu-id="1e9b5-103">Entrée (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="1e9b5-103">Entry (PhoneNumber)</span></span>

<span data-ttu-id="1e9b5-104">L’élément **entry** représente un numéro de téléphone pour un contact.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-104">The **Entry** element represents a telephone number for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="1e9b5-105">**PhoneNumberDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="1e9b5-105">**PhoneNumberDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e9b5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1e9b5-106">Attributes and elements</span></span>

<span data-ttu-id="1e9b5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e9b5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1e9b5-108">Attributes</span></span>

|<span data-ttu-id="1e9b5-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1e9b5-109">**Attribute**</span></span>|<span data-ttu-id="1e9b5-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e9b5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1e9b5-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="1e9b5-111">**Key**</span></span> <br/> | <span data-ttu-id="1e9b5-112">Identifie le numéro de téléphone.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-112">Identifies the telephone number.</span></span> <span data-ttu-id="1e9b5-113">L’attribut key est de type **PhoneNumberKeyType**.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-113">The Key attribute is of type **PhoneNumberKeyType**.</span></span><br/><br/> <span data-ttu-id="1e9b5-114">Les valeurs possibles pour cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="1e9b5-114">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="1e9b5-115">- AssistantPhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-115">-  AssistantPhone</span></span>  <br/><span data-ttu-id="1e9b5-116">- BusinessFax</span><span class="sxs-lookup"><span data-stu-id="1e9b5-116">-  BusinessFax</span></span>  <br/><span data-ttu-id="1e9b5-117">- BusinessPhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-117">-  BusinessPhone</span></span>  <br/><span data-ttu-id="1e9b5-118">- BusinessPhone2</span><span class="sxs-lookup"><span data-stu-id="1e9b5-118">-  BusinessPhone2</span></span>  <br/><span data-ttu-id="1e9b5-119">-Callback</span><span class="sxs-lookup"><span data-stu-id="1e9b5-119">-  Callback</span></span>  <br/><span data-ttu-id="1e9b5-120">- CarPhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-120">-  CarPhone</span></span>  <br/><span data-ttu-id="1e9b5-121">- CompanyMainPhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-121">-  CompanyMainPhone</span></span>  <br/><span data-ttu-id="1e9b5-122">- HomeFax</span><span class="sxs-lookup"><span data-stu-id="1e9b5-122">-  HomeFax</span></span>  <br/><span data-ttu-id="1e9b5-123">-HomePhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-123">-  HomePhone</span></span>  <br/><span data-ttu-id="1e9b5-124">- HomePhone2</span><span class="sxs-lookup"><span data-stu-id="1e9b5-124">-  HomePhone2</span></span>  <br/><span data-ttu-id="1e9b5-125">-RNIS</span><span class="sxs-lookup"><span data-stu-id="1e9b5-125">-  Isdn</span></span>  <br/><span data-ttu-id="1e9b5-126">-MobilePhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-126">-  MobilePhone</span></span>  <br/><span data-ttu-id="1e9b5-127">-OtherFax</span><span class="sxs-lookup"><span data-stu-id="1e9b5-127">-  OtherFax</span></span>  <br/><span data-ttu-id="1e9b5-128">-OtherTelephone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-128">-  OtherTelephone</span></span>  <br/><span data-ttu-id="1e9b5-129">-Récepteur de radiomessagerie</span><span class="sxs-lookup"><span data-stu-id="1e9b5-129">-  Pager</span></span>  <br/><span data-ttu-id="1e9b5-130">- PrimaryPhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-130">-  PrimaryPhone</span></span>  <br/><span data-ttu-id="1e9b5-131">-Radiotéléphone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-131">-  RadioPhone</span></span>  <br/><span data-ttu-id="1e9b5-132">-Télex</span><span class="sxs-lookup"><span data-stu-id="1e9b5-132">-  Telex</span></span>  <br/><span data-ttu-id="1e9b5-133">- TtyTddPhone</span><span class="sxs-lookup"><span data-stu-id="1e9b5-133">-  TtyTddPhone</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1e9b5-134">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1e9b5-134">Child elements</span></span>

<span data-ttu-id="1e9b5-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1e9b5-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1e9b5-136">Parent elements</span></span>

|<span data-ttu-id="1e9b5-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e9b5-137">**Element**</span></span>|<span data-ttu-id="1e9b5-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e9b5-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e9b5-139">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="1e9b5-139">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="1e9b5-140">Représente une collection de numéros de téléphone pour un contact.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-140">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e9b5-141">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1e9b5-141">Text value</span></span>

<span data-ttu-id="1e9b5-142">Une valeur de texte qui représente un numéro de téléphone est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-142">A text value that represents a telephone number is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1e9b5-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="1e9b5-143">Remarks</span></span>

<span data-ttu-id="1e9b5-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1e9b5-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e9b5-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1e9b5-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e9b5-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1e9b5-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e9b5-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1e9b5-147">Schema name</span></span>  <br/> |<span data-ttu-id="1e9b5-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1e9b5-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e9b5-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1e9b5-149">Validation file</span></span>  <br/> |<span data-ttu-id="1e9b5-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1e9b5-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e9b5-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1e9b5-151">Can be empty</span></span>  <br/> |<span data-ttu-id="1e9b5-152">False</span><span class="sxs-lookup"><span data-stu-id="1e9b5-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e9b5-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1e9b5-153">See also</span></span>

- [<span data-ttu-id="1e9b5-154">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1e9b5-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="1e9b5-155">Création de Contacts (Services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="1e9b5-155">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="1e9b5-156">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="1e9b5-156">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="1e9b5-157">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="1e9b5-157">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

