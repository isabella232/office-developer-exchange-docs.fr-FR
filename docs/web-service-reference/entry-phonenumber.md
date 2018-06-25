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
description: L’élément d’entrée représente un numéro de téléphone d’un contact.
ms.openlocfilehash: 3953488fb0b57fcf01c2fb99039478bbe03c7f5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756201"
---
# <a name="entry-phonenumber"></a><span data-ttu-id="3716c-103">Entrée (PhoneNumber)</span><span class="sxs-lookup"><span data-stu-id="3716c-103">Entry (PhoneNumber)</span></span>

<span data-ttu-id="3716c-104">L’élément **d’entrée** représente un numéro de téléphone d’un contact.</span><span class="sxs-lookup"><span data-stu-id="3716c-104">The **Entry** element represents a telephone number for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="3716c-105">**PhoneNumberDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="3716c-105">**PhoneNumberDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3716c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3716c-106">Attributes and elements</span></span>

<span data-ttu-id="3716c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3716c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3716c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3716c-108">Attributes</span></span>

|<span data-ttu-id="3716c-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="3716c-109">**Attribute**</span></span>|<span data-ttu-id="3716c-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="3716c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3716c-111">**Clé**</span><span class="sxs-lookup"><span data-stu-id="3716c-111">**Key**</span></span> <br/> | <span data-ttu-id="3716c-112">Identifie le numéro de téléphone.</span><span class="sxs-lookup"><span data-stu-id="3716c-112">Identifies the telephone number.</span></span> <span data-ttu-id="3716c-113">L’attribut Key est de type **PhoneNumberKeyType**.</span><span class="sxs-lookup"><span data-stu-id="3716c-113">The Key attribute is of type **PhoneNumberKeyType**.</span></span><br/><br/> <span data-ttu-id="3716c-114">Les valeurs possibles de cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="3716c-114">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="3716c-115">-AssistantPhone</span><span class="sxs-lookup"><span data-stu-id="3716c-115">-  AssistantPhone</span></span>  <br/><span data-ttu-id="3716c-116">-BusinessFax</span><span class="sxs-lookup"><span data-stu-id="3716c-116">-  BusinessFax</span></span>  <br/><span data-ttu-id="3716c-117">-BusinessPhone</span><span class="sxs-lookup"><span data-stu-id="3716c-117">-  BusinessPhone</span></span>  <br/><span data-ttu-id="3716c-118">-BusinessPhone2</span><span class="sxs-lookup"><span data-stu-id="3716c-118">-  BusinessPhone2</span></span>  <br/><span data-ttu-id="3716c-119">-Rappel</span><span class="sxs-lookup"><span data-stu-id="3716c-119">-  Callback</span></span>  <br/><span data-ttu-id="3716c-120">-Téléphone de voiture</span><span class="sxs-lookup"><span data-stu-id="3716c-120">-  CarPhone</span></span>  <br/><span data-ttu-id="3716c-121">-CompanyMainPhone</span><span class="sxs-lookup"><span data-stu-id="3716c-121">-  CompanyMainPhone</span></span>  <br/><span data-ttu-id="3716c-122">-Télécopie personnelle</span><span class="sxs-lookup"><span data-stu-id="3716c-122">-  HomeFax</span></span>  <br/><span data-ttu-id="3716c-123">-HomePhone</span><span class="sxs-lookup"><span data-stu-id="3716c-123">-  HomePhone</span></span>  <br/><span data-ttu-id="3716c-124">-HomePhone2</span><span class="sxs-lookup"><span data-stu-id="3716c-124">-  HomePhone2</span></span>  <br/><span data-ttu-id="3716c-125">-RNIS</span><span class="sxs-lookup"><span data-stu-id="3716c-125">-  Isdn</span></span>  <br/><span data-ttu-id="3716c-126">-MobilePhone</span><span class="sxs-lookup"><span data-stu-id="3716c-126">-  MobilePhone</span></span>  <br/><span data-ttu-id="3716c-127">-OtherFax</span><span class="sxs-lookup"><span data-stu-id="3716c-127">-  OtherFax</span></span>  <br/><span data-ttu-id="3716c-128">-OtherTelephone</span><span class="sxs-lookup"><span data-stu-id="3716c-128">-  OtherTelephone</span></span>  <br/><span data-ttu-id="3716c-129">-Récepteur de radiomessagerie</span><span class="sxs-lookup"><span data-stu-id="3716c-129">-  Pager</span></span>  <br/><span data-ttu-id="3716c-130">-PrimaryPhone</span><span class="sxs-lookup"><span data-stu-id="3716c-130">-  PrimaryPhone</span></span>  <br/><span data-ttu-id="3716c-131">-RadioPhone</span><span class="sxs-lookup"><span data-stu-id="3716c-131">-  RadioPhone</span></span>  <br/><span data-ttu-id="3716c-132">-Télex</span><span class="sxs-lookup"><span data-stu-id="3716c-132">-  Telex</span></span>  <br/><span data-ttu-id="3716c-133">-TtyTddPhone</span><span class="sxs-lookup"><span data-stu-id="3716c-133">-  TtyTddPhone</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3716c-134">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3716c-134">Child elements</span></span>

<span data-ttu-id="3716c-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3716c-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3716c-136">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3716c-136">Parent elements</span></span>

|<span data-ttu-id="3716c-137">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3716c-137">**Element**</span></span>|<span data-ttu-id="3716c-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="3716c-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3716c-139">PhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="3716c-139">PhoneNumbers</span></span>](phonenumbers.md) <br/> |<span data-ttu-id="3716c-140">Représente une collection de numéros de téléphone pour un contact.</span><span class="sxs-lookup"><span data-stu-id="3716c-140">Represents a collection of telephone numbers for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3716c-141">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3716c-141">Text value</span></span>

<span data-ttu-id="3716c-142">Une valeur de texte qui représente un numéro de téléphone est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="3716c-142">A text value that represents a telephone number is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3716c-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="3716c-143">Remarks</span></span>

<span data-ttu-id="3716c-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3716c-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3716c-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3716c-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3716c-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3716c-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3716c-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3716c-147">Schema name</span></span>  <br/> |<span data-ttu-id="3716c-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3716c-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="3716c-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3716c-149">Validation file</span></span>  <br/> |<span data-ttu-id="3716c-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3716c-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3716c-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3716c-151">Can be empty</span></span>  <br/> |<span data-ttu-id="3716c-152">False</span><span class="sxs-lookup"><span data-stu-id="3716c-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3716c-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3716c-153">See also</span></span>

- [<span data-ttu-id="3716c-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3716c-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="3716c-155">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="3716c-155">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="3716c-156">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="3716c-156">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="3716c-157">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="3716c-157">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

