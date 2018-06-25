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
description: L’opération CreateManagedFolder crée un dossier géré dans la banque d’informations Exchange.
ms.openlocfilehash: 2c2af53dc5dbe1e6fcbc7f3b1174a856e51e4905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755735"
---
# <a name="createmanagedfolder-operation"></a>Opération CreateManagedFolder

L’opération CreateManagedFolder crée un dossier géré dans la banque d’informations Exchange.
  
## <a name="using-the-createmanagedfolder-operation"></a>Utilisation de l’opération CreateManagedFolder

L’opération CreateManagedFolder ajoute un dossier personnalisé géré à la boîte aux lettres d’un utilisateur. Vous pouvez utiliser l’applet de commande Exchange Management Shell, **Get-ManagedFolder** pour rechercher les dossiers gérés disponibles à ajouter. Bien que cette applet de commande renvoie les dossiers personnalisés gérés et les dossiers gérés par défaut uniquement gérés personnalisés dossiers peuvent être ajoutés. Dossiers personnalisés gérés sont identifiés par le type de dossier ManagedCustomFolder. L’espace de noms System.DirectoryServices inclut également les types qui peuvent être utilisés pour découvrir les noms des dossiers gérés disponibles. 
  
> [!NOTE]
> Vous ne pouvez pas utiliser les Services Web Exchange pour rechercher les noms de dossiers gérés disponibles à ajouter à une boîte aux lettres. 
  
Vous pouvez utiliser les opérations FindFolder et GetFolder pour accéder aux dossiers gérés. FindFolder est utilisé pour rechercher des dossiers dans un dossier parent spécifié. Cela peut être utilisé pour que les dossiers gérés peuvent être découverts dans un dossier avant la tentative d’ajout de qu'un dossier personnalisé dans le même répertoire géré par un double. GetFolder est utilisée après l’opération FindFolder pour obtenir plus d’informations sur un dossier personnalisé géré.
  
## <a name="remarks"></a>Remarques

Pour plus d’informations sur la façon de configurer la stratégie de gestion (MRM) des enregistrements de messagerie, voir [comment créer une stratégie de boîte aux lettres de dossier géré](http://go.microsoft.com/fwlink/?LinkId=100975).
  
Pour plus d’informations sur la suppression des dossiers personnalisés gérés à partir d’une boîte aux lettres, voir [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).
  
## <a name="createmanagedfolder-request-example"></a>Exemple de requête CreateManagedFolder

### <a name="description"></a>Description

Une demande CreateManagedFolder l’exemple suivant montre comment ajouter un dossier géré nommé dossier géré de Test pour une boîte aux lettres.
  
> [!NOTE]
> Vous pouvez également utiliser l’accès délégué pour ajouter des dossiers personnalisés gérés. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [CreateManagedFolder](createmanagedfolder.md)
    
- [Noms de dossier](foldernames.md)
    
- [FolderName](foldername.md)
    
Pour trouver d’autres options pour le message de demande de l’opération CreateManagedFolder, explorez la hiérarchie de schéma. Commencer à l’élément [CreateManagedFolder](createmanagedfolder.md) . 
  
## <a name="successful-createmanagedfolder-response"></a>Réponse CreateManagedFolder réussie

### <a name="description"></a>Description

L’exemple de code suivant montre une réponse positive à une demande CreateManagedFolder.
  
> [!NOTE]
> Les valeurs d’attribut **Id** et **ChangeKey** ont été réduits afin de préserver la lisibilité. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse : 
  
- [CreateManagedFolderResponse](createmanagedfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
Pour trouver d’autres options pour les messages de réponse de l’opération CreateManagedFolder, explorez la hiérarchie de schéma. Démarrez au niveau de l’élément [CreateManagedFolderResponse](createmanagedfolderresponse.md) . 
  
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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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


[Recherche de dossiers](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

