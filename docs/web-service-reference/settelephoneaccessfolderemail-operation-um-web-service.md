---
title: Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 2c92d914-bdee-4337-b3ea-0655fdb658e9
description: L’opération SetTelephoneAccessFolderEmail définit le dossier à partir duquel la messagerie unifiée lit les messages à l’utilisateur par téléphone.
ms.openlocfilehash: cf8e80e021d6467ba3a724cc0d04e165e00e8397
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544716"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)

L’opération SetTelephoneAccessFolderEmail définit le dossier à partir duquel la messagerie unifiée lit les messages à l’utilisateur par téléphone.
  
## <a name="settelephoneaccessfolderemail-request-example"></a>Exemple de requête SetTelephoneAccessFolderEmail

### <a name="description"></a>Description

L’exemple suivant d’une demande SetTelephoneAccessFolderEmail montre comment former une demande pour définir le dossier à partir duquel la messagerie unifiée sera lue à l’utilisateur par téléphone.
  
### <a name="code"></a>Code

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

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>Exemple de réponse SetTelephoneAccessFolderEmail réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse SetTelephoneAccessFolderEmail affiche une réponse à la demande SetTelephoneAccessFolderEmail.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmailResponse (service web de messagerie unifiée)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (service web de messagerie unifiée)](base64folderid-um-web-service.md)

