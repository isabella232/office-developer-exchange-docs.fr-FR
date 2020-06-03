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
description: L’élément Entry représente une adresse de messagerie instantanée (IM) pour un contact.
ms.openlocfilehash: b6cc37447eb0f231e9e852a6c3cd64d6e1f3a89f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460700"
---
# <a name="entry-imaddress"></a><span data-ttu-id="d2461-103">Entrée (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="d2461-103">Entry (IMAddress)</span></span>

<span data-ttu-id="d2461-104">L’élément **entry** représente une adresse de messagerie instantanée (im) pour un contact.</span><span class="sxs-lookup"><span data-stu-id="d2461-104">The **Entry** element represents an instant messaging (IM) address for a contact.</span></span> 
  
```xml
<Entry Key=""/>
```

 <span data-ttu-id="d2461-105">**ImAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="d2461-105">**ImAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2461-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d2461-106">Attributes and elements</span></span>

<span data-ttu-id="d2461-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d2461-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2461-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d2461-108">Attributes</span></span>

|<span data-ttu-id="d2461-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d2461-109">**Attribute**</span></span>|<span data-ttu-id="d2461-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2461-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2461-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="d2461-111">**Key**</span></span> <br/> | <span data-ttu-id="d2461-112">Identifie l’adresse de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="d2461-112">Identifies the IM address.</span></span><br/><br/><span data-ttu-id="d2461-113">Les valeurs possibles pour cet attribut sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="d2461-113">The following are the possible values for this attribute:</span></span><br/><br/><span data-ttu-id="d2461-114">- ImAddress1</span><span class="sxs-lookup"><span data-stu-id="d2461-114">-  ImAddress1</span></span>  <br/><span data-ttu-id="d2461-115">- ImAddress2</span><span class="sxs-lookup"><span data-stu-id="d2461-115">-  ImAddress2</span></span>  <br/><span data-ttu-id="d2461-116">- ImAddress3</span><span class="sxs-lookup"><span data-stu-id="d2461-116">-  ImAddress3</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d2461-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d2461-117">Child elements</span></span>

<span data-ttu-id="d2461-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d2461-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2461-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d2461-119">Parent elements</span></span>

|<span data-ttu-id="d2461-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2461-120">**Element**</span></span>|<span data-ttu-id="d2461-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2461-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2461-122">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="d2461-122">ImAddresses</span></span>](imaddresses.md) <br/> |<span data-ttu-id="d2461-123">Représente une collection d’adresses de messagerie instantanée pour un contact.</span><span class="sxs-lookup"><span data-stu-id="d2461-123">Represents a collection of IM addresses for a contact.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2461-124">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d2461-124">Text value</span></span>

<span data-ttu-id="d2461-125">Une valeur de texte qui représente l’adresse de messagerie instantanée est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="d2461-125">A text value that represents the IM address is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2461-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="d2461-126">Remarks</span></span>

<span data-ttu-id="d2461-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d2461-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2461-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d2461-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2461-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d2461-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2461-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d2461-130">Schema name</span></span>  <br/> |<span data-ttu-id="d2461-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d2461-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2461-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d2461-132">Validation file</span></span>  <br/> |<span data-ttu-id="d2461-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2461-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2461-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d2461-134">Can be empty</span></span>  <br/> |<span data-ttu-id="d2461-135">False</span><span class="sxs-lookup"><span data-stu-id="d2461-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2461-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2461-136">See also</span></span>

- [<span data-ttu-id="d2461-137">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2461-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="d2461-138">Création de Contacts (Services Web Exchange)</span><span class="sxs-lookup"><span data-stu-id="d2461-138">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="d2461-139">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="d2461-139">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="d2461-140">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="d2461-140">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

