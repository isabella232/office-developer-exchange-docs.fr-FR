---
title: Boîte aux lettres (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: L’élément de boîte aux lettres contient l’identificateur de la boîte aux lettres et l’adresse SMTP Simple Mail Transfer Protocol () principale de l’utilisateur.
ms.openlocfilehash: 1b6669928015bc880806479d294a4063034a559f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828255"
---
# <a name="mailbox-previewitemmailboxtype"></a><span data-ttu-id="d1eb7-103">Boîte aux lettres (PreviewItemMailboxType)</span><span class="sxs-lookup"><span data-stu-id="d1eb7-103">Mailbox (PreviewItemMailboxType)</span></span>

<span data-ttu-id="d1eb7-104">L’élément de **boîte aux lettres** contient l’identificateur de la boîte aux lettres et l’adresse SMTP Simple Mail Transfer Protocol () principale de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1eb7-104">The **Mailbox** element contains the mailbox identifier and the user's primary Simple Mail Transfer Protocol (SMTP) address.</span></span> 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

<span data-ttu-id="d1eb7-105">**PreviewItemMailboxType**</span><span class="sxs-lookup"><span data-stu-id="d1eb7-105">**PreviewItemMailboxType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d1eb7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d1eb7-106">Attributes and elements</span></span>

<span data-ttu-id="d1eb7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d1eb7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1eb7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d1eb7-108">Attributes</span></span>

<span data-ttu-id="d1eb7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d1eb7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1eb7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d1eb7-110">Child elements</span></span>

<span data-ttu-id="d1eb7-111">[MailboxId](mailboxid.md) | [PrimarySmtpAddress (chaîne)](primarysmtpaddress-string.md)</span><span class="sxs-lookup"><span data-stu-id="d1eb7-111">[MailboxId](mailboxid.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1eb7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d1eb7-112">Parent elements</span></span>

[<span data-ttu-id="d1eb7-113">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="d1eb7-113">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="d1eb7-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="d1eb7-114">Remarks</span></span>

<span data-ttu-id="d1eb7-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d1eb7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d1eb7-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1eb7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1eb7-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d1eb7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1eb7-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d1eb7-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1eb7-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d1eb7-119">Schema name</span></span>  <br/> |<span data-ttu-id="d1eb7-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d1eb7-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1eb7-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d1eb7-121">Validation file</span></span>  <br/> |<span data-ttu-id="d1eb7-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d1eb7-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1eb7-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d1eb7-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d1eb7-124">false</span><span class="sxs-lookup"><span data-stu-id="d1eb7-124">false</span></span>  <br/> |
   

