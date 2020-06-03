---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: L’élément FolderShape identifie les propriétés de dossier à inclure dans une réponse GetFolder, FindFolder ou Opérationsyncfolderhierarchy.
ms.openlocfilehash: f841fcc4570604c474387dfa24ec07c9d2784f62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461344"
---
# <a name="foldershape"></a>FolderShape

L’élément **FolderShape** identifie les propriétés de dossier à inclure dans une réponse [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [opérationsyncfolderhierarchy](syncfolderhierarchy.md) . 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 **FolderResponseShapeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Identifie la configuration de base des propriétés à renvoyer dans une réponse.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifie les propriétés supplémentaires à renvoyer dans une réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande pour identifier les dossiers d’une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindFolder` <br/> |
|[GetFolder](getfolder.md) <br/> |Définit une demande d’obtention d’un dossier à partir de la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetFolder` <br/> |
|[Opérationsyncfolderhierarchy](syncfolderhierarchy.md) <br/> |Définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **FolderShape** est un élément enfant obligatoire de l’élément [FindFolder](findfolder.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple de requête suivant montre comment rechercher tous les dossiers situés dans le premier niveau du dossier boîte de réception.
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[FindFolder](findfolder.md)

