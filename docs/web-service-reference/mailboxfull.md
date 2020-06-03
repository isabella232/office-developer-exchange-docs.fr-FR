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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465974"
---
# <a name="mailboxfull"></a><span data-ttu-id="461c8-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="461c8-103">MailboxFull</span></span>

<span data-ttu-id="461c8-104">L’élément **MailboxFull** indique si la boîte aux lettres du destinataire est complète.</span><span class="sxs-lookup"><span data-stu-id="461c8-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="461c8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="461c8-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="461c8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="461c8-106">Attributes and elements</span></span>

<span data-ttu-id="461c8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="461c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="461c8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="461c8-108">Attributes</span></span>

<span data-ttu-id="461c8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="461c8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="461c8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="461c8-110">Child elements</span></span>

<span data-ttu-id="461c8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="461c8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="461c8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="461c8-112">Parent elements</span></span>

|<span data-ttu-id="461c8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="461c8-113">**Element**</span></span>|<span data-ttu-id="461c8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="461c8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="461c8-115">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="461c8-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="461c8-116">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="461c8-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="461c8-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="461c8-117">Text value</span></span>

<span data-ttu-id="461c8-118">Cet élément peut avoir la **valeur true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="461c8-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="461c8-119">La valeur **true** indique que la boîte aux lettres a atteint sa capacité ; la valeur **false** indique qu’elle n’a pas atteint la capacité.</span><span class="sxs-lookup"><span data-stu-id="461c8-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="461c8-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="461c8-120">Remarks</span></span>

<span data-ttu-id="461c8-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="461c8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="461c8-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="461c8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="461c8-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="461c8-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="461c8-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="461c8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="461c8-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="461c8-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="461c8-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="461c8-126">Validation File</span></span>  <br/> |<span data-ttu-id="461c8-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="461c8-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="461c8-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="461c8-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="461c8-129">False</span><span class="sxs-lookup"><span data-stu-id="461c8-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="461c8-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="461c8-130">See also</span></span>

- [<span data-ttu-id="461c8-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="461c8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

