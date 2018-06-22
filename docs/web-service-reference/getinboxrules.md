---
title: GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: 7a54992d-03a6-4afc-a2e4-dcdc9ce54194
description: L'élément GetInboxRules définit une requête pour obtenir les règles de boîte de réception sur une boîte aux lettres dans le magasin du serveur.
ms.openlocfilehash: 3c3ee682dd009e5c4bec940637a7dfa3c11f8402
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756644"
---
# <a name="getinboxrules"></a><span data-ttu-id="c0784-103">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="c0784-103">GetInboxRules</span></span>

<span data-ttu-id="c0784-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **GetInboxRules** définit une requête pour obtenir les règles de boîte de réception sur une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="c0784-104">The **GetInboxRules** element defines a request to get the Inbox rules on a mailbox in the server store.</span></span> 
  
```XML
<GetInboxRules>
   <MailboxSmtpAddress/>
</GetInboxRules>
```

 <span data-ttu-id="c0784-105">**GetInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="c0784-105">**GetInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0784-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c0784-106">Attributes and elements</span></span>

<span data-ttu-id="c0784-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c0784-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0784-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c0784-108">Attributes</span></span>

<span data-ttu-id="c0784-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c0784-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0784-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c0784-110">Child elements</span></span>

|<span data-ttu-id="c0784-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c0784-111">**Element**</span></span>|<span data-ttu-id="c0784-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c0784-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0784-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="c0784-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="c0784-114">Représente l'adresse SMTP de l'utilisateur dont les règles de boîte de réception doivent être récupérés.</span><span class="sxs-lookup"><span data-stu-id="c0784-114">Represents the SMTP address of the user whose Inbox rules are to be retrieved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0784-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c0784-115">Parent elements</span></span>

<span data-ttu-id="c0784-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c0784-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c0784-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="c0784-117">Remarks</span></span>

<span data-ttu-id="c0784-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0784-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0784-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c0784-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0784-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c0784-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c0784-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c0784-121">Schema Name</span></span>  <br/> |<span data-ttu-id="c0784-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c0784-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c0784-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c0784-123">Validation File</span></span>  <br/> |<span data-ttu-id="c0784-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c0784-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0784-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c0784-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0784-126">True</span><span class="sxs-lookup"><span data-stu-id="c0784-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0784-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c0784-127">See also</span></span>



[<span data-ttu-id="c0784-128">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="c0784-128">GetInboxRules operation</span></span>](getinboxrules-operation.md)

