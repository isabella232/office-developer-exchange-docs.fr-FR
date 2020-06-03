---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: L’élément SerializedSecurityContext est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour la sérialisation de jetons dans l’authentification de serveur à serveur. La sérialisation de jetons n’est pas prise en charge.
ms.openlocfilehash: 58fea1c7f613315d59e81935561f92f318afc769
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462051"
---
# <a name="serializedsecuritycontext"></a><span data-ttu-id="fcd10-104">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="fcd10-104">SerializedSecurityContext</span></span>

<span data-ttu-id="fcd10-105">L’élément **SerializedSecurityContext** est utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour la sérialisation de jetons dans l’authentification de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="fcd10-105">The **SerializedSecurityContext** element is used in the Simple Object Access Protocol (SOAP) header for token serialization in server-to-server authentication.</span></span> <span data-ttu-id="fcd10-106">La sérialisation de jetons n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="fcd10-106">Token serialization is not supported.</span></span> 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 <span data-ttu-id="fcd10-107">**SerializedSecurityContextType**</span><span class="sxs-lookup"><span data-stu-id="fcd10-107">**SerializedSecurityContextType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fcd10-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fcd10-108">Attributes and elements</span></span>

<span data-ttu-id="fcd10-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fcd10-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fcd10-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="fcd10-110">Attributes</span></span>

<span data-ttu-id="fcd10-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fcd10-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fcd10-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fcd10-112">Child elements</span></span>

|<span data-ttu-id="fcd10-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fcd10-113">**Element**</span></span>|<span data-ttu-id="fcd10-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fcd10-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fcd10-115">UserSid</span><span class="sxs-lookup"><span data-stu-id="fcd10-115">UserSid</span></span>](usersid.md) <br/> |<span data-ttu-id="fcd10-116">Représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité de l’utilisateur dans un en-tête SOAP de contexte de sécurité sérialisé.</span><span class="sxs-lookup"><span data-stu-id="fcd10-116">Represents the security descriptor definition language (SDDL) form of the user security identifier in a serialized security context SOAP header.</span></span>  <br/> |
|[<span data-ttu-id="fcd10-117">GroupSids</span><span class="sxs-lookup"><span data-stu-id="fcd10-117">GroupSids</span></span>](groupsids.md) <br/> |<span data-ttu-id="fcd10-118">Représente une collection d’identificateurs de sécurité d’objet de groupe de service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fcd10-118">Represents a collection of Active Directory directory service group object security identifiers.</span></span>  <br/> |
|[<span data-ttu-id="fcd10-119">RestrictedGroupSids</span><span class="sxs-lookup"><span data-stu-id="fcd10-119">RestrictedGroupSids</span></span>](restrictedgroupsids.md) <br/> |<span data-ttu-id="fcd10-120">Représente l’identificateur de sécurité de groupe et les attributs d’un groupe restreint.</span><span class="sxs-lookup"><span data-stu-id="fcd10-120">Represents the group security identifier and attributes for a restricted group.</span></span>  <br/> |
|[<span data-ttu-id="fcd10-121">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="fcd10-121">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="fcd10-122">Représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’autorisation de serveur à serveur.</span><span class="sxs-lookup"><span data-stu-id="fcd10-122">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fcd10-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fcd10-123">Parent elements</span></span>

<span data-ttu-id="fcd10-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fcd10-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fcd10-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="fcd10-125">Remarks</span></span>

<span data-ttu-id="fcd10-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client (CAS) est installé.</span><span class="sxs-lookup"><span data-stu-id="fcd10-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server (CAS) role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fcd10-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fcd10-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fcd10-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fcd10-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fcd10-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fcd10-129">Schema Name</span></span>  <br/> |<span data-ttu-id="fcd10-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fcd10-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="fcd10-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fcd10-131">Validation File</span></span>  <br/> |<span data-ttu-id="fcd10-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fcd10-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fcd10-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fcd10-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="fcd10-134">False</span><span class="sxs-lookup"><span data-stu-id="fcd10-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fcd10-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fcd10-135">See also</span></span>



- [<span data-ttu-id="fcd10-136">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fcd10-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fcd10-137">Autorisation de serveur à serveur dans EWS</span><span class="sxs-lookup"><span data-stu-id="fcd10-137">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

