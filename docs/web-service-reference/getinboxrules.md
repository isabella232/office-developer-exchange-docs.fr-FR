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
ms.openlocfilehash: 890592fd3f87fc5592a618a2febf28e4daf0dbe4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457927"
---
# <a name="getinboxrules"></a><span data-ttu-id="f580f-103">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="f580f-103">GetInboxRules</span></span>

<span data-ttu-id="f580f-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **GetInboxRules** définit une requête pour obtenir les règles de boîte de réception sur une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="f580f-104">The **GetInboxRules** element defines a request to get the Inbox rules on a mailbox in the server store.</span></span> 
  
```XML
<GetInboxRules>
   <MailboxSmtpAddress/>
</GetInboxRules>
```

 <span data-ttu-id="f580f-105">**GetInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="f580f-105">**GetInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f580f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f580f-106">Attributes and elements</span></span>

<span data-ttu-id="f580f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f580f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f580f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f580f-108">Attributes</span></span>

<span data-ttu-id="f580f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f580f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f580f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f580f-110">Child elements</span></span>

|<span data-ttu-id="f580f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f580f-111">**Element**</span></span>|<span data-ttu-id="f580f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f580f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f580f-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="f580f-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="f580f-114">Représente l'adresse SMTP de l'utilisateur dont les règles de boîte de réception doivent être récupérés.</span><span class="sxs-lookup"><span data-stu-id="f580f-114">Represents the SMTP address of the user whose Inbox rules are to be retrieved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f580f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f580f-115">Parent elements</span></span>

<span data-ttu-id="f580f-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f580f-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f580f-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="f580f-117">Remarks</span></span>

<span data-ttu-id="f580f-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f580f-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f580f-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f580f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f580f-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f580f-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f580f-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f580f-121">Schema Name</span></span>  <br/> |<span data-ttu-id="f580f-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f580f-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f580f-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f580f-123">Validation File</span></span>  <br/> |<span data-ttu-id="f580f-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f580f-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f580f-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f580f-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="f580f-126">True</span><span class="sxs-lookup"><span data-stu-id="f580f-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f580f-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f580f-127">See also</span></span>



[<span data-ttu-id="f580f-128">Opération de GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="f580f-128">GetInboxRules operation</span></span>](getinboxrules-operation.md)

