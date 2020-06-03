---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: L’élément HasIrm spécifie si au moins un message de la conversation et le dossier actif est un message protégé par IRM.
ms.openlocfilehash: 1596610ed5f6b2bac353900624fbec9140aaa693
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462779"
---
# <a name="hasirm"></a><span data-ttu-id="bbdd7-103">HasIrm</span><span class="sxs-lookup"><span data-stu-id="bbdd7-103">HasIrm</span></span>

<span data-ttu-id="bbdd7-104">L’élément **HasIrm** spécifie si au moins un message de la conversation et le dossier actif est un message protégé par IRM.</span><span class="sxs-lookup"><span data-stu-id="bbdd7-104">The **HasIrm** element specifies whether at least one message in the conversation and the current folder is an IRM protected message.</span></span> 
  
```XML
<HasIrm> true | false </HasIrm>
```

 <span data-ttu-id="bbdd7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bbdd7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bbdd7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bbdd7-106">Attributes and elements</span></span>

<span data-ttu-id="bbdd7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bbdd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbdd7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bbdd7-108">Attributes</span></span>

<span data-ttu-id="bbdd7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bbdd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bbdd7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bbdd7-110">Child elements</span></span>

<span data-ttu-id="bbdd7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bbdd7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bbdd7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bbdd7-112">Parent elements</span></span>

[<span data-ttu-id="bbdd7-113">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="bbdd7-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="bbdd7-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="bbdd7-114">Text value</span></span>

<span data-ttu-id="bbdd7-115">La valeur de texte de l’élément **HasIrm** est **true** si au moins un message de la conversation et le dossier actif a une gestion des droits relatifs à l’information (IRM).</span><span class="sxs-lookup"><span data-stu-id="bbdd7-115">The text value of the **HasIrm** element is **true** if at least one message in the conversation and the current folder has IRM.</span></span> <span data-ttu-id="bbdd7-116">Sinon, la valeur est **false**.</span><span class="sxs-lookup"><span data-stu-id="bbdd7-116">Otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bbdd7-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="bbdd7-117">Remarks</span></span>

<span data-ttu-id="bbdd7-118">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bbdd7-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="bbdd7-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bbdd7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bbdd7-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bbdd7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbdd7-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bbdd7-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bbdd7-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bbdd7-122">Schema Name</span></span>  <br/> |<span data-ttu-id="bbdd7-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bbdd7-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="bbdd7-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bbdd7-124">Validation File</span></span>  <br/> |<span data-ttu-id="bbdd7-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bbdd7-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bbdd7-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bbdd7-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbdd7-127">True</span><span class="sxs-lookup"><span data-stu-id="bbdd7-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbdd7-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bbdd7-128">See also</span></span>



[<span data-ttu-id="bbdd7-129">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="bbdd7-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="bbdd7-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bbdd7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

