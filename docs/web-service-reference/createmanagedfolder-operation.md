---
title: Opération CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: L’opération CreateManagedFolder crée un dossier géré dans la Exchange store.
ms.openlocfilehash: 2b00691fbaba294950a091d5caafb8054f3e2073
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536423"
---
# <a name="createmanagedfolder-operation"></a>Opération CreateManagedFolder

L’opération CreateManagedFolder crée un dossier géré dans la Exchange store.
  
## <a name="using-the-createmanagedfolder-operation"></a>Utilisation de l’opération CreateManagedFolder

L’opération CreateManagedFolder ajoute un dossier personnalisé géré à la boîte aux lettres d’un utilisateur. Vous pouvez utiliser la cmdlet Exchange Management Shell **Get-ManagedFolder** pour rechercher les dossiers gérés disponibles à ajouter. Bien que cette cmdlet renvoie des dossiers personnalisés gérés et des dossiers gérés par défaut, seuls les dossiers personnalisés gérés peuvent être ajoutés. Les dossiers personnalisés gérés sont identifiés par le type de dossier ManagedCustomFolder. L’espace de noms System.DirectoryServices inclut également des types qui peuvent être utilisés pour découvrir les noms des dossiers gérés disponibles. 
  
> [!NOTE]
> Vous ne pouvez pas utiliser Exchange Web Services pour rechercher les noms des dossiers gérés disponibles à ajouter à une boîte aux lettres. 
  
Vous pouvez utiliser les opérations FindFolder et GetFolder pour accéder aux dossiers gérés. FindFolder permet de rechercher des dossiers dans un dossier parent spécifié. Cela permet de découvrir des dossiers gérés dans un dossier avant d’essayer d’ajouter un dossier personnalisé géré en double dans le même répertoire. GetFolder est utilisé après l’opération FindFolder pour obtenir plus d’informations sur un dossier personnalisé géré.
  
## <a name="remarks"></a>Remarques

Pour plus d’informations sur la façon de configurer la stratégie de gestion des enregistrements de messagerie (MRM), voir [How to Create a Managed Folder Mailbox Policy](https://go.microsoft.com/fwlink/?LinkId=100975).
  
Pour plus d’informations sur la suppression de dossiers personnalisés gérés d’une boîte aux lettres, voir [Remove-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).
  
## <a name="createmanagedfolder-request-example"></a>Exemple de requête CreateManagedFolder

### <a name="description"></a>Description

L’exemple suivant d’une demande CreateManagedFolder montre comment ajouter un dossier géré nommé Dossier géré de test à une boîte aux lettres.
  
> [!NOTE]
> Vous pouvez également utiliser l’accès délégué pour ajouter des dossiers personnalisés gérés. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [FolderNames](foldernames.md)
    
- [FolderName](foldername.md)
    
Pour rechercher d’autres options pour le message de demande de l’opération CreateManagedFolder, explorez la hiérarchie de schéma. Commencez à [l’élément CreateManagedFolder.](createmanagedfolder.md) 
  
## <a name="successful-createmanagedfolder-response"></a>Réponse CreateManagedFolder réussie

### <a name="description"></a>Description

L’exemple de code suivant montre une réponse réussie à une demande CreateManagedFolder.
  
> [!NOTE]
> Les **valeurs des** attributs ID et **ChangeKey** ont été raccourcies pour préserver la lisibilité. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse : 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Pour rechercher d’autres options pour les messages de réponse de l’opération CreateManagedFolder, explorez la hiérarchie de schéma. Commencez à [l’élément CreateManagedFolderResponse.](createmanagedfolderresponse.md) 
  
## <a name="createmanagedfolder-error-response"></a>Réponse d’erreur CreateManagedFolder

### <a name="description"></a>Description

L’exemple de code suivant montre une réponse d’erreur à une demande CreateManagedFolder.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a>Voir aussi



[Opération GetFolder](getfolder-operation.md)
  
[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

