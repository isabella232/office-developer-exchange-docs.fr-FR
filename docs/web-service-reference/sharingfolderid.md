---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: L’élément SharingFolderId représente l’identificateur du dossier local dans une relation de partage.
ms.openlocfilehash: 02780251639ee651ca65d8eadded43260852aaf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526577"
---
# <a name="sharingfolderid"></a>SharingFolderId

L’élément **SharingFolderId** représente l’identificateur du dossier local dans une relation de partage. 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Contient une chaîne qui identifie un dossier dans la Banque d’Exchange. Cet attribut est obligatoire.  <br/> |
|ChangeKey  <br/> |Contient une chaîne qui identifie la version d’un dossier identifiée par l’attribut ID. Cet attribut est facultatif. Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RefreshSharingFolder](refreshsharingfolder.md) <br/> |Définit une demande d’actualisation du dossier local spécifié.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Définit une réponse à une demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

