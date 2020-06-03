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
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>Opération SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)

L’opération SetTelephoneAccessFolderEmail définit le dossier à partir duquel la messagerie unifiée lira les messages à l’utilisateur par téléphone.
  
## <a name="settelephoneaccessfolderemail-request-example"></a>Exemple de requête SetTelephoneAccessFolderEmail

### <a name="description"></a>Description

L’exemple de requête SetTelephoneAccessFolderEmail suivant montre comment créer une demande de définition du dossier à partir duquel la messagerie unifiée sera lue vers l’utilisateur par téléphone.
  
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

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>Exemple de réponse SetTelephoneAccessFolderEmail réussi

### <a name="description"></a>Description

L’exemple suivant de réponse SetTelephoneAccessFolderEmail indique une réponse à la demande SetTelephoneAccessFolderEmail.
  
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



[SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmailResponse (service Web de messagerie unifiée)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (service Web de messagerie unifiée)](base64folderid-um-web-service.md)

