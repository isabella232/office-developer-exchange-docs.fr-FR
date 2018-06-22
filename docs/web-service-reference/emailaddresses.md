---
title: EmailAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EmailAddresses
api_type:
- schema
ms.assetid: fd4d773c-f7dc-4a04-9025-e772d7a45fdf
description: L’élément EmailAddresses représente une collection d’adresses de messagerie d’un contact.
ms.openlocfilehash: 2eddb68ecffd8f61a2fbb775d8013433d715db1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756119"
---
# <a name="emailaddresses"></a><span data-ttu-id="3cc0b-103">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="3cc0b-103">EmailAddresses</span></span>

<span data-ttu-id="3cc0b-104">L’élément **EmailAddresses** représente une collection d’adresses de messagerie d’un contact.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-104">The **EmailAddresses** element represents a collection of e-mail addresses for a contact.</span></span> 
  
```xml
<EmailAddresses>
   <Entry/>
</EmailAddresses>
```

 <span data-ttu-id="3cc0b-105">**EmailAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="3cc0b-105">**EmailAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cc0b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3cc0b-106">Attributes and elements</span></span>

<span data-ttu-id="3cc0b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cc0b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3cc0b-108">Attributes</span></span>

<span data-ttu-id="3cc0b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3cc0b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3cc0b-110">Child elements</span></span>

|<span data-ttu-id="3cc0b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3cc0b-111">**Element**</span></span>|<span data-ttu-id="3cc0b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3cc0b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cc0b-113">Entrée (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3cc0b-113">Entry (EmailAddress)</span></span>](entry-emailaddress.md) <br/> |<span data-ttu-id="3cc0b-114">Représente une adresse de messagerie unique pour un contact.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-114">Represents a single e-mail address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3cc0b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3cc0b-115">Parent elements</span></span>

|<span data-ttu-id="3cc0b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3cc0b-116">**Element**</span></span>|<span data-ttu-id="3cc0b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3cc0b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cc0b-118">Contact</span><span class="sxs-lookup"><span data-stu-id="3cc0b-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3cc0b-119">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3cc0b-120">Note</span><span class="sxs-lookup"><span data-stu-id="3cc0b-120">Remarks</span></span>

<span data-ttu-id="3cc0b-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3cc0b-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3cc0b-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3cc0b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cc0b-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3cc0b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3cc0b-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3cc0b-124">Schema name</span></span>  <br/> |<span data-ttu-id="3cc0b-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3cc0b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="3cc0b-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3cc0b-126">Validation file</span></span>  <br/> |<span data-ttu-id="3cc0b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3cc0b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3cc0b-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3cc0b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="3cc0b-129">False</span><span class="sxs-lookup"><span data-stu-id="3cc0b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3cc0b-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3cc0b-130">See also</span></span>

- [<span data-ttu-id="3cc0b-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3cc0b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="3cc0b-132">Creating Contacts (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="3cc0b-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [<span data-ttu-id="3cc0b-133">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="3cc0b-133">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx) 
- [<span data-ttu-id="3cc0b-134">Deleting Contacts</span><span class="sxs-lookup"><span data-stu-id="3cc0b-134">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

