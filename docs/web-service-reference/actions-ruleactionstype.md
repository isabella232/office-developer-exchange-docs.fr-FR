---
title: Actions (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: L’élément actions contient une liste d’actions associées aux règles de boîte de réception.
ms.openlocfilehash: fbef3b69b1688d7c612af018d6a19f9ec1728066
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529678"
---
# <a name="actions-ruleactionstype"></a><span data-ttu-id="ba49a-103">Actions (RuleActionsType)</span><span class="sxs-lookup"><span data-stu-id="ba49a-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="ba49a-104">L’élément **actions** contient une liste d’actions associées aux règles de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ba49a-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
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

 <span data-ttu-id="ba49a-105">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="ba49a-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba49a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba49a-106">Attributes and elements</span></span>

<span data-ttu-id="ba49a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba49a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba49a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba49a-108">Attributes</span></span>

<span data-ttu-id="ba49a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ba49a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba49a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba49a-110">Child elements</span></span>

<span data-ttu-id="ba49a-111">[AssignCategories](assigncategories.md)  |  [CopyToFolder,](copytofolder.md)  |  [Supprimer](delete.md)  |  [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md)  |  [ForwardToRecipients](forwardtorecipients.md)  |  [MarkImportance](markimportance.md)  |  [MarkAsRead](markasread.md)  |  [MoveToFolder](movetofolder.md)  |  [PermanentDelete](permanentdelete.md)  |  [RedirectToRecipients](redirecttorecipients.md)  |  [SendSMSAlertToRecipients](sendsmsalerttorecipients.md)  |  [ServerReplyWithMessage](serverreplywithmessage.md)  |  [StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="ba49a-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba49a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba49a-112">Parent elements</span></span>

[<span data-ttu-id="ba49a-113">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="ba49a-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="ba49a-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba49a-114">Remarks</span></span>

<span data-ttu-id="ba49a-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ba49a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ba49a-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba49a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba49a-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba49a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba49a-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba49a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba49a-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba49a-119">Schema name</span></span>  <br/> |<span data-ttu-id="ba49a-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ba49a-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba49a-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba49a-121">Validation file</span></span>  <br/> |<span data-ttu-id="ba49a-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ba49a-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba49a-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba49a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="ba49a-124">false</span><span class="sxs-lookup"><span data-stu-id="ba49a-124">false</span></span>  <br/> |
   

