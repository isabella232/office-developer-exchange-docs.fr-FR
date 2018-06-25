---
title: ServerVersionInfo (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: L’élément ServerVersionInfo contient la version du serveur qui a traité la demande.
ms.openlocfilehash: b02071e4997aba91fb538d52df2612fe6fd32800
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829385"
---
# <a name="serverversioninfo-soap"></a>ServerVersionInfo (SOAP)

L’élément **ServerVersionInfo** contient la version du serveur qui a traité la demande. 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 **ServerVersionInfo**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MajorVersion (SOAP)](majorversion-soap.md) <br/> |Le numéro de version principal pour le serveur.  <br/> |
|[MinorVersion (SOAP)](minorversion-soap.md) <br/> |Numéro de version secondaire pour le serveur.  <br/> |
|[MajorBuildNumber (SOAP)](majorbuildnumber-soap.md) <br/> |Numéro de version majeur pour le serveur.  <br/> |
|[MinorBuildNumber (SOAP)](minorbuildnumber-soap.md) <br/> |Numéro de version secondaire pour le serveur.  <br/> |
|[Version (SOAP)](version-soap.md) <br/> |Description de la version de produit du serveur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est retourné dans l’en-tête SOAP.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

