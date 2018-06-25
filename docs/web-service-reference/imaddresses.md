---
title: ImAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ImAddresses
api_type:
- schema
ms.assetid: 29f614a7-7fe6-47fa-b5f2-8feff106aa99
description: L’élément ImAddresses représente une collection d’adresses de messagerie instantanées pour un contact.
ms.openlocfilehash: e8c7a22e8537a4526594042905f7bb8454238bf1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827861"
---
# <a name="imaddresses"></a><span data-ttu-id="04aad-103">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="04aad-103">ImAddresses</span></span>

<span data-ttu-id="04aad-104">L’élément **ImAddresses** représente une collection d’adresses de messagerie instantanées pour un contact.</span><span class="sxs-lookup"><span data-stu-id="04aad-104">The **ImAddresses** element represents a collection of instant messaging addresses for a contact.</span></span> 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 <span data-ttu-id="04aad-105">**ImAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="04aad-105">**ImAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04aad-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04aad-106">Attributes and elements</span></span>

<span data-ttu-id="04aad-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04aad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04aad-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="04aad-108">Attributes</span></span>

<span data-ttu-id="04aad-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04aad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04aad-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04aad-110">Child elements</span></span>

|<span data-ttu-id="04aad-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04aad-111">**Element**</span></span>|<span data-ttu-id="04aad-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="04aad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04aad-113">Entrée (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="04aad-113">Entry (IMAddress)</span></span>](entry-imaddress.md) <br/> |<span data-ttu-id="04aad-114">Représente une adresse d’un contact de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="04aad-114">Represents an instant messaging address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04aad-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04aad-115">Parent elements</span></span>

|<span data-ttu-id="04aad-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04aad-116">**Element**</span></span>|<span data-ttu-id="04aad-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="04aad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04aad-118">Contact</span><span class="sxs-lookup"><span data-stu-id="04aad-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="04aad-119">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="04aad-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04aad-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="04aad-120">Remarks</span></span>

<span data-ttu-id="04aad-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="04aad-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04aad-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04aad-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04aad-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04aad-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04aad-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04aad-124">Schema name</span></span>  <br/> |<span data-ttu-id="04aad-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="04aad-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="04aad-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04aad-126">Validation file</span></span>  <br/> |<span data-ttu-id="04aad-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04aad-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04aad-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04aad-128">Can be empty</span></span>  <br/> |<span data-ttu-id="04aad-129">False</span><span class="sxs-lookup"><span data-stu-id="04aad-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04aad-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04aad-130">See also</span></span>



- [<span data-ttu-id="04aad-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="04aad-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

