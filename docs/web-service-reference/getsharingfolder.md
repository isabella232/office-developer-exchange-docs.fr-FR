---
title: GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: ed5bb61f-89c7-4baa-83ee-30f06a49ff9b
description: L’élément GetSharingFolder définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié. Il s’agit de l’élément de base pour l’opération GetSharingFolder.
ms.openlocfilehash: cb76c534d9b30d0a9d1b267396551eb2871e638a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460504"
---
# <a name="getsharingfolder"></a><span data-ttu-id="d1b3f-104">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="d1b3f-104">GetSharingFolder</span></span>

<span data-ttu-id="d1b3f-105">L’élément **GetSharingFolder** définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-105">The **GetSharingFolder** element defines a request to get the local folder identifier of a specified shared folder.</span></span> <span data-ttu-id="d1b3f-106">Il s’agit de l’élément de base pour l' [opération GetSharingFolder](getsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d1b3f-106">It is the base element for the [GetSharingFolder operation](getsharingfolder-operation.md).</span></span>
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 <span data-ttu-id="d1b3f-107">**GetSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="d1b3f-107">**GetSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1b3f-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d1b3f-108">Attributes and elements</span></span>

<span data-ttu-id="d1b3f-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1b3f-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d1b3f-110">Attributes</span></span>

<span data-ttu-id="d1b3f-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1b3f-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d1b3f-112">Child elements</span></span>

|<span data-ttu-id="d1b3f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d1b3f-113">**Element**</span></span>|<span data-ttu-id="d1b3f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d1b3f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1b3f-115">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="d1b3f-115">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="d1b3f-116">Représente l’adresse de messagerie SMTP de l’autre partie dans la relation de partage.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-116">Represents the SMTP e-mail address of the other party in the sharing relationship.</span></span> <span data-ttu-id="d1b3f-117">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-117">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d1b3f-118">DataType</span><span class="sxs-lookup"><span data-stu-id="d1b3f-118">DataType</span></span>](datatype.md) <br/> |<span data-ttu-id="d1b3f-119">Décrit le type de données partagées par un dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-119">Describes the type of data that is shared by a shared folder.</span></span> <span data-ttu-id="d1b3f-120">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d1b3f-121">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="d1b3f-121">SharedFolderId</span></span>](sharedfolderid.md) <br/> |<span data-ttu-id="d1b3f-122">Représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-122">Represents the identifier of the shared folder whose local folder identifier should be returned.</span></span> <span data-ttu-id="d1b3f-123">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-123">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d1b3f-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d1b3f-124">Parent elements</span></span>

<span data-ttu-id="d1b3f-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d1b3f-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="d1b3f-126">Remarks</span></span>

<span data-ttu-id="d1b3f-127">Un élément GetSharingFolder doit contenir un élément [SmtpAddress](smtpaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="d1b3f-127">A GetSharingFolder element must contain an [SmtpAddress](smtpaddress.md) element.</span></span> <span data-ttu-id="d1b3f-128">Un élément GetSharingFolder doit également contenir un élément [DataType](datatype.md) ou un élément [SharedFolderId](sharedfolderid.md) , mais ne peut pas contenir les deux.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-128">A GetSharingFolder element must also contain either a [DataType](datatype.md) element or a [SharedFolderId](sharedfolderid.md) element, but cannot contain both.</span></span> 
  
<span data-ttu-id="d1b3f-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d1b3f-129">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1b3f-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d1b3f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1b3f-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d1b3f-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d1b3f-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d1b3f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d1b3f-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d1b3f-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d1b3f-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d1b3f-134">Validation File</span></span>  <br/> |<span data-ttu-id="d1b3f-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d1b3f-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1b3f-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d1b3f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1b3f-137">False</span><span class="sxs-lookup"><span data-stu-id="d1b3f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1b3f-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d1b3f-138">See also</span></span>



[<span data-ttu-id="d1b3f-139">Opération GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="d1b3f-139">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="d1b3f-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d1b3f-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

