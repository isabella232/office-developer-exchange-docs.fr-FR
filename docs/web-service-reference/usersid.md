---
title: UserSid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserSid
api_type:
- schema
ms.assetid: f8a0dcd9-8564-4e35-b307-c5d2761b48d8
description: L’élément UserSid représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité utilisateur dans un en-tête SOAP de contexte sérialisés de sécurité. Sérialisation de jeton n’est pas pris en charge.
ms.openlocfilehash: 3c72f68638f99a4ee5081517027f0834ebf65b49
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838980"
---
# <a name="usersid"></a><span data-ttu-id="491bf-104">UserSid</span><span class="sxs-lookup"><span data-stu-id="491bf-104">UserSid</span></span>

<span data-ttu-id="491bf-105">L’élément **UserSid** représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité utilisateur dans un en-tête SOAP de contexte sérialisés de sécurité.</span><span class="sxs-lookup"><span data-stu-id="491bf-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="491bf-106">Sérialisation de jeton n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="491bf-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="491bf-107">**Chaîne**</span><span class="sxs-lookup"><span data-stu-id="491bf-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="491bf-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="491bf-108">Attributes and elements</span></span>

<span data-ttu-id="491bf-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="491bf-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="491bf-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="491bf-110">Attributes</span></span>

<span data-ttu-id="491bf-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="491bf-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="491bf-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="491bf-112">Child elements</span></span>

<span data-ttu-id="491bf-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="491bf-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="491bf-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="491bf-114">Parent elements</span></span>

|<span data-ttu-id="491bf-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="491bf-115">**Element**</span></span>|<span data-ttu-id="491bf-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="491bf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="491bf-117">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="491bf-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="491bf-118">Utilisé dans l’en-tête SOAP pour sérialisation de jeton de l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="491bf-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="491bf-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="491bf-119">Text value</span></span>

<span data-ttu-id="491bf-120">La valeur de text représente l’identificateur de sécurité d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="491bf-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="491bf-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="491bf-121">Remarks</span></span>

<span data-ttu-id="491bf-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="491bf-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="491bf-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="491bf-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="491bf-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="491bf-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="491bf-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="491bf-125">Schema Name</span></span>  <br/> |<span data-ttu-id="491bf-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="491bf-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="491bf-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="491bf-127">Validation File</span></span>  <br/> |<span data-ttu-id="491bf-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="491bf-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="491bf-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="491bf-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="491bf-130">False</span><span class="sxs-lookup"><span data-stu-id="491bf-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="491bf-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="491bf-131">See also</span></span>



- [<span data-ttu-id="491bf-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="491bf-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

