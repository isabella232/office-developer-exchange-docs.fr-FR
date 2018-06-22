---
title: Entrée (IMAddress)
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
ms.assetid: ee444170-7353-4e86-86c6-d7300a2f1777
description: L’élément d’entrée représente une adresse (MI) d’un contact de messagerie instantanée.
ms.openlocfilehash: 77de059cef470dde90ab0b929845cb260b4b867c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756209"
---
# <a name="entry-imaddress"></a><span data-ttu-id="2ac67-103">Entrée (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="2ac67-103">Entry (IMAddress)</span></span>

<span data-ttu-id="2ac67-104">L’élément **d’entrée** représente une adresse (MI) d’un contact de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="2ac67-104">The **Entry** element represents an instant messaging (IM) address for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="2ac67-105">**ImAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="2ac67-105">**ImAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ac67-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ac67-106">Attributes and elements</span></span>

<span data-ttu-id="2ac67-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ac67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ac67-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ac67-108">Attributes</span></span>

|<span data-ttu-id="2ac67-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="2ac67-109">**Attribute**</span></span>|<span data-ttu-id="2ac67-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ac67-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2ac67-111">**Clé**</span><span class="sxs-lookup"><span data-stu-id="2ac67-111">**Key**</span></span> <br/> | <span data-ttu-id="2ac67-112">Identifie l’adresse de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="2ac67-112">Identifies the IM address.</span></span><br/><br/><span data-ttu-id="2ac67-113">Les valeurs possibles de cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="2ac67-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="2ac67-114">-ImAddress1</span><span class="sxs-lookup"><span data-stu-id="2ac67-114">-  ImAddress1</span></span>  <br/><span data-ttu-id="2ac67-115">-ImAddress2</span><span class="sxs-lookup"><span data-stu-id="2ac67-115">-  ImAddress2</span></span>  <br/><span data-ttu-id="2ac67-116">-ImAddress3</span><span class="sxs-lookup"><span data-stu-id="2ac67-116">-  ImAddress3</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2ac67-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ac67-117">Child elements</span></span>

<span data-ttu-id="2ac67-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2ac67-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ac67-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ac67-119">Parent elements</span></span>

|<span data-ttu-id="2ac67-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2ac67-120">**Element**</span></span>|<span data-ttu-id="2ac67-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="2ac67-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ac67-122">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="2ac67-122">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="2ac67-123">Représente une collection d’adresses de messagerie instantanée d’un contact.</span><span class="sxs-lookup"><span data-stu-id="2ac67-123">Represents a collection of IM addresses for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ac67-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2ac67-124">Text value</span></span>

<span data-ttu-id="2ac67-125">Une valeur de texte qui représente l’adresse de messagerie instantanée est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="2ac67-125">A text value that represents the IM address is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2ac67-126">Note</span><span class="sxs-lookup"><span data-stu-id="2ac67-126">Remarks</span></span>

<span data-ttu-id="2ac67-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2ac67-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ac67-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ac67-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ac67-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ac67-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ac67-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ac67-130">Schema name</span></span>  <br/> |<span data-ttu-id="2ac67-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2ac67-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ac67-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ac67-132">Validation file</span></span>  <br/> |<span data-ttu-id="2ac67-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ac67-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ac67-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ac67-134">Can be empty</span></span>  <br/> |<span data-ttu-id="2ac67-135">False</span><span class="sxs-lookup"><span data-stu-id="2ac67-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ac67-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ac67-136">See also</span></span>

- [<span data-ttu-id="2ac67-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2ac67-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="2ac67-138">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="2ac67-138">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="2ac67-139">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="2ac67-139">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="2ac67-140">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="2ac67-140">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

