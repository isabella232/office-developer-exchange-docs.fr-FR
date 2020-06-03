---
title: Opération CreateManagedFolder
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
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: L’opération CreateManagedFolder crée un dossier géré dans la Banque d’Exchange.
ms.openlocfilehash: 779c730b55b9b441644108a6837f9e22d39cc2f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44444592"
---
# <a name="createmanagedfolder-operation"></a>Opération CreateManagedFolder

L’opération CreateManagedFolder crée un dossier géré dans la Banque d’Exchange.
  
## <a name="using-the-createmanagedfolder-operation"></a>Utilisation de l’opération CreateManagedFolder

L’opération CreateManagedFolder ajoute un dossier personnalisé géré à la boîte aux lettres d’un utilisateur. Vous pouvez utiliser la cmdlet **Get-ManagedFolder** de l’environnement de commande Exchange Management Shell pour rechercher les dossiers gérés à ajouter. Bien que cette applet de commande renvoie les dossiers personnalisés gérés et les dossiers par défaut gérés, seuls les dossiers personnalisés gérés peuvent être ajoutés. Les dossiers personnalisés gérés sont identifiés par le type de dossier ManagedCustomFolder. L’espace de noms System. DirectoryServices inclut également des types qui peuvent être utilisés pour découvrir les noms des dossiers gérés disponibles. 
  
> [!NOTE]
> Vous ne pouvez pas utiliser les services Web Exchange pour rechercher les noms des dossiers gérés disponibles à ajouter à une boîte aux lettres. 
  
Vous pouvez utiliser les opérations FindFolder et GetFolder pour accéder aux dossiers gérés. FindFolder permet de rechercher des dossiers dans un dossier parent spécifié. Cela peut être utilisé afin que les dossiers gérés puissent être découverts dans un dossier avant d’essayer d’ajouter un dossier personnalisé géré en double dans le même répertoire. GetFolder est utilisé après l’opération FindFolder pour obtenir plus d’informations sur un dossier personnalisé géré.
  
## <a name="remarks"></a>Remarques

Pour plus d’informations sur la configuration de la stratégie de gestion des enregistrements de messagerie (MRM), voir [comment créer une stratégie de boîte aux lettres de dossier géré](https://go.microsoft.com/fwlink/?LinkId=100975).
  
Pour plus d’informations sur la suppression de dossiers personnalisés gérés d’une boîte aux lettres, consultez la rubrique [Remove-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).
  
## <a name="createmanagedfolder-request-example"></a>Exemple de requête CreateManagedFolder

### <a name="description"></a>Description

L’exemple de requête CreateManagedFolder suivant montre comment ajouter un dossier géré nommé test du dossier géré à une boîte aux lettres.
  
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

### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [FolderNames](foldernames.md)
    
- [FolderName](foldername.md)
    
Pour trouver d’autres options pour le message de demande de l’opération CreateManagedFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CreateManagedFolder](createmanagedfolder.md) . 
  
## <a name="successful-createmanagedfolder-response"></a>Réponse CreateManagedFolder réussie

### <a name="description"></a>Description

L’exemple de code suivant montre une réponse réussie à une demande CreateManagedFolder.
  
> [!NOTE]
> Les valeurs d’attribut **ID** et **ChangeKey** ont été raccourcies afin de préserver la lisibilité. 
  
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
    
Pour rechercher d’autres options pour les messages de réponse de l’opération CreateManagedFolder, explorez la hiérarchie du schéma. Commencez par l’élément [CreateManagedFolderResponse](createmanagedfolderresponse.md) . 
  
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

