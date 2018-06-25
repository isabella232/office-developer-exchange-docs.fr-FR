---
title: Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)
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
description: L’opération SetTelephoneAccessFolderEmail définit le dossier à partir duquel la messagerie unifiée lira arrière de messages à l’utilisateur par téléphone.
ms.openlocfilehash: 9497e58f66b8efcf7e358aa529223942298a3bed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829459"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)

L’opération SetTelephoneAccessFolderEmail définit le dossier à partir duquel la messagerie unifiée lira arrière de messages à l’utilisateur par téléphone.
  
## <a name="settelephoneaccessfolderemail-request-example"></a>Exemple de requête SetTelephoneAccessFolderEmail

### <a name="description"></a>Description

L’exemple suivant d’une demande SetTelephoneAccessFolderEmail montre comment former une demande pour définir le dossier à partir duquel la messagerie unifiée lira à l’utilisateur par téléphone.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>Exemple de réponse SetTelephoneAccessFolderEmail réussie

### <a name="description"></a>Description

Une réponse SetTelephoneAccessFolderEmail l’exemple suivant montre une réponse à la demande SetTelephoneAccessFolderEmail.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetTelephoneAccessFolderEmail (service web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmailResponse (service web de messagerie unifiée)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (service web de messagerie unifiée)](base64folderid-um-web-service.md)

