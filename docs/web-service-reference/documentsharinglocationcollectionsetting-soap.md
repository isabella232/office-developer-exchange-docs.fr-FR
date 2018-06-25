---
title: DocumentSharingLocationCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e3346f9-7a55-4e87-b121-9b1ee7f227f4
description: L’élément DocumentSharingLocationCollectionSetting représente un utilisateur de paramètre qui est une collection de documentation de métadonnées et les emplacements de partage.
ms.openlocfilehash: 9871e3fccdcce95fc275768d99159c70f57a07af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756023"
---
# <a name="documentsharinglocationcollectionsetting-soap"></a>DocumentSharingLocationCollectionSetting (SOAP)

L’élément **DocumentSharingLocationCollectionSetting** représente un utilisateur de paramètre qui est une collection de documentation de métadonnées et les emplacements de partage. 
  
[DocumentSharingLocationCollectionSetting (SOAP)](documentsharinglocationcollectionsetting-soap.md)
  
```XML
<DocumentSharingLocationCollectionSetting>
    <DocumentSharingLocations />
</DocumentSharingLocationCollectionSetting>
```

 **DocumentSharingLocationCollectionSetting**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Représente l’emplacement et les métadonnées pour une liste des emplacements de partage de documents.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserSettings (SOAP)](usersettings-soap.md) <br/> |Représente une collection de paramètres utilisateur.  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Éléments du fichier XML Autodiscover SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

