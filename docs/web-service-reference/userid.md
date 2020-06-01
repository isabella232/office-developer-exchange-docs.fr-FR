---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: L’élément UserId identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.
ms.openlocfilehash: 68075e335383835ddce9575d85ba5fa945ed305c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455540"
---
# <a name="userid"></a><span data-ttu-id="0fc3d-103">UserId</span><span class="sxs-lookup"><span data-stu-id="0fc3d-103">UserId</span></span>

<span data-ttu-id="0fc3d-104">L’élément **userid** identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="0fc3d-105">**UserIdType**</span><span class="sxs-lookup"><span data-stu-id="0fc3d-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0fc3d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0fc3d-106">Attributes and elements</span></span>

<span data-ttu-id="0fc3d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fc3d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0fc3d-108">Attributes</span></span>

<span data-ttu-id="0fc3d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0fc3d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0fc3d-110">Child elements</span></span>

|<span data-ttu-id="0fc3d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fc3d-111">**Element**</span></span>|<span data-ttu-id="0fc3d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fc3d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fc3d-113">SID</span><span class="sxs-lookup"><span data-stu-id="0fc3d-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="0fc3d-114">Représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité (SID).</span><span class="sxs-lookup"><span data-stu-id="0fc3d-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="0fc3d-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="0fc3d-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="0fc3d-116">Représente l’adresse SMTP (Simple Mail Transfer Protocol) principale d’un compte à utiliser pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="0fc3d-117">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="0fc3d-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="0fc3d-118">Définit le nom d’affichage d’un dossier, d’un contact, d’une liste de distribution ou d’un utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="0fc3d-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="0fc3d-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="0fc3d-120">Identifie les comptes d’utilisateur anonymes et par défaut pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="0fc3d-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="0fc3d-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="0fc3d-122">Identifie un utilisateur délégué externe ou un utilisateur externe qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fc3d-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0fc3d-123">Parent elements</span></span>

|<span data-ttu-id="0fc3d-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fc3d-124">**Element**</span></span>|<span data-ttu-id="0fc3d-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fc3d-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fc3d-126">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="0fc3d-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="0fc3d-127">Identifie un seul délégué à ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0fc3d-128">Autorisation</span><span class="sxs-lookup"><span data-stu-id="0fc3d-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="0fc3d-129">Définit l'accès dont dispose un utilisateur dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="0fc3d-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="0fc3d-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="0fc3d-131">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="0fc3d-132">UserIds</span><span class="sxs-lookup"><span data-stu-id="0fc3d-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="0fc3d-133">Contient un tableau d’utilisateurs délégués à obtenir ou supprimer de la boîte aux lettres d’un principal.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0fc3d-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0fc3d-134">Text value</span></span>

<span data-ttu-id="0fc3d-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0fc3d-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="0fc3d-136">Remarks</span></span>

<span data-ttu-id="0fc3d-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fc3d-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fc3d-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0fc3d-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fc3d-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0fc3d-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0fc3d-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0fc3d-140">Schema Name</span></span>  <br/> |<span data-ttu-id="0fc3d-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0fc3d-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="0fc3d-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0fc3d-142">Validation File</span></span>  <br/> |<span data-ttu-id="0fc3d-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0fc3d-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0fc3d-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0fc3d-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="0fc3d-145">False</span><span class="sxs-lookup"><span data-stu-id="0fc3d-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fc3d-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0fc3d-146">See also</span></span>



[<span data-ttu-id="0fc3d-147">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="0fc3d-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="0fc3d-148">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="0fc3d-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="0fc3d-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0fc3d-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0fc3d-150">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="0fc3d-150">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

