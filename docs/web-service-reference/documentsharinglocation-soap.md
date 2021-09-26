---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: L’élément DocumentSharingLocation contient des informations d’emplacement et de métadonnées pour un emplacement de partage de documents.
ms.openlocfilehash: f4011dfb846d314d926ba644f4ddc2176283008a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541482"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

**L’élément DocumentSharingLocation** contient des informations d’emplacement et de métadonnées pour un emplacement de partage de documents. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |Représente l’URL du service web de partage de documents.  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |Représente l’URL de l’emplacement de partage de documents.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Représente le nom de l’emplacement de partage de documents à utiliser dans l’interface utilisateur.  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |Représente les extensions de fichier qui peuvent être stockées dans l’emplacement de partage de documents.  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |Indique si l’emplacement de partage de documents est disponible pour les connexions externes.  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |Indique si l’accès à l’emplacement de partage nécessite un utilisateur authentifié.  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |Indique si l’utilisateur peut modifier les autorisations d’accès à l’emplacement de partage de documents.  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |Indique si l’emplacement de partage de documents est l’emplacement de partage par défaut de l’utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Contient une liste d’emplacements et de métadonnées de partage de documents.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

