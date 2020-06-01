---
title: Opération UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'L’opération UpdateFolder est utilisée pour modifier les propriétés d’un élément existant dans la Banque d’Exchange. Chaque opération UpdateFolder comprend les éléments suivants :'
ms.openlocfilehash: fb894d9f42358b67f81e9fe8ae41ba61e6f46460
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467360"
---
# <a name="updatefolder-operation"></a><span data-ttu-id="5bebe-104">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5bebe-104">UpdateFolder operation</span></span>

<span data-ttu-id="5bebe-105">L’opération UpdateFolder est utilisée pour modifier les propriétés d’un élément existant dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="5bebe-105">The UpdateFolder operation is used to modify properties of an existing item in the Exchange store.</span></span> <span data-ttu-id="5bebe-106">Chaque opération UpdateFolder comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5bebe-106">Each UpdateFolder operation consists of the following:</span></span>
  
- <span data-ttu-id="5bebe-107">Élément [FolderId](folderid.md) qui spécifie un dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="5bebe-107">A [FolderId](folderid.md) element that specifies a folder to update.</span></span> 
    
- <span data-ttu-id="5bebe-108">Chemin d’accès interne d’un élément dans le dossier, tel que spécifié par la forme Folder, qui spécifie les données à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="5bebe-108">An internal path of an element in the folder, as specified by the folder shape, which specifies the data to update.</span></span>
    
- <span data-ttu-id="5bebe-109">Dossier qui contient la nouvelle valeur du champ mis à jour, si la mise à jour n’est pas une suppression.</span><span class="sxs-lookup"><span data-stu-id="5bebe-109">A folder that contains the new value of the updated field, if the update is not a deletion.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="5bebe-110">Remarques</span><span class="sxs-lookup"><span data-stu-id="5bebe-110">Remarks</span></span>

<span data-ttu-id="5bebe-111">Trois actions de mise à jour de base peuvent être effectuées sur un élément.</span><span class="sxs-lookup"><span data-stu-id="5bebe-111">Three basic update actions can be performed on an item.</span></span> <span data-ttu-id="5bebe-112">Ces actions sont répertoriées dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5bebe-112">These actions are listed in the following table.</span></span>
  
|<span data-ttu-id="5bebe-113">**Action**</span><span class="sxs-lookup"><span data-stu-id="5bebe-113">**Action**</span></span>|<span data-ttu-id="5bebe-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5bebe-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5bebe-115">Ajout</span><span class="sxs-lookup"><span data-stu-id="5bebe-115">Append</span></span>  <br/> |<span data-ttu-id="5bebe-116">L’action Append ajoute des données à une propriété existante.</span><span class="sxs-lookup"><span data-stu-id="5bebe-116">The append action adds data to an existing property.</span></span> <span data-ttu-id="5bebe-117">Il conserve les données qui s’y trouvent actuellement.</span><span class="sxs-lookup"><span data-stu-id="5bebe-117">It preserves the data that is currently there.</span></span> <span data-ttu-id="5bebe-118">Append n’est pas applicable à toutes les propriétés.</span><span class="sxs-lookup"><span data-stu-id="5bebe-118">Append is not applicable to all properties.</span></span>  <br/> |
|<span data-ttu-id="5bebe-119">Set</span><span class="sxs-lookup"><span data-stu-id="5bebe-119">Set</span></span>  <br/> |<span data-ttu-id="5bebe-120">L’action Set remplace les données d’une propriété si celle-ci contient des données, ou crée la propriété et définit sa valeur si elle n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="5bebe-120">The set action replaces data for a property if it contains data, or creates the property and sets its value if it does not exist.</span></span> <span data-ttu-id="5bebe-121">L’action set n’est applicable qu’aux propriétés accessibles en écriture.</span><span class="sxs-lookup"><span data-stu-id="5bebe-121">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="5bebe-122">Supprimer</span><span class="sxs-lookup"><span data-stu-id="5bebe-122">Delete</span></span>  <br/> |<span data-ttu-id="5bebe-123">L’action Supprimer supprime une propriété d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="5bebe-123">The delete action removes a property from a folder.</span></span> <span data-ttu-id="5bebe-124">Elle est différente de la définition d’une valeur vide.</span><span class="sxs-lookup"><span data-stu-id="5bebe-124">This is different than setting it to an empty value.</span></span> <span data-ttu-id="5bebe-125">Lorsque vous avez terminé, la propriété n’existe pas pour le dossier.</span><span class="sxs-lookup"><span data-stu-id="5bebe-125">When complete, the property does not exist for the folder.</span></span> <span data-ttu-id="5bebe-126">La méthode Delete n’est applicable qu’aux propriétés accessibles en écriture.</span><span class="sxs-lookup"><span data-stu-id="5bebe-126">Delete is only applicable to writable properties.</span></span>  <br/> |
   
## <a name="updatefolder-request-example"></a><span data-ttu-id="5bebe-127">Exemple de requête UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5bebe-127">UpdateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="5bebe-128">Description</span><span class="sxs-lookup"><span data-stu-id="5bebe-128">Description</span></span>

<span data-ttu-id="5bebe-129">L’exemple de requête UpdateFolder suivant montre comment mettre à jour le nom d’affichage d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="5bebe-129">The following example of an UpdateFolder request shows how to update a folder display name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5bebe-130">Code</span><span class="sxs-lookup"><span data-stu-id="5bebe-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AScA" ChangeKey="GO3u/"/>
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName"/>
              <t:Folder>
                <t:DisplayName>NewFolderName</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </FolderChanges>
    </UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5bebe-131">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5bebe-131">Comments</span></span>

