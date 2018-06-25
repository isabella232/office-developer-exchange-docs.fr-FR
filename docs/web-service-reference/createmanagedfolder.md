---
title: CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: cfdf01a9-0191-47c7-a7ad-5254d8bdee4a
description: L’élément CreateManagedFolder définit une requête pour ajouter des dossiers personnalisés gérés à une boîte aux lettres.
ms.openlocfilehash: 4acc931de2a8665db092c3b309d914f0a3c67558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755734"
---
# <a name="createmanagedfolder"></a><span data-ttu-id="8149f-103">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="8149f-103">CreateManagedFolder</span></span>

<span data-ttu-id="8149f-104">L’élément **CreateManagedFolder** définit une requête pour ajouter des dossiers personnalisés gérés à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8149f-104">The **CreateManagedFolder** element defines a request to add managed custom folders to a mailbox.</span></span> 
  
```xml
<CreateManagedFolder>
   <FolderNames/>
   <Mailbox/>
</CreateManagedFolder>
```

 <span data-ttu-id="8149f-105">**CreateManagedFolderRequestType**</span><span class="sxs-lookup"><span data-stu-id="8149f-105">**CreateManagedFolderRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8149f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8149f-106">Attributes and elements</span></span>

<span data-ttu-id="8149f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8149f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8149f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8149f-108">Attributes</span></span>

<span data-ttu-id="8149f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8149f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8149f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8149f-110">Child elements</span></span>

|<span data-ttu-id="8149f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8149f-111">**Element**</span></span>|<span data-ttu-id="8149f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8149f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8149f-113">Noms de dossier</span><span class="sxs-lookup"><span data-stu-id="8149f-113">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="8149f-114">Contient un tableau des dossiers gérés nommées à ajouter à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8149f-114">Contains an array of named managed folders to add to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8149f-115">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="8149f-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8149f-116">Identifie un objet de service d'annuaire à extension messagerie Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8149f-116">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8149f-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8149f-117">Parent elements</span></span>

<span data-ttu-id="8149f-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8149f-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8149f-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="8149f-119">Remarks</span></span>

<span data-ttu-id="8149f-120">Le compte de la personne qui effectue la demande doit posséder les autorisations de FullAccess sur la boîte aux lettres dans lequel les dossiers gérés sont créés.</span><span class="sxs-lookup"><span data-stu-id="8149f-120">The account of the person who is making the request must have FullAccess permissions on the mailbox where the managed folders are created.</span></span> <span data-ttu-id="8149f-121">Vous pouvez utiliser le paramètre de _ _ - AccessRights avec l’applet de commande Exchange Management Shell **Add-MailboxPermission** pour attribuer l’autorisation FullAccess.</span><span class="sxs-lookup"><span data-stu-id="8149f-121">You can use the _ -AccessRights _ parameter with the Exchange Management Shell **Add-MailboxPermission** cmdlet to assign the FullAccess permission.</span></span> 
  
<span data-ttu-id="8149f-122">Bien que vous pouvez utiliser les Services Web Exchange pour ajouter des dossiers gérés pour une boîte aux lettres, vous ne pouvez pas utiliser les Services Web Exchange pour accéder à la liste des dossiers gérés qui sont disponibles.</span><span class="sxs-lookup"><span data-stu-id="8149f-122">Although you can use Exchange Web Services to add managed folders to a mailbox, you cannot use Exchange Web Services to access the list of managed folders that are available.</span></span> <span data-ttu-id="8149f-123">Pour obtenir une liste des dossiers gérés disponibles, utilisez l’applet de commande **get-managedfolder** Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="8149f-123">To obtain a list of available managed folders, use the **get-managedfolder** Exchange Management Shell cmdlet.</span></span> <span data-ttu-id="8149f-124">La liste qui est renvoyée par la **cmdlet get-managedfolder** contiendra des dossiers personnalisés gérés et dossiers gérés par défaut.</span><span class="sxs-lookup"><span data-stu-id="8149f-124">The list that is returned by the **get-managedfolder cmdlet** will contain both managed custom folders and managed default folders.</span></span> <span data-ttu-id="8149f-125">Vous pouvez uniquement ajouter des dossiers de type **managedcustomfolder** la boîte aux lettres à l’aide de l’opération CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="8149f-125">You can only add folders of type **managedcustomfolder** to the mailbox by using the CreateManagedFolder operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8149f-126">Vous pouvez également obtenir une liste des dossiers gérés à l’aide de l’API DirectoryServices de Microsoft .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="8149f-126">You can also get a list of managed folders by using the DirectoryServices API of the Microsoft .NET Framework.</span></span> 
  
<span data-ttu-id="8149f-127">Vous pouvez utiliser l' [opération FindFolder](findfolder-operation.md) pour rechercher les dossiers gérés dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8149f-127">You can use the [FindFolder operation](findfolder-operation.md) to find managed folders in a mailbox.</span></span> <span data-ttu-id="8149f-128">Dossiers gérés peuvent être distingués en définissant l’élément [BaseShape](baseshape.md) AllProperties dans la demande.</span><span class="sxs-lookup"><span data-stu-id="8149f-128">Managed folders can be distinguished by setting the [BaseShape](baseshape.md) element to AllProperties in the request.</span></span> <span data-ttu-id="8149f-129">La réponse contient un élément [ManagedFolderInformation](managedfolderinformation.md) pour distinguer les dossiers gérés dans les dossiers de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="8149f-129">The response will contain a [ManagedFolderInformation](managedfolderinformation.md) element to distinguish the managed folders from the Exchange store folders.</span></span> <span data-ttu-id="8149f-130">Vous pouvez supprimer des dossiers gérés de la même manière que vous supprimez d’autres types de dossier.</span><span class="sxs-lookup"><span data-stu-id="8149f-130">You can delete managed folders in the same manner that you delete other folder types.</span></span> 
  
<span data-ttu-id="8149f-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8149f-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8149f-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8149f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8149f-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8149f-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8149f-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8149f-134">Schema Name</span></span>  <br/> |<span data-ttu-id="8149f-135">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8149f-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8149f-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8149f-136">Validation File</span></span>  <br/> |<span data-ttu-id="8149f-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8149f-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8149f-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8149f-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="8149f-139">False</span><span class="sxs-lookup"><span data-stu-id="8149f-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8149f-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8149f-140">See also</span></span>



[<span data-ttu-id="8149f-141">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="8149f-141">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)
  
[<span data-ttu-id="8149f-142">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="8149f-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="8149f-143">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="8149f-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="8149f-144">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="8149f-144">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

