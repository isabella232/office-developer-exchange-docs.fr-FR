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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838957"
---
# <a name="userid"></a><span data-ttu-id="aef53-103">UserId</span><span class="sxs-lookup"><span data-stu-id="aef53-103">UserId</span></span>

<span data-ttu-id="aef53-104">L’élément **UserId** identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="aef53-104">The **UserId** element identifies a delegate user or a user who has folder access permissions.</span></span> 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 <span data-ttu-id="aef53-105">**UserIdType**</span><span class="sxs-lookup"><span data-stu-id="aef53-105">**UserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aef53-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aef53-106">Attributes and elements</span></span>

<span data-ttu-id="aef53-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aef53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aef53-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="aef53-108">Attributes</span></span>

<span data-ttu-id="aef53-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aef53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aef53-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aef53-110">Child elements</span></span>

|<span data-ttu-id="aef53-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aef53-111">**Element**</span></span>|<span data-ttu-id="aef53-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="aef53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aef53-113">SID</span><span class="sxs-lookup"><span data-stu-id="aef53-113">SID</span></span>](sid.md) <br/> |<span data-ttu-id="aef53-114">Représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID).</span><span class="sxs-lookup"><span data-stu-id="aef53-114">Represents the security descriptor definition language (SDDL) form of the security identifier (SID).</span></span>  <br/> |
|[<span data-ttu-id="aef53-115">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="aef53-115">PrimarySmtpAddress</span></span>](primarysmtpaddress.md) <br/> |<span data-ttu-id="aef53-116">Représente l’adresse SMTP Simple Mail Transfer Protocol () principal d’un compte à utiliser pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="aef53-116">Represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="aef53-117">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="aef53-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="aef53-118">Définit le nom complet d’un dossier, un contact, une liste de distribution ou un utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="aef53-118">Defines the display name of a folder, contact, distribution list, or delegate user.</span></span>  <br/> |
|[<span data-ttu-id="aef53-119">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="aef53-119">DistinguishedUser</span></span>](distinguisheduser.md) <br/> |<span data-ttu-id="aef53-120">Identifie les comptes d’utilisateurs par défaut et anonymes pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="aef53-120">Identifies Anonymous and Default user accounts for delegate access.</span></span>  <br/> |
|[<span data-ttu-id="aef53-121">ExternalUserIdentity</span><span class="sxs-lookup"><span data-stu-id="aef53-121">ExternalUserIdentity</span></span>](externaluseridentity.md) <br/> |<span data-ttu-id="aef53-122">Identifie un utilisateur délégué externe ou un utilisateur externe qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="aef53-122">Identifies an external delegate user or an external user who has folder access permissions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aef53-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aef53-123">Parent elements</span></span>

|<span data-ttu-id="aef53-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aef53-124">**Element**</span></span>|<span data-ttu-id="aef53-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="aef53-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aef53-126">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="aef53-126">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="aef53-127">Identifie un délégué pour ajouter ou mettre à jour dans une boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="aef53-127">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="aef53-128">Autorisation</span><span class="sxs-lookup"><span data-stu-id="aef53-128">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="aef53-129">Définit l'accès dont dispose un utilisateur dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="aef53-129">Defines the access that a user has to a folder.</span></span>  <br/> |
|[<span data-ttu-id="aef53-130">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="aef53-130">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="aef53-131">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="aef53-131">Defines the access that a user has to a Calendar folder.</span></span>  <br/> |
|[<span data-ttu-id="aef53-132">ID utilisateur</span><span class="sxs-lookup"><span data-stu-id="aef53-132">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="aef53-133">Contient un tableau d’utilisateurs délégué d’obtenir ou de supprimer la boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="aef53-133">Contains an array of delegate users to get or remove from a principal's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aef53-134">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="aef53-134">Text value</span></span>

<span data-ttu-id="aef53-135">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aef53-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aef53-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="aef53-136">Remarks</span></span>

<span data-ttu-id="aef53-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="aef53-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aef53-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="aef53-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aef53-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="aef53-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aef53-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="aef53-140">Schema Name</span></span>  <br/> |<span data-ttu-id="aef53-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="aef53-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="aef53-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="aef53-142">Validation File</span></span>  <br/> |<span data-ttu-id="aef53-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aef53-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aef53-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="aef53-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="aef53-145">False</span><span class="sxs-lookup"><span data-stu-id="aef53-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aef53-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aef53-146">See also</span></span>



[<span data-ttu-id="aef53-147">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="aef53-147">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="aef53-148">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="aef53-148">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="aef53-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="aef53-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="aef53-150">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="aef53-150">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

