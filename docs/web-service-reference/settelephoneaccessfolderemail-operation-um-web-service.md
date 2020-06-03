---
title: Opération SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 2c92d914-bdee-4337-b3ea-0655fdb658e9
description: L’opération SetTelephoneAccessFolderEmail définit le dossier à partir duquel la messagerie unifiée lira les messages à l’utilisateur par téléphone.
ms.openlocfilehash: a2bb630f812ca811b4cbe68db1308dc18e5d3ba0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467332"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a><span data-ttu-id="e4dc0-103">Opération SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e4dc0-103">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>

<span data-ttu-id="e4dc0-104">L’opération SetTelephoneAccessFolderEmail définit le dossier à partir duquel la messagerie unifiée lira les messages à l’utilisateur par téléphone.</span><span class="sxs-lookup"><span data-stu-id="e4dc0-104">The SetTelephoneAccessFolderEmail operation sets the folder from which Unified Messaging will read back messages to the user over the telephone.</span></span>
  
## <a name="settelephoneaccessfolderemail-request-example"></a><span data-ttu-id="e4dc0-105">Exemple de requête SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="e4dc0-105">SetTelephoneAccessFolderEmail request example</span></span>

### <a name="description"></a><span data-ttu-id="e4dc0-106">Description</span><span class="sxs-lookup"><span data-stu-id="e4dc0-106">Description</span></span>

<span data-ttu-id="e4dc0-107">L’exemple de requête SetTelephoneAccessFolderEmail suivant montre comment créer une demande de définition du dossier à partir duquel la messagerie unifiée sera lue vers l’utilisateur par téléphone.</span><span class="sxs-lookup"><span data-stu-id="e4dc0-107">The following example of a SetTelephoneAccessFolderEmail request shows how to form a request to set the folder from which Unified Messaging will read back to the user over the telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="e4dc0-108">Code</span><span class="sxs-lookup"><span data-stu-id="e4dc0-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a><span data-ttu-id="e4dc0-109">Exemple de réponse SetTelephoneAccessFolderEmail réussi</span><span class="sxs-lookup"><span data-stu-id="e4dc0-109">Successful SetTelephoneAccessFolderEmail response example</span></span>

### <a name="description"></a><span data-ttu-id="e4dc0-110">Description</span><span class="sxs-lookup"><span data-stu-id="e4dc0-110">Description</span></span>

<span data-ttu-id="e4dc0-111">L’exemple suivant de réponse SetTelephoneAccessFolderEmail indique une réponse à la demande SetTelephoneAccessFolderEmail.</span><span class="sxs-lookup"><span data-stu-id="e4dc0-111">The following example of a SetTelephoneAccessFolderEmail response shows a response to the SetTelephoneAccessFolderEmail request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e4dc0-112">Code</span><span class="sxs-lookup"><span data-stu-id="e4dc0-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="e4dc0-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e4dc0-113">See also</span></span>



[<span data-ttu-id="e4dc0-114">SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e4dc0-114">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="e4dc0-115">SetTelephoneAccessFolderEmailResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e4dc0-115">SetTelephoneAccessFolderEmailResponse (UM web service)</span></span>](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[<span data-ttu-id="e4dc0-116">base64FolderId (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="e4dc0-116">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)

