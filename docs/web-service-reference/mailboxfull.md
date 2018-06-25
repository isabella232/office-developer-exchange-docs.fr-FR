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
description: L’élément MailboxFull indique si la boîte aux lettres du destinataire est pleine.
ms.openlocfilehash: 8e2c9e01b93af03e875834724a942cd9b17a73f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828286"
---
# <a name="mailboxfull"></a><span data-ttu-id="a0fd3-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="a0fd3-103">MailboxFull</span></span>

<span data-ttu-id="a0fd3-104">L’élément **MailboxFull** indique si la boîte aux lettres du destinataire est pleine.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="a0fd3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a0fd3-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a0fd3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0fd3-106">Attributes and elements</span></span>

<span data-ttu-id="a0fd3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0fd3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0fd3-108">Attributes</span></span>

<span data-ttu-id="a0fd3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0fd3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0fd3-110">Child elements</span></span>

<span data-ttu-id="a0fd3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0fd3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0fd3-112">Parent elements</span></span>

|<span data-ttu-id="a0fd3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0fd3-113">**Element**</span></span>|<span data-ttu-id="a0fd3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0fd3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0fd3-115">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="a0fd3-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="a0fd3-116">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0fd3-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a0fd3-117">Text value</span></span>

<span data-ttu-id="a0fd3-118">Cet élément peut être **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="a0fd3-119">La valeur **true** indique que la boîte aux lettres a atteint sa capacité ; la valeur **false** indique qu’il n’a pas atteint la capacité.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a0fd3-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0fd3-120">Remarks</span></span>

<span data-ttu-id="a0fd3-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0fd3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0fd3-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0fd3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0fd3-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0fd3-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0fd3-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0fd3-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a0fd3-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a0fd3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0fd3-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0fd3-126">Validation File</span></span>  <br/> |<span data-ttu-id="a0fd3-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a0fd3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0fd3-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0fd3-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0fd3-129">False</span><span class="sxs-lookup"><span data-stu-id="a0fd3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0fd3-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0fd3-130">See also</span></span>

- [<span data-ttu-id="a0fd3-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a0fd3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