<span data-ttu-id="5bebe-132">Cet exemple montre comment modifier le nom d’affichage du dossier en NewFolderName.</span><span class="sxs-lookup"><span data-stu-id="5bebe-132">This example changes the display name of the folder to NewFolderName.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5bebe-133">Les valeurs des attributs **ID** et **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5bebe-133">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="5bebe-134">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="5bebe-134">Request elements</span></span>

<span data-ttu-id="5bebe-135">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="5bebe-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5bebe-136">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5bebe-136">UpdateFolder</span></span>](updatefolder.md)
    
- [<span data-ttu-id="5bebe-137">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="5bebe-137">FolderChanges</span></span>](folderchanges.md)
    
- [<span data-ttu-id="5bebe-138">FolderChange</span><span class="sxs-lookup"><span data-stu-id="5bebe-138">FolderChange</span></span>](folderchange.md)
    
- [<span data-ttu-id="5bebe-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="5bebe-139">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="5bebe-140">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="5bebe-140">Updates (Folder)</span></span>](updates-folder.md)
    
- [<span data-ttu-id="5bebe-141">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="5bebe-141">SetFolderField</span></span>](setfolderfield.md)
    
- [<span data-ttu-id="5bebe-142">FieldURI</span><span class="sxs-lookup"><span data-stu-id="5bebe-142">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="5bebe-143">Folder</span><span class="sxs-lookup"><span data-stu-id="5bebe-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5bebe-144">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5bebe-144">DisplayName (string)</span></span>](displayname-string.md)
    
<span data-ttu-id="5bebe-145">Consultez le schéma pour les éléments supplémentaires que vous pouvez utiliser pour former une requête UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="5bebe-145">See the schema for additional elements that you can use to form an UpdateFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5bebe-146">L’emplacement par défaut du schéma se trouve dans le répertoire virtuel EWS de l’ordinateur sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5bebe-146">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="updatefolder-response-example"></a><span data-ttu-id="5bebe-147">Exemple de réponse UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5bebe-147">UpdateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="5bebe-148">Description</span><span class="sxs-lookup"><span data-stu-id="5bebe-148">Description</span></span>

<span data-ttu-id="5bebe-149">L’exemple suivant montre une réponse réussie à la demande UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="5bebe-149">The following example shows a successful response to the UpdateFolder request.</span></span> <span data-ttu-id="5bebe-150">Dans cet exemple, la nouvelle clé de modification est renvoyée pour refléter l’État mis à jour du dossier.</span><span class="sxs-lookup"><span data-stu-id="5bebe-150">In this example, the new change key is returned to reflect the updated status of the folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="5bebe-151">Code</span><span class="sxs-lookup"><span data-stu-id="5bebe-151">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFVz" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5bebe-152">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5bebe-152">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="5bebe-153">L’ID de dossier et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5bebe-153">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="5bebe-154">L’ID de dossier renvoyé dans la réponse représente le dossier mis à jour.</span><span class="sxs-lookup"><span data-stu-id="5bebe-154">The folder ID that is returned in the response represents the updated folder.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="5bebe-155">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="5bebe-155">Successful response elements</span></span>

<span data-ttu-id="5bebe-156">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5bebe-156">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5bebe-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5bebe-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5bebe-158">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5bebe-158">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="5bebe-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5bebe-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5bebe-160">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5bebe-160">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="5bebe-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5bebe-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5bebe-162">Dossiers</span><span class="sxs-lookup"><span data-stu-id="5bebe-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5bebe-163">Folder</span><span class="sxs-lookup"><span data-stu-id="5bebe-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5bebe-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="5bebe-164">FolderId</span></span>](folderid.md)
    
## <a name="updatefolder-error-response-example"></a><span data-ttu-id="5bebe-165">Exemple de réponse d’erreur UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5bebe-165">UpdateFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="5bebe-166">Description</span><span class="sxs-lookup"><span data-stu-id="5bebe-166">Description</span></span>

<span data-ttu-id="5bebe-167">L’exemple suivant montre une réponse d’erreur à une demande UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="5bebe-167">The following example shows an error response to an UpdateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5bebe-168">Code</span><span class="sxs-lookup"><span data-stu-id="5bebe-168">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5bebe-169">Commentaires</span><span class="sxs-lookup"><span data-stu-id="5bebe-169">Comments</span></span>

<span data-ttu-id="5bebe-170">Cet exemple montre une réponse d’erreur causée par un attribut **ChangeKey** non valide dans la demande.</span><span class="sxs-lookup"><span data-stu-id="5bebe-170">This example shows an error response that is caused by an invalid **ChangeKey** attribute in the request.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="5bebe-171">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="5bebe-171">Error response elements</span></span>

<span data-ttu-id="5bebe-172">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="5bebe-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="5bebe-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5bebe-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5bebe-174">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5bebe-174">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="5bebe-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5bebe-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5bebe-176">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5bebe-176">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="5bebe-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="5bebe-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5bebe-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5bebe-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5bebe-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5bebe-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5bebe-180">Dossiers</span><span class="sxs-lookup"><span data-stu-id="5bebe-180">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="5bebe-181">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5bebe-181">See also</span></span>



- [<span data-ttu-id="5bebe-182">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5bebe-182">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

