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
ms.openlocfilehash: 7c2f31aa27c1cbde6cdad2b41a341916b4bed2ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827669"
---
# <a name="getsharingfolder"></a>GetSharingFolder

L’élément **GetSharingFolder** définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié. Il s’agit de l’élément de base pour l' [opération GetSharingFolder](getsharingfolder-operation.md).
  
```xml
<GetSharingFolder>   <SmtpAddress/>   <DataType/>   <SharedFolderId/></GetSharingFolder>
```

 **GetSharingFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Représente l’adresse de messagerie SMTP de l’autre partie de la relation de partage. Cet élément est obligatoire.  <br/> |
|[DataType](datatype.md) <br/> |Décrit le type de données qui sont partagés par un dossier partagé. Cet élément est facultatif.  <br/> |
|[SharedFolderId](sharedfolderid.md) <br/> |Représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être retourné. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Un élément GetSharingFolder doit contenir un élément de [SmtpAddress](smtpaddress.md) . Un élément GetSharingFolder doit également contenir un élément de [type de données](datatype.md) ou un élément [SharedFolderId](sharedfolderid.md) , mais ne peut pas contenir à la fois. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetSharingFolder](getsharingfolder-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

