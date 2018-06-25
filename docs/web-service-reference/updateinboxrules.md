---
title: UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: d220064f-ff4d-4537-8077-adf94f2cbdbd
description: L'élément UpdateInboxRules définit une demande pour mettre à jour les règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.
ms.openlocfilehash: 73af3efcbf4320604576b724acf18530b8b86b26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838878"
---
# <a name="updateinboxrules"></a><span data-ttu-id="a5c0d-103">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="a5c0d-103">UpdateInboxRules</span></span>

<span data-ttu-id="a5c0d-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **UpdateInboxRules** définit une demande pour mettre à jour les règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-104">The **UpdateInboxRules** element defines a request to update the Inbox rules in a mailbox in the server store.</span></span> 
  
```XML
<UpdateInboxRules>
   <MailboxSmtpAddress/>
   <RemoveOutlookRuleBlob/>
   <Operations/>
</UpdateInboxRules>
```

 <span data-ttu-id="a5c0d-105">**UpdateInboxRulesRequestType**</span><span class="sxs-lookup"><span data-stu-id="a5c0d-105">**UpdateInboxRulesRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5c0d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a5c0d-106">Attributes and elements</span></span>

<span data-ttu-id="a5c0d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5c0d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a5c0d-108">Attributes</span></span>

<span data-ttu-id="a5c0d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5c0d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a5c0d-110">Child elements</span></span>

|<span data-ttu-id="a5c0d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a5c0d-111">**Element**</span></span>|<span data-ttu-id="a5c0d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a5c0d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5c0d-113">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a5c0d-113">MailboxSmtpAddress</span></span>](mailboxsmtpaddress.md) <br/> |<span data-ttu-id="a5c0d-114">Représente l'adresse SMTP de l'utilisateur dont les règles de boîte de réception doivent être créés, modifié ou supprimé.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-114">Represents the SMTP address of the user whose Inbox rules are to be created, modified, or deleted.</span></span>  <br/> |
|[<span data-ttu-id="a5c0d-115">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="a5c0d-115">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md) <br/> |<span data-ttu-id="a5c0d-116">Indique s'il faut supprimer le blob de règle de Microsoft Outlook.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-116">Indicates whether to remove the Microsoft Outlook rule blob.</span></span>  <br/> |
|[<span data-ttu-id="a5c0d-117">Opérations</span><span class="sxs-lookup"><span data-stu-id="a5c0d-117">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="a5c0d-118">Contient un tableau des opérations de règle qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-118">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5c0d-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a5c0d-119">Parent elements</span></span>

<span data-ttu-id="a5c0d-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a5c0d-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a5c0d-121">Text value</span></span>

<span data-ttu-id="a5c0d-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a5c0d-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="a5c0d-123">Remarks</span></span>

<span data-ttu-id="a5c0d-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5c0d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5c0d-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a5c0d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5c0d-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a5c0d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a5c0d-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a5c0d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a5c0d-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a5c0d-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a5c0d-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a5c0d-129">Validation File</span></span>  <br/> |<span data-ttu-id="a5c0d-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a5c0d-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a5c0d-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a5c0d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5c0d-132">True</span><span class="sxs-lookup"><span data-stu-id="a5c0d-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5c0d-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a5c0d-133">See also</span></span>



[<span data-ttu-id="a5c0d-134">Opération de UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="a5c0d-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="a5c0d-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a5c0d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

