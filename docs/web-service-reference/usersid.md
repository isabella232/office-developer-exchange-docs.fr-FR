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
description: L’élément UserSid représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité de l’utilisateur dans un en-tête SOAP de contexte de sécurité sérialisé. La sérialisation de jetons n’est pas prise en charge.
ms.openlocfilehash: b8ee51b1998546fc4ab14bd3666192ae63c8dba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462016"
---
# <a name="usersid"></a><span data-ttu-id="78e9e-104">UserSid</span><span class="sxs-lookup"><span data-stu-id="78e9e-104">UserSid</span></span>

<span data-ttu-id="78e9e-105">L’élément **UserSid** représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité de l’utilisateur dans un en-tête SOAP de contexte de sécurité sérialisé.</span><span class="sxs-lookup"><span data-stu-id="78e9e-105">The **UserSid** element represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span> <span data-ttu-id="78e9e-106">La sérialisation de jetons n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="78e9e-106">Token serialization is not supported.</span></span> 
  
```xml
<UserSid/>
```

 <span data-ttu-id="78e9e-107">**String**</span><span class="sxs-lookup"><span data-stu-id="78e9e-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78e9e-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="78e9e-108">Attributes and elements</span></span>

<span data-ttu-id="78e9e-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="78e9e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78e9e-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="78e9e-110">Attributes</span></span>

<span data-ttu-id="78e9e-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="78e9e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78e9e-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="78e9e-112">Child elements</span></span>

<span data-ttu-id="78e9e-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="78e9e-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78e9e-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="78e9e-114">Parent elements</span></span>

|<span data-ttu-id="78e9e-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78e9e-115">**Element**</span></span>|<span data-ttu-id="78e9e-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="78e9e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78e9e-117">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="78e9e-117">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="78e9e-118">Utilisé dans l’en-tête SOAP pour la sérialisation de jetons dans l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="78e9e-118">Used in the SOAP header for token serialization in server-to-server authentication.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78e9e-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="78e9e-119">Text value</span></span>

<span data-ttu-id="78e9e-120">La valeur texte représente l’identificateur de sécurité d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="78e9e-120">The text value represents a user's security identifier.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="78e9e-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="78e9e-121">Remarks</span></span>

<span data-ttu-id="78e9e-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="78e9e-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78e9e-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="78e9e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78e9e-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="78e9e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78e9e-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="78e9e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="78e9e-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="78e9e-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="78e9e-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="78e9e-127">Validation File</span></span>  <br/> |<span data-ttu-id="78e9e-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78e9e-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78e9e-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="78e9e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="78e9e-130">False</span><span class="sxs-lookup"><span data-stu-id="78e9e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78e9e-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="78e9e-131">See also</span></span>



- [<span data-ttu-id="78e9e-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="78e9e-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

