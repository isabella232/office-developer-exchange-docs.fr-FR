---
title: ReplyBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: L’élément ReplyBody contient un message d’absence du bureau et la langue utilisée pour le message.
ms.openlocfilehash: 496d336d1f87d9ea493ba7da362eef5a416fd899
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465302"
---
# <a name="replybody"></a><span data-ttu-id="eaf31-103">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="eaf31-103">ReplyBody</span></span>

<span data-ttu-id="eaf31-104">L’élément **ReplyBody** contient un message d’absence du bureau et la langue utilisée pour le message.</span><span class="sxs-lookup"><span data-stu-id="eaf31-104">The **ReplyBody** element contains an Out of Office (OOF) message and the language used for the message.</span></span> 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 <span data-ttu-id="eaf31-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="eaf31-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eaf31-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eaf31-106">Attributes and elements</span></span>

<span data-ttu-id="eaf31-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eaf31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eaf31-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="eaf31-108">Attributes</span></span>

|<span data-ttu-id="eaf31-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="eaf31-109">**Attribute**</span></span>|<span data-ttu-id="eaf31-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="eaf31-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eaf31-111">XML : lang</span><span class="sxs-lookup"><span data-stu-id="eaf31-111">xml:lang</span></span>  <br/> |<span data-ttu-id="eaf31-112">Spécifie la langue utilisée dans le contenu **ReplyBody** .</span><span class="sxs-lookup"><span data-stu-id="eaf31-112">Specifies the language used in the **ReplyBody** contents.</span></span> <span data-ttu-id="eaf31-113">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="eaf31-113">This attribute is optional.</span></span> <span data-ttu-id="eaf31-114">Les valeurs possibles de cet attribut sont définies par IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="eaf31-114">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="eaf31-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eaf31-115">Child elements</span></span>

|<span data-ttu-id="eaf31-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eaf31-116">**Element**</span></span>|<span data-ttu-id="eaf31-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="eaf31-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eaf31-118">Message (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="eaf31-118">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="eaf31-119">Contient la réponse absent (e) du bureau.</span><span class="sxs-lookup"><span data-stu-id="eaf31-119">Contains the out of office (OOF) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eaf31-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eaf31-120">Parent elements</span></span>

|<span data-ttu-id="eaf31-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eaf31-121">**Element**</span></span>|<span data-ttu-id="eaf31-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="eaf31-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eaf31-123">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="eaf31-123">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="eaf31-124">Définit le message de réponse OOF et une durée d’envoi du message de réponse pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="eaf31-124">Defines the OOF response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eaf31-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="eaf31-125">Text value</span></span>

<span data-ttu-id="eaf31-126">Aucun.</span><span class="sxs-lookup"><span data-stu-id="eaf31-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eaf31-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="eaf31-127">Remarks</span></span>

<span data-ttu-id="eaf31-128">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="eaf31-128">This element is required.</span></span>
  
<span data-ttu-id="eaf31-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="eaf31-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eaf31-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eaf31-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eaf31-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eaf31-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eaf31-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eaf31-132">Schema Name</span></span>  <br/> |<span data-ttu-id="eaf31-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="eaf31-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="eaf31-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eaf31-134">Validation File</span></span>  <br/> |<span data-ttu-id="eaf31-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eaf31-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eaf31-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eaf31-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="eaf31-137">False</span><span class="sxs-lookup"><span data-stu-id="eaf31-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eaf31-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eaf31-138">See also</span></span>



- [<span data-ttu-id="eaf31-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="eaf31-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

