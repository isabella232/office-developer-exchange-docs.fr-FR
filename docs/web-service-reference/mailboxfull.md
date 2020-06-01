---
title: MailboxFull
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxFull
api_type:
- schema
ms.assetid: 38b28c9b-9da2-4d6a-9cda-9c393986575b
description: L’élément MailboxFull indique si la boîte aux lettres du destinataire est complète.
ms.openlocfilehash: f336f1eda122bb170aafb22a028e3faf84f4d782
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465974"
---
# <a name="mailboxfull"></a><span data-ttu-id="ae23f-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="ae23f-103">MailboxFull</span></span>

<span data-ttu-id="ae23f-104">L’élément **MailboxFull** indique si la boîte aux lettres du destinataire est complète.</span><span class="sxs-lookup"><span data-stu-id="ae23f-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="ae23f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ae23f-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ae23f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ae23f-106">Attributes and elements</span></span>

<span data-ttu-id="ae23f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ae23f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae23f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ae23f-108">Attributes</span></span>

<span data-ttu-id="ae23f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ae23f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae23f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ae23f-110">Child elements</span></span>

<span data-ttu-id="ae23f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ae23f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ae23f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ae23f-112">Parent elements</span></span>

|<span data-ttu-id="ae23f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae23f-113">**Element**</span></span>|<span data-ttu-id="ae23f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae23f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae23f-115">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="ae23f-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="ae23f-116">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="ae23f-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae23f-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ae23f-117">Text value</span></span>

<span data-ttu-id="ae23f-118">Cet élément peut avoir la **valeur true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="ae23f-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="ae23f-119">La valeur **true** indique que la boîte aux lettres a atteint sa capacité ; la valeur **false** indique qu’elle n’a pas atteint la capacité.</span><span class="sxs-lookup"><span data-stu-id="ae23f-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ae23f-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ae23f-120">Remarks</span></span>

<span data-ttu-id="ae23f-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae23f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae23f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ae23f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae23f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ae23f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae23f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ae23f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ae23f-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ae23f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae23f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ae23f-126">Validation File</span></span>  <br/> |<span data-ttu-id="ae23f-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ae23f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae23f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ae23f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae23f-129">False</span><span class="sxs-lookup"><span data-stu-id="ae23f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae23f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ae23f-130">See also</span></span>

- [<span data-ttu-id="ae23f-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ae23f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

