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
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838957"
---
# <a name="userid"></a><span data-ttu-id="e5aae-103">UserId</span><span class="sxs-lookup"><span data-stu-id="e5aae-103">UserId</span></span>

<span data-ttu-id="e5aae-104">L’élément **UserId** identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="e5aae-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="e5aae-105">**UserIdType**</span><span class="sxs-lookup"><span data-stu-id="e5aae-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5aae-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e5aae-106">Attributes and elements</span></span>

<span data-ttu-id="e5aae-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e5aae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5aae-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e5aae-108">Attributes</span></span>

<span data-ttu-id="e5aae-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e5aae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5aae-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e5aae-110">Child elements</span></span>

|<span data-ttu-id="e5aae-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e5aae-111">**Element**</span></span>|<span data-ttu-id="e5aae-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e5aae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5aae-113">SID</span><span class="sxs-lookup"><span data-stu-id="e5aae-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="e5aae-114">Représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID).</span><span class="sxs-lookup"><span data-stu-id="e5aae-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="e5aae-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="e5aae-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="e5aae-116">Représente l’adresse SMTP Simple Mail Transfer Protocol () principal d’un compte à utiliser pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="e5aae-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="e5aae-117">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="e5aae-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e5aae-118">Définit le nom complet d’un dossier, un contact, une liste de distribution ou un utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="e5aae-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="e5aae-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="e5aae-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="e5aae-120">Identifie les comptes d’utilisateurs par défaut et anonymes pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="e5aae-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="e5aae-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="e5aae-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="e5aae-122">Identifie un utilisateur délégué externe ou un utilisateur externe qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="e5aae-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5aae-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e5aae-123">Parent elements</span></span>

|<span data-ttu-id="e5aae-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e5aae-124">**Element**</span></span>|<span data-ttu-id="e5aae-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="e5aae-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5aae-126">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="e5aae-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="e5aae-127">Identifie un délégué pour ajouter ou mettre à jour dans une boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="e5aae-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="e5aae-128">Autorisation</span><span class="sxs-lookup"><span data-stu-id="e5aae-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="e5aae-129">Définit l'accès dont dispose un utilisateur dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="e5aae-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="e5aae-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="e5aae-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="e5aae-131">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="e5aae-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="e5aae-132">ID utilisateur</span><span class="sxs-lookup"><span data-stu-id="e5aae-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="e5aae-133">Contient un tableau d’utilisateurs délégué d’obtenir ou de supprimer la boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="e5aae-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5aae-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e5aae-134">Text value</span></span>

<span data-ttu-id="e5aae-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e5aae-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e5aae-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="e5aae-136">Remarks</span></span>

<span data-ttu-id="e5aae-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e5aae-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5aae-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e5aae-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5aae-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e5aae-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5aae-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e5aae-140">Schema Name</span></span>  <br/> |<span data-ttu-id="e5aae-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e5aae-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="e5aae-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e5aae-142">Validation File</span></span>  <br/> |<span data-ttu-id="e5aae-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e5aae-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5aae-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e5aae-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5aae-145">False</span><span class="sxs-lookup"><span data-stu-id="e5aae-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5aae-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e5aae-146">See also</span></span>



[<span data-ttu-id="e5aae-147">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="e5aae-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="e5aae-148">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="e5aae-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="e5aae-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e5aae-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e5aae-150">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="e5aae-150">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

