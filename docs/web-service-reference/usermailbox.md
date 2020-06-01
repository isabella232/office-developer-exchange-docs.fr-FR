---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: L’élément UserMailbox identifie une boîte aux lettres utilisateur.
ms.openlocfilehash: 9bb1b08320f5e6f4843383a8e3aff96fc3dcccad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465316"
---
# <a name="usermailbox"></a><span data-ttu-id="25cfc-103">UserMailbox</span><span class="sxs-lookup"><span data-stu-id="25cfc-103">UserMailbox</span></span>

<span data-ttu-id="25cfc-104">L’élément **UserMailbox** identifie une boîte aux lettres utilisateur.</span><span class="sxs-lookup"><span data-stu-id="25cfc-104">The **UserMailbox** element identifies a user mailbox.</span></span> 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 <span data-ttu-id="25cfc-105">**UserMailboxType**</span><span class="sxs-lookup"><span data-stu-id="25cfc-105">**UserMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25cfc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="25cfc-106">Attributes and elements</span></span>

<span data-ttu-id="25cfc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="25cfc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25cfc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="25cfc-108">Attributes</span></span>

|<span data-ttu-id="25cfc-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="25cfc-109">**Attribute**</span></span>|<span data-ttu-id="25cfc-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="25cfc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25cfc-111">ID</span><span class="sxs-lookup"><span data-stu-id="25cfc-111">Id</span></span>  <br/> |<span data-ttu-id="25cfc-112">La valeur de texte de l’attribut **ID** est l’identificateur de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25cfc-112">The text value of the **Id** attribute is the identifier of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="25cfc-113">IsArchive</span><span class="sxs-lookup"><span data-stu-id="25cfc-113">IsArchive</span></span>  <br/> |<span data-ttu-id="25cfc-114">La valeur de texte de l’attribut **IsArchive** indique si la boîte aux lettres est une boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="25cfc-114">The text value of the **IsArchive** attribute indicates whether the mailbox is an archive mailbox.</span></span> <span data-ttu-id="25cfc-115">Une valeur de texte de **true** pour l’attribut **IsArchive** indique que la boîte aux lettres est une boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="25cfc-115">A text value of **true** for the **IsArchive** attribute indicates that the mailbox is an archive mailbox.</span></span> <span data-ttu-id="25cfc-116">La valeur **false** pour l’attribut **IsArchive** indique que la boîte aux lettres est une boîte aux lettres principale.</span><span class="sxs-lookup"><span data-stu-id="25cfc-116">A value of **false** for the **IsArchive** attribute indicates that the mailbox is a primary mailbox.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="25cfc-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="25cfc-117">Child elements</span></span>

<span data-ttu-id="25cfc-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="25cfc-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25cfc-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="25cfc-119">Parent elements</span></span>

<span data-ttu-id="25cfc-120">[Boîtes aux lettres (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md)  |  [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="25cfc-120">[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="25cfc-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="25cfc-121">Remarks</span></span>

<span data-ttu-id="25cfc-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="25cfc-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="25cfc-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="25cfc-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25cfc-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="25cfc-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25cfc-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="25cfc-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25cfc-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="25cfc-126">Schema name</span></span>  <br/> |<span data-ttu-id="25cfc-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="25cfc-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="25cfc-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="25cfc-128">Validation file</span></span>  <br/> |<span data-ttu-id="25cfc-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25cfc-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25cfc-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="25cfc-130">Can be empty</span></span>  <br/> |<span data-ttu-id="25cfc-131">true</span><span class="sxs-lookup"><span data-stu-id="25cfc-131">true</span></span>  <br/> |
   

