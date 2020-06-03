---
title: ServerVersionInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerVersionInfo
api_type:
- schema
ms.assetid: c04a6872-ca27-432b-aac2-36b023d0afc6
description: L’élément ServerVersionInfo représente le numéro de version de Microsoft Exchange Server.
ms.openlocfilehash: 5bd1fbd8fdee584a9d272fa8ab82f2a31c1357fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466828"
---
# <a name="serverversioninfo"></a><span data-ttu-id="b12d1-103">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b12d1-103">ServerVersionInfo</span></span>

<span data-ttu-id="b12d1-104">L’élément **ServerVersionInfo** représente le numéro de version de Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="b12d1-104">The **ServerVersionInfo** element represents the Microsoft Exchange Server version number.</span></span> 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b12d1-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b12d1-105">Attributes and elements</span></span>

<span data-ttu-id="b12d1-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b12d1-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b12d1-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="b12d1-107">Attributes</span></span>

|<span data-ttu-id="b12d1-108">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b12d1-108">**Attribute**</span></span>|<span data-ttu-id="b12d1-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="b12d1-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b12d1-110">MajorVersion</span><span class="sxs-lookup"><span data-stu-id="b12d1-110">MajorVersion</span></span>  <br/> |<span data-ttu-id="b12d1-111">Décrit le numéro de version principale.</span><span class="sxs-lookup"><span data-stu-id="b12d1-111">Describes the major version number.</span></span>  <br/> |
|<span data-ttu-id="b12d1-112">MinorVersion</span><span class="sxs-lookup"><span data-stu-id="b12d1-112">MinorVersion</span></span>  <br/> |<span data-ttu-id="b12d1-113">Décrit le numéro de version mineure.</span><span class="sxs-lookup"><span data-stu-id="b12d1-113">Describes the minor version number.</span></span>  <br/> |
|<span data-ttu-id="b12d1-114">MajorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="b12d1-114">MajorBuildNumber</span></span>  <br/> |<span data-ttu-id="b12d1-115">Décrit le numéro de build principal.</span><span class="sxs-lookup"><span data-stu-id="b12d1-115">Describes the major build number.</span></span>  <br/> |
|<span data-ttu-id="b12d1-116">MinorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="b12d1-116">MinorBuildNumber</span></span>  <br/> |<span data-ttu-id="b12d1-117">Décrit le numéro de version mineure.</span><span class="sxs-lookup"><span data-stu-id="b12d1-117">Describes the minor build number.</span></span>  <br/> |
|<span data-ttu-id="b12d1-118">Version</span><span class="sxs-lookup"><span data-stu-id="b12d1-118">Version</span></span>  <br/> |<span data-ttu-id="b12d1-119">Décrit la version du schéma des services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="b12d1-119">Describes the Exchange Web Services (EWS) schema version.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b12d1-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b12d1-120">Child elements</span></span>

<span data-ttu-id="b12d1-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b12d1-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b12d1-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b12d1-122">Parent elements</span></span>

<span data-ttu-id="b12d1-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b12d1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b12d1-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="b12d1-124">Remarks</span></span>

<span data-ttu-id="b12d1-125">Cet élément est renvoyé dans l’en-tête SOAP d’un message de réponse des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b12d1-125">This element is returned in the SOAP header of an Exchange Web Services response message.</span></span>
  
<span data-ttu-id="b12d1-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b12d1-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b12d1-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b12d1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b12d1-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b12d1-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b12d1-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b12d1-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b12d1-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b12d1-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b12d1-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b12d1-131">Validation File</span></span>  <br/> |<span data-ttu-id="b12d1-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b12d1-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b12d1-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b12d1-133">Can Be Empty</span></span>  <br/> |<span data-ttu-id="b12d1-134">False</span><span class="sxs-lookup"><span data-stu-id="b12d1-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b12d1-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b12d1-135">See also</span></span>



- [<span data-ttu-id="b12d1-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b12d1-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

