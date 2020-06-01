---
title: Contenu
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Content
api_type:
- schema
ms.assetid: 24f8c54a-505f-4fc0-b7e7-93ad50b97070
description: L’élément content contient le contenu encodé en base64 d’une pièce jointe.
ms.openlocfilehash: 81f6acf69ff702bd0645663cb2e499ee5b45ea78
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458949"
---
# <a name="content"></a><span data-ttu-id="04e08-103">Contenu</span><span class="sxs-lookup"><span data-stu-id="04e08-103">Content</span></span>

<span data-ttu-id="04e08-104">L’élément **content** contient le contenu encodé en base64 d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="04e08-104">The **Content** element contains the Base64-encoded contents of a file attachment.</span></span> 
  
```xml
<Content/>
```

 <span data-ttu-id="04e08-105">**Au base64Binary**</span><span class="sxs-lookup"><span data-stu-id="04e08-105">**Base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04e08-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04e08-106">Attributes and elements</span></span>

<span data-ttu-id="04e08-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04e08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04e08-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="04e08-108">Attributes</span></span>

<span data-ttu-id="04e08-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="04e08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04e08-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04e08-110">Child elements</span></span>

<span data-ttu-id="04e08-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04e08-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04e08-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04e08-112">Parent elements</span></span>

|<span data-ttu-id="04e08-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04e08-113">**Element**</span></span>|<span data-ttu-id="04e08-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="04e08-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04e08-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="04e08-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="04e08-116">Représente un fichier t thattached à un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="04e08-116">Represents a file t is thattached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04e08-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="04e08-117">Text value</span></span>

<span data-ttu-id="04e08-118">La valeur de chaîne représente les données binaires codées en base64 de la pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="04e08-118">The string value represents the Base64-encoded binary data of the file attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04e08-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="04e08-119">Remarks</span></span>

<span data-ttu-id="04e08-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="04e08-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04e08-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04e08-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04e08-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04e08-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04e08-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04e08-123">Schema name</span></span>  <br/> |<span data-ttu-id="04e08-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="04e08-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="04e08-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04e08-125">Validation file</span></span>  <br/> |<span data-ttu-id="04e08-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04e08-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04e08-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04e08-127">Can be empty</span></span>  <br/> |<span data-ttu-id="04e08-128">False</span><span class="sxs-lookup"><span data-stu-id="04e08-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04e08-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04e08-129">See also</span></span>



- [<span data-ttu-id="04e08-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="04e08-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

