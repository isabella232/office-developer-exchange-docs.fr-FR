---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: L’élément DocumentSharingLocation contient l’emplacement et les informations de métadonnées pour un emplacement de partage de documents.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756024"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

L’élément **DocumentSharingLocation** contient l’emplacement et les informations de métadonnées pour un emplacement de partage de documents. 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 **DocumentSharingLocation**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |Représente l’URL du service web de partage de document.  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |Représente l’URL de l’emplacement de partage de documents.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Représente le nom de l’emplacement à utiliser dans l’interface utilisateur de partage de documents.  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |Représente les extensions de fichier qui peuvent être stockées dans l’emplacement de partage de documents.  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |Indique si l’emplacement de partage de documents sont disponible à l’extérieur des connexions.  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |Indique si l’accès à l’emplacement de partage requiert qu’un utilisateur authentifié.  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |Indique si l’utilisateur peut modifier les autorisations d’accès à l’emplacement de partage de documents.  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |Indique si l’emplacement de partage de documents sont par défaut de l’utilisateur à l’emplacement de partage.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Contient une liste d’emplacements et les métadonnées de partage de documents.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
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

