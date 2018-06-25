---
title: Nom du paramètre (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8bcb0411-58b0-4e37-b97e-00c07dcbecb1
description: L’élément nom du paramètre représente le nom d’un paramètre dans la réponse.
ms.openlocfilehash: 9bf7c8197693bc6887a99ffcbeb2240e1f4c3b20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829468"
---
# <a name="settingname-soap"></a><span data-ttu-id="1b057-103">Nom du paramètre (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b057-103">SettingName (SOAP)</span></span>

<span data-ttu-id="1b057-104">L’élément **nom du paramètre** représente le nom d’un paramètre dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1b057-104">The **SettingName** element represents the name of a setting in the response.</span></span> 
  
```XML
<SettingName/>
```

 <span data-ttu-id="1b057-105">**string**</span><span class="sxs-lookup"><span data-stu-id="1b057-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b057-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1b057-106">Attributes and elements</span></span>

<span data-ttu-id="1b057-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1b057-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b057-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1b057-108">Attributes</span></span>

<span data-ttu-id="1b057-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b057-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b057-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1b057-110">Child elements</span></span>

<span data-ttu-id="1b057-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b057-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b057-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1b057-112">Parent elements</span></span>

|<span data-ttu-id="1b057-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1b057-113">**Element**</span></span>|<span data-ttu-id="1b057-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b057-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b057-115">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b057-115">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="1b057-116">Représente une erreur est renvoyée lors de la récupération d’un paramètre de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1b057-116">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="1b057-117">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b057-117">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="1b057-118">Représente une erreur s’est produite lors de la récupération d’un paramètre du domaine.</span><span class="sxs-lookup"><span data-stu-id="1b057-118">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="1b057-119">Cela représente une erreur à partir d’une demande **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="1b057-119">This represents an error from a **GetDomainSettings** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b057-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1b057-120">Text value</span></span>

<span data-ttu-id="1b057-121">La valeur de l’élément du **nom du paramètre** représente le nom d’un paramètre dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="1b057-121">The value of the **SettingName** element represents the name of a setting in a response.</span></span> 
  
<span data-ttu-id="1b057-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b057-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b057-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1b057-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b057-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1b057-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1b057-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1b057-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1b057-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="1b057-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1b057-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1b057-127">Validation File</span></span>  <br/> |<span data-ttu-id="1b057-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b057-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b057-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1b057-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b057-130">True</span><span class="sxs-lookup"><span data-stu-id="1b057-130">True</span></span>  <br/> |
   

