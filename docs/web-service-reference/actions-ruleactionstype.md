---
title: Actions (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: L’élément Actions contient une liste d’actions associées aux règles de boîte de réception.
ms.openlocfilehash: 8ed8095ca8b41e037c2c0dad319c9c4ab99ed2bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755245"
---
# <a name="actions-ruleactionstype"></a><span data-ttu-id="635ce-103">Actions (RuleActionsType)</span><span class="sxs-lookup"><span data-stu-id="635ce-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="635ce-104">L’élément **Actions** contient une liste d’actions associées aux règles de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="635ce-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
```XML
<Actions>
   <AssignCategories/>
   <CopyToFolder/>
   <Delete/>
   <ForwardAsAttachmentToRecipients/>
   <ForwardToRecipients/>
   <MarkImportance/>
   <MarkAsRead/>
   <MoveToFolder/>
   <PermanentDelete/>
   <RedirectToRecipients/>
   <SendSMSAlertToRecipients/>
   <ServerReplyWithMessage/>
   <StopProcessingRules/>
</Actions>
```

 <span data-ttu-id="635ce-105">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="635ce-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="635ce-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="635ce-106">Attributes and elements</span></span>

<span data-ttu-id="635ce-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="635ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="635ce-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="635ce-108">Attributes</span></span>

<span data-ttu-id="635ce-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="635ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="635ce-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="635ce-110">Child elements</span></span>

<span data-ttu-id="635ce-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Supprimer](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead ](markasread.md)  |  [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md)  |  [ StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="635ce-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="635ce-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="635ce-112">Parent elements</span></span>

[<span data-ttu-id="635ce-113">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="635ce-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="635ce-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="635ce-114">Remarks</span></span>

<span data-ttu-id="635ce-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="635ce-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="635ce-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="635ce-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="635ce-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="635ce-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="635ce-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="635ce-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="635ce-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="635ce-119">Schema name</span></span>  <br/> |<span data-ttu-id="635ce-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="635ce-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="635ce-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="635ce-121">Validation file</span></span>  <br/> |<span data-ttu-id="635ce-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="635ce-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="635ce-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="635ce-123">Can be empty</span></span>  <br/> |<span data-ttu-id="635ce-124">false</span><span class="sxs-lookup"><span data-stu-id="635ce-124">false</span></span>  <br/> |
   

