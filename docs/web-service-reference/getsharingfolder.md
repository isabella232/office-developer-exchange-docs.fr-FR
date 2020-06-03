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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460504"
---
# <a name="getsharingfolder"></a>GetSharingFolder

L’élément **GetSharingFolder** définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié. Il s’agit de l’élément de base pour l' [opération GetSharingFolder](getsharingfolder-operation.md).
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **GetSharingFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Représente l’adresse de messagerie SMTP de l’autre partie dans la relation de partage. Cet élément est obligatoire.  <br/> |
|[DataType](datatype.md) <br/> |Décrit le type de données partagées par un dossier partagé. Cet élément est facultatif.  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |Représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Un élément GetSharingFolder doit contenir un élément [SmtpAddress](smtpaddress.md) . Un élément GetSharingFolder doit également contenir un élément [DataType](datatype.md) ou un élément [SharedFolderId](sharedfolderid.md) , mais ne peut pas contenir les deux. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetSharingFolder](getsharingfolder-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

