---
title: FileAsMapping
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FileAsMapping
api_type:
- schema
ms.assetid: 2c98e7c6-09b0-47b3-bbf7-8c4ef9510280
description: L’élément FileAsMapping définit comment construire ce qui est affiché pour un contact.
ms.openlocfilehash: 35397ebd5cb9235ad55093b43bde89eef466e672
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518504"
---
# <a name="fileasmapping"></a>FileAsMapping

**L’élément FileAsMapping** définit comment construire ce qui est affiché pour un contact. 
  
```xml
<FileAsMapping/>
```

 **FileAsMappingType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de cet élément est limitée à l’une des valeurs de chaîne suivantes :
  
- Aucun
    
- LastCommaFirst
    
- FirstSpaceLast
    
- Company
    
- LastCommaFirstCompany
    
- CompanyLastFirst
    
- LastFirst
    
- LastFirstCompany
    
- CompanyLastCommaFirst
    
- LastFirstSuffix
    
- LastSpaceFirstCompany
    
- CompanyLastSpaceFirst
    
- LastSpaceFirst
    
- DisplayName
    
- FirstName
    
- LastFirstMiddleSuffix
    
- LastName
    
- Vide
    
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Création de Contacts (Services Web Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Updating Contacts](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Deleting Contacts](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

