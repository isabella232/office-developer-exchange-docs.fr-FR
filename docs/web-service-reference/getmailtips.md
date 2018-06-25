---
title: GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 4a24ff79-f1ae-43a1-9ac2-49baf3eaa173
description: L’élément GetMailTips représente les destinataires et les types d’astuces de la messagerie à récupérer.
ms.openlocfilehash: aad3b3d9dd578d0c92bf7d48ee8b78b58c63e23d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756669"
---
# <a name="getmailtips"></a><span data-ttu-id="07d87-103">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="07d87-103">GetMailTips</span></span>

<span data-ttu-id="07d87-104">L’élément **GetMailTips** représente les destinataires et les types d’astuces de la messagerie à récupérer.</span><span class="sxs-lookup"><span data-stu-id="07d87-104">The **GetMailTips** element represents the recipients and types of mail tips to retrieve.</span></span> 
  
```XML
<GetMailTips>
   <SendingAs/>
   <Recipients/>
   <MailTipsRequested/>
</GetMailTips>
```

 <span data-ttu-id="07d87-105">**GetMailTipsType**</span><span class="sxs-lookup"><span data-stu-id="07d87-105">**GetMailTipsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07d87-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="07d87-106">Attributes and elements</span></span>

<span data-ttu-id="07d87-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="07d87-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07d87-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="07d87-108">Attributes</span></span>

<span data-ttu-id="07d87-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="07d87-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07d87-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="07d87-110">Child elements</span></span>

|<span data-ttu-id="07d87-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="07d87-111">**Element**</span></span>|<span data-ttu-id="07d87-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="07d87-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07d87-113">SendingAs</span><span class="sxs-lookup"><span data-stu-id="07d87-113">SendingAs</span></span>](sendingas.md) <br/> |<span data-ttu-id="07d87-114">Contient une adresse de messagerie qu’un utilisateur tente d’envoyer en tant que.</span><span class="sxs-lookup"><span data-stu-id="07d87-114">Contains an e-mail address that a user is trying to send as.</span></span>  <br/> |
|[<span data-ttu-id="07d87-115">Destinataires (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="07d87-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="07d87-116">Contient une liste de destinataires pour vérifier les astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="07d87-116">Contains a list of recipients to check for mail tips.</span></span>  <br/> |
|[<span data-ttu-id="07d87-117">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="07d87-117">MailTipsRequested</span></span>](mailtipsrequested.md) <br/> |<span data-ttu-id="07d87-118">Contient les types de conseils de messagerie demandées à partir du service.</span><span class="sxs-lookup"><span data-stu-id="07d87-118">Contains the types of mail tips requested from the service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07d87-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="07d87-119">Parent elements</span></span>

<span data-ttu-id="07d87-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="07d87-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="07d87-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="07d87-121">Text value</span></span>

<span data-ttu-id="07d87-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="07d87-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="07d87-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="07d87-123">Remarks</span></span>

<span data-ttu-id="07d87-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="07d87-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07d87-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="07d87-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07d87-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="07d87-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="07d87-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="07d87-127">Schema Name</span></span>  <br/> |<span data-ttu-id="07d87-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="07d87-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="07d87-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="07d87-129">Validation File</span></span>  <br/> |<span data-ttu-id="07d87-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="07d87-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="07d87-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="07d87-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="07d87-132">False</span><span class="sxs-lookup"><span data-stu-id="07d87-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07d87-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="07d87-133">See also</span></span>



- [<span data-ttu-id="07d87-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07d87-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

