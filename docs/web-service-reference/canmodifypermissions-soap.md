---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: L’élément CanModifyPermissions indique si un utilisateur peut modifier les autorisations d’accès à un emplacement de partage de document.
ms.openlocfilehash: 16526cb79eeca591af6e009e67959a1c3b58a5d7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755492"
---
# <a name="canmodifypermissions-soap"></a><span data-ttu-id="bff19-103">CanModifyPermissions (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bff19-103">CanModifyPermissions (SOAP)</span></span>

<span data-ttu-id="bff19-104">L’élément **CanModifyPermissions** indique si un utilisateur peut modifier les autorisations d’accès à un emplacement de partage de document.</span><span class="sxs-lookup"><span data-stu-id="bff19-104">The **CanModifyPermissions** element indicates whether a user can modify access permissions to a document sharing location.</span></span> 
  
```XML
<CanModifyPermissions /> 
```

 <span data-ttu-id="bff19-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bff19-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bff19-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bff19-106">Attributes and elements</span></span>

<span data-ttu-id="bff19-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bff19-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bff19-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bff19-108">Attributes</span></span>

<span data-ttu-id="bff19-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bff19-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bff19-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bff19-110">Child elements</span></span>

<span data-ttu-id="bff19-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bff19-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bff19-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bff19-112">Parent elements</span></span>

|<span data-ttu-id="bff19-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bff19-113">**Element**</span></span>|<span data-ttu-id="bff19-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="bff19-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bff19-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bff19-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="bff19-116">Représente les informations d’emplacement et les métadonnées pour un emplacement de partage de document.</span><span class="sxs-lookup"><span data-stu-id="bff19-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bff19-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bff19-117">Text value</span></span>

<span data-ttu-id="bff19-118">La valeur de type Boolean de l’élément **CanModifyPermissions** indique si les utilisateurs peuvent modifier les autorisations d’accès à l’emplacement de partage.</span><span class="sxs-lookup"><span data-stu-id="bff19-118">The Boolean value of the **CanModifyPermissions** element indicates whether users can modify access permissions to the sharing location.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="bff19-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bff19-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bff19-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bff19-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bff19-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bff19-121">Schema Name</span></span>  <br/> |<span data-ttu-id="bff19-122">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="bff19-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bff19-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bff19-123">Validation File</span></span>  <br/> |<span data-ttu-id="bff19-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bff19-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bff19-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bff19-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="bff19-126">True</span><span class="sxs-lookup"><span data-stu-id="bff19-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bff19-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bff19-127">See also</span></span>



[<span data-ttu-id="bff19-128">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bff19-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="bff19-129">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="bff19-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="bff19-130">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="bff19-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

