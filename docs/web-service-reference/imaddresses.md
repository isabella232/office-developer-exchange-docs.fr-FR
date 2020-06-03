---
title: Adresses
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
description: L’élément imaddresss représente une collection d’adresses de messagerie instantanée pour un contact.
ms.openlocfilehash: 24ff74d29c918d71116e25e097878b6e4e0a8ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460427"
---
# <a name="imaddresses"></a><span data-ttu-id="07fc3-103">Adresses</span><span class="sxs-lookup"><span data-stu-id="07fc3-103">ImAddresses</span></span>

<span data-ttu-id="07fc3-104">L’élément **Imaddresss** représente une collection d’adresses de messagerie instantanée pour un contact.</span><span class="sxs-lookup"><span data-stu-id="07fc3-104">The **ImAddresses** element represents a collection of instant messaging addresses for a contact.</span></span> 
  
```xml
<ImAddresses>
   <Entry/>
</ImAddresses>
```

 <span data-ttu-id="07fc3-105">**ImAddressDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="07fc3-105">**ImAddressDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07fc3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="07fc3-106">Attributes and elements</span></span>

<span data-ttu-id="07fc3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="07fc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07fc3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="07fc3-108">Attributes</span></span>

<span data-ttu-id="07fc3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="07fc3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07fc3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="07fc3-110">Child elements</span></span>

|<span data-ttu-id="07fc3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="07fc3-111">**Element**</span></span>|<span data-ttu-id="07fc3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="07fc3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07fc3-113">Entrée (IMAddress)</span><span class="sxs-lookup"><span data-stu-id="07fc3-113">Entry (IMAddress)</span></span>](entry-imaddress.md) <br/> |<span data-ttu-id="07fc3-114">Représente une adresse de messagerie instantanée pour un contact.</span><span class="sxs-lookup"><span data-stu-id="07fc3-114">Represents an instant messaging address for a contact.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07fc3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="07fc3-115">Parent elements</span></span>

|<span data-ttu-id="07fc3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="07fc3-116">**Element**</span></span>|<span data-ttu-id="07fc3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="07fc3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07fc3-118">Contact</span><span class="sxs-lookup"><span data-stu-id="07fc3-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="07fc3-119">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="07fc3-119">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07fc3-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="07fc3-120">Remarks</span></span>

<span data-ttu-id="07fc3-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="07fc3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07fc3-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="07fc3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07fc3-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="07fc3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07fc3-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="07fc3-124">Schema name</span></span>  <br/> |<span data-ttu-id="07fc3-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="07fc3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="07fc3-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="07fc3-126">Validation file</span></span>  <br/> |<span data-ttu-id="07fc3-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07fc3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07fc3-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="07fc3-128">Can be empty</span></span>  <br/> |<span data-ttu-id="07fc3-129">False</span><span class="sxs-lookup"><span data-stu-id="07fc3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07fc3-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="07fc3-130">See also</span></span>



- [<span data-ttu-id="07fc3-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07fc3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

